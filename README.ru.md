# Настройки уведомлений Android по маркам телефонов

Почему уведомление опаздывает или не приходит и какую настройку поменять. Восемь семейств телефонов: Pixel и чистый Android, Samsung, Xiaomi / Redmi / POCO, Huawei / Honor, OPPO / realme, OnePlus, vivo / iQOO, Tecno / Infinix.

Данные на русском и английском. Это те же данные, на которых работает [проверка настроек уведомлений](https://kipriassistant.com/tools/android-notifications/) на kipriassistant.com: один файл JSON и по странице на марку.

[English version](README.md)

## Марки

| Марка | Шаги | На сайте |
| --- | --- | --- |
| Чистый Android (Pixel, Motorola) | [ru/pixel.md](ru/pixel.md) | [проверка](https://kipriassistant.com/tools/android-notifications/pixel/) |
| Samsung | [ru/samsung.md](ru/samsung.md) | [проверка](https://kipriassistant.com/tools/android-notifications/samsung/) |
| Xiaomi, Redmi, POCO | [ru/xiaomi.md](ru/xiaomi.md) | [проверка](https://kipriassistant.com/tools/android-notifications/xiaomi/) |
| Huawei, Honor | [ru/huawei-honor.md](ru/huawei-honor.md) | [проверка](https://kipriassistant.com/tools/android-notifications/huawei-honor/) |
| OPPO, realme | [ru/oppo-realme.md](ru/oppo-realme.md) | [проверка](https://kipriassistant.com/tools/android-notifications/oppo-realme/) |
| OnePlus | [ru/oneplus.md](ru/oneplus.md) | [проверка](https://kipriassistant.com/tools/android-notifications/oneplus/) |
| vivo, iQOO | [ru/vivo.md](ru/vivo.md) | [проверка](https://kipriassistant.com/tools/android-notifications/vivo/) |
| Tecno, Infinix | [ru/tecno-infinix.md](ru/tecno-infinix.md) | [проверка](https://kipriassistant.com/tools/android-notifications/tecno-infinix/) |

## Что в файле

В `android-notification-settings.json` четыре списка.

- `steps`: 9 настроек в том порядке, в котором их стоит проверять. У каждой название, причина, по которой она мешает уведомлениям (`why`), и путь в настройках (`where`). `where.default` годится для телефонов без своей записи, ключ марки, например `where.samsung`, заменяет его для этой марки. `androidVersions` и `vendors` говорят, где шаг применим; `null` значит везде. `critical` стоит у шагов, которые чаще всего решают проблему сами.
- `vendors`: марки, шаги, которые есть у каждой, страница на сайте и страницы справки производителя, с которыми сверены пути.
- `symptoms`: какие шаги проверять, если уведомления не приходят совсем, приходят без звука или опаздывают.
- `androidVersions`: группы версий, на которые ссылаются `steps`.

Каждое текстовое поле - объект с ключами `ru` и `en`.

## Как это проверялось

Пути и подписи взяты из справки производителей и документации Android. Страницы справки перечислены у каждой марки в `sources`. У части марок адреса пока не записаны: список пуст, и на странице марки об этом сказано. `checkedAt` - дата последней сверки, а не выгрузки.

Подписи меняются от версии к версии оболочки. На вашем телефоне пункт может называться иначе; там, где справка для разных версий расходится, в тексте предложен поиск по настройкам. Подробнее о том, как мы проверяем: https://kipriassistant.com/how-we-check/

## Как пользоваться

Лицензия CC BY 4.0: берите данные в приложение, раздел помощи или статью и ставьте ссылку на https://kipriassistant.com/tools/android-notifications/ как на источник.

Если пользователи жалуются, что уведомления вашего приложения не приходят, есть готовая ссылка: она открывает проверку с названием вашего приложения в каждом пути. https://kipriassistant.com/tools/for-developers/

## Нашли ошибку

Заведите issue: модель телефона, версия Android и как путь выглядит у вас. Правка сначала попадает на сайт, потом сюда.
