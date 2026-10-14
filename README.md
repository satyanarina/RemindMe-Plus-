# RemindMe+ — Smart Accountability Reminder

RemindMe+ is an Android starter project for reminders plus accountability. It begins with a small native Kotlin MVP and is designed to be extended carefully.

## Current starter features
- Create a task with date and time
- One-time or daily reminders
- Android notification scheduling
- Mark tasks completed or missed
- Virtual points (+10 / -10)
- Local task storage
- Re-schedule pending tasks after device reboot (best effort)

## Not implemented yet
- Photo proof and automatic secure deletion
- Location/geofence reminders
- Firebase login and cloud sync
- Friend notifications
- Payment integration
- AI prioritization
- A guarantee of sound while Silent/DND is enabled

These are planned phases, not working features in this starter.

## Build
1. Install the latest stable Android Studio.
2. Open this folder as an existing Android Studio project.
3. Allow Gradle sync to finish.
4. Connect an Android phone with USB debugging enabled, or create an emulator.
5. Run the `app` configuration.
6. Grant notification permission when prompted.
7. Add a reminder a few minutes in the future to test it.

## Requirements
- Android Studio with Android SDK Platform 35 installed
- JDK 17 as configured by your Android Studio installation
- Android device or emulator running Android 8.0+ (API 26+)

## Important behavior and limitations
- Android 13+ requires notification permission.
- Exact alarms can require the user to grant special access on Android 12+; the app falls back to an inexact alarm when access is unavailable.
- Android may delay alarms because of battery optimization, OEM restrictions, or permission settings.
- Ordinary notifications cannot guarantee sound while the device is silent or Do Not Disturb is enabled.
- Daily repetition is a simple 24-hour recurrence in this starter and is not daylight-saving/time-zone robust.
- Task data is stored locally using SharedPreferences JSON for simplicity. For a production app, migrate to Room and add tested backup/recovery.
- This app does not make real-money payments.
- This starter has not been built or device-tested in this environment. Run it in Android Studio and fix any SDK/Gradle issues that your installed versions report before relying on it.

## Privacy and safety
Do not use this app as the sole mechanism for critical medical reminders. A reminder notification does not verify that medication was taken. Use a clinician-approved medication plan and suitable reminder backup.
