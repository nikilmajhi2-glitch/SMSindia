# SMSindia

Private task-based earning Android app (Android 15+). Users earn for sending SMS messages. This repo contains the initial project skeleton: Android app (Kotlin), Firebase rules, sample Cloud Function, and documentation. Replace placeholders (google-services.json, admin UIDs) before building.

Features (planned):
- SMS sending using device SIM (multi-SIM aware)
- Runtime permission flow and consent
- Background sending with WorkManager
- Firebase integration: Authentication, Firestore for users, sms logs, inventory, withdrawals
- Admin-configured daily SMS inventory
- Withdrawals: single bank account per user (INR), admin approval via Cloud Function

Setup
1. Add your Firebase `google-services.json` to `app/`.
2. Open the project in Android Studio (keep Gradle and plugin versions aligned to your environment).
3. Update `app/build.gradle` with Firebase BOM versions if needed.

Important notes
- This is a private app; still ensure users consent before sending SMS.
- The app requests SEND_SMS and READ_PHONE_STATE runtime permissions.
