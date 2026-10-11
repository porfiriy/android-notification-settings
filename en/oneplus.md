# OnePlus: notification settings to check

What to check on OnePlus phones when notifications and reminders arrive late or do not arrive at all. Paths were last checked on 2026-09-26. Menu labels change between versions of the manufacturer's skin. If a path does not match, look for the setting through the settings search.

Interactive version with a timer test: https://kipriassistant.com/en/tools/android-notifications/oneplus/

## 1. Permission to show notifications (key step)

Applies to: Android 13, Android 14 and newer.

**Where to find it.** Settings → Apps → your app → Notifications. The toggle at the top must be on.

**Why it matters.** Since Android 13 an app has to ask for this separately on first launch. Declining switches off every notification the app has, reminders included, and the dialog never appears again: the only way back is by hand.

## 2. Alarms and reminders (key step)

Applies to: Android 12, Android 13, Android 14 and newer.

**Where to find it.** Settings → Apps → Special app access → Alarms and reminders. Or Settings → Apps → your app → the advanced section.

**Why it matters.** Without this permission the system is free to move a reminder: inexact alarms get batched, and the phone wakes once for all of them, sometimes a minute later, sometimes fifteen. Since Android 14 it is no longer granted automatically even to apps that declare it at install time.

## 3. Battery: remove restrictions (key step)

Applies to: all Android versions.

**Where to find it.** Settings → Battery → Battery optimisation → All apps → your app → Don’t optimise. If there is no such screen, open the app’s own battery page and allow background activity, as on OPPO.

**Why it matters.** Doze puts the phone to sleep once it lies still with the screen off, and standby buckets since Android 9 cut background work for apps you rarely open. An exemption lifts both.

## 4. Autostart (key step)

Applies to: all Android versions.

**Where to find it.** App settings → Battery → allow auto launch. On some firmware it is a separate item in the app’s settings; the settings search finds it fastest.

**Why it matters.** The skin refuses to let the app start after a reboot or after it has been cleared from memory. At that point there is nobody to show the reminder: the app is not running and never learns that the time has come.

## 5. Lock the card in recents

Applies to: all Android versions.

**Where to find it.** Open recents, press and hold the app’s card, then tap the padlock in its corner.

**Why it matters.** On Xiaomi, vivo, OPPO, realme, Tecno and Infinix, clearing the recents list unloads the app entirely, along with everything it had scheduled. A locked card survives that, which is why vivo’s and realme’s own help pages recommend it.

## 6. Notification channel importance

Applies to: all Android versions.

**Where to find it.** Settings → Apps → your app → Notifications → the reminders channel. Set it to urgent, or turn on pop-ups together with sound.

**Why it matters.** A medium-importance channel arrives silently: the notification is in the shade, the sound is not. An app cannot raise its own importance, only you can, so if you once turned it down this is the only place to put it back.

## 7. Do Not Disturb

Applies to: all Android versions.

**Where to find it.** Settings → Notifications → Do Not Disturb → Exceptions. Permission to override the mode is granted to a specific channel, not to the whole app.

**Why it matters.** It does not cancel the notification, it mutes it. If a night schedule runs into your morning, the reminder arrives silently, and from the outside that looks exactly like a reminder that never came.

## 8. Background data

Applies to: all Android versions.

**Where to find it.** Settings → Apps → your app → Mobile data and Wi-Fi → allow background data and allow usage while data saver is on.

**Why it matters.** This one is about sync rather than the reminders themselves: without background data, records from your other devices only arrive when you open the app. Reminders keep working, because they live in the system rather than on the network.

## Sources

The manufacturer help pages for this brand are not recorded in the data yet.

[All brands](../README.md)
