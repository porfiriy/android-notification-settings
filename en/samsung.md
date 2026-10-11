# Samsung: notification settings to check

What to check on Samsung phones when notifications and reminders arrive late or do not arrive at all. Paths were last checked on 2026-09-26. Menu labels change between versions of the manufacturer's skin. If a path does not match, look for the setting through the settings search.

Interactive version with a timer test: https://kipriassistant.com/en/tools/android-notifications/samsung/

## 1. Permission to show notifications (key step)

Applies to: Android 13, Android 14 and newer.

**Where to find it.** Settings → Apps → your app → Notifications.

**Why it matters.** Since Android 13 an app has to ask for this separately on first launch. Declining switches off every notification the app has, reminders included, and the dialog never appears again: the only way back is by hand.

## 2. Alarms and reminders (key step)

Applies to: Android 12, Android 13, Android 14 and newer.

**Where to find it.** Settings → Apps → Special app access → Alarms and reminders. Or Settings → Apps → your app → the advanced section.

**Why it matters.** Without this permission the system is free to move a reminder: inexact alarms get batched, and the phone wakes once for all of them, sometimes a minute later, sometimes fifteen. Since Android 14 it is no longer granted automatically even to apps that declare it at install time.

## 3. Battery: remove restrictions (key step)

Applies to: all Android versions.

**Where to find it.** Settings → Apps → your app → Battery → Unrestricted.

**Why it matters.** Doze puts the phone to sleep once it lies still with the screen off, and standby buckets since Android 9 cut background work for apps you rarely open. An exemption lifts both.

## 4. Sleeping apps (key step)

Applies to: all Android versions.

**Where to find it.** Settings → Battery → Background usage limits on One UI 7 and later; on older firmware it is Settings → Battery and device care → Battery → Background usage limits. Make sure the app is in neither Sleeping apps nor Deep sleeping apps, and add it to Never auto sleeping apps.

**Why it matters.** Samsung keeps two lists, sleeping and deep sleeping apps. A deep sleeping app does not run in the background at all and shows no notifications, and it can land there automatically simply because you have not opened it for a few days.

## 5. Notification channel importance

Applies to: all Android versions.

**Where to find it.** Settings → Apps → your app → Notifications → the reminders channel. Set it to urgent, or turn on pop-ups together with sound.

**Why it matters.** A medium-importance channel arrives silently: the notification is in the shade, the sound is not. An app cannot raise its own importance, only you can, so if you once turned it down this is the only place to put it back.

## 6. Do Not Disturb

Applies to: all Android versions.

**Where to find it.** Settings → Notifications → Do Not Disturb → Exceptions. Permission to override the mode is granted to a specific channel, not to the whole app.

**Why it matters.** It does not cancel the notification, it mutes it. If a night schedule runs into your morning, the reminder arrives silently, and from the outside that looks exactly like a reminder that never came.

## 7. Background data

Applies to: all Android versions.

**Where to find it.** Settings → Apps → your app → Mobile data and Wi-Fi → allow background data and allow usage while data saver is on.

**Why it matters.** This one is about sync rather than the reminders themselves: without background data, records from your other devices only arrive when you open the app. Reminders keep working, because they live in the system rather than on the network.

## Sources

- [Samsung US: put unused apps to sleep on a Galaxy phone](https://www.samsung.com/us/support/answer/ANS10003442/)
- [Samsung US: Galaxy battery optimization, Never sleeping apps](https://www.samsung.com/us/support/galaxy-battery/optimization/)

[All brands](../README.md)
