# Android notification settings by phone brand

Why a notification arrives late or never, and which setting to change, for eight families of Android phones: Pixel and stock Android, Samsung, Xiaomi / Redmi / POCO, Huawei / Honor, OPPO / realme, OnePlus, vivo / iQOO, Tecno / Infinix.

The data is in English and Russian. It is the same data that runs the [notification settings checker](https://kipriassistant.com/en/tools/android-notifications/) on kipriassistant.com, exported as one JSON file and as a page per brand.

[Русская версия](README.ru.md)

## Brands

| Brand | Steps | On the site |
| --- | --- | --- |
| Stock Android (Pixel, Motorola) | [en/pixel.md](en/pixel.md) | [checker](https://kipriassistant.com/en/tools/android-notifications/pixel/) |
| Samsung | [en/samsung.md](en/samsung.md) | [checker](https://kipriassistant.com/en/tools/android-notifications/samsung/) |
| Xiaomi, Redmi, POCO | [en/xiaomi.md](en/xiaomi.md) | [checker](https://kipriassistant.com/en/tools/android-notifications/xiaomi/) |
| Huawei, Honor | [en/huawei-honor.md](en/huawei-honor.md) | [checker](https://kipriassistant.com/en/tools/android-notifications/huawei-honor/) |
| OPPO, realme | [en/oppo-realme.md](en/oppo-realme.md) | [checker](https://kipriassistant.com/en/tools/android-notifications/oppo-realme/) |
| OnePlus | [en/oneplus.md](en/oneplus.md) | [checker](https://kipriassistant.com/en/tools/android-notifications/oneplus/) |
| vivo, iQOO | [en/vivo.md](en/vivo.md) | [checker](https://kipriassistant.com/en/tools/android-notifications/vivo/) |
| Tecno, Infinix | [en/tecno-infinix.md](en/tecno-infinix.md) | [checker](https://kipriassistant.com/en/tools/android-notifications/tecno-infinix/) |

## What is in the file

`android-notification-settings.json` has four lists.

- `steps`: 9 settings to check, in the order to check them. Each has a title, the reason it blocks notifications (`why`) and the path in settings (`where`). `where.default` is the path for phones without their own entry; a brand key such as `where.samsung` replaces it for that brand. `androidVersions` and `vendors` say where the step applies; `null` means everywhere. `critical` marks the steps that most often fix the problem alone.
- `vendors`: the brands, the steps that exist on each, the page on the site and the manufacturer help pages the paths were checked against.
- `symptoms`: which steps to check for "never arrive", "arrive without sound" and "arrive late".
- `androidVersions`: the version groups used in `steps`.

Every text field is an object with `ru` and `en`.

## How it was checked

Paths and labels come from the manufacturers' own help pages and from the Android documentation. The pages are listed per brand in `sources`. Some brands have no sources recorded yet; their list is empty and the brand page says so. `checkedAt` is the date of the last check, not of the last export.

Labels change between versions of a skin. A path here may be named differently on your phone, and where the help pages disagree between versions the text says to use the settings search. More on the method: https://kipriassistant.com/en/how-we-check/

## Using it

The licence is CC BY 4.0: use the data in an app, a help centre or an article, and link back to https://kipriassistant.com/en/tools/android-notifications/ as the source.

If your users complain that your app's notifications do not arrive, there is also a ready link that opens the checker with your app's name in every path: https://kipriassistant.com/en/tools/for-developers/

## Found a mistake

Open an issue with the phone model, the Android version and what the path looks like on your phone. Corrections go into the site first and then into this repository.
