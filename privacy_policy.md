# Privacy Policy — MyMedi App

**Last Updated**: September 27, 2026

At **MyMedi** ("we", "our", or "us"), your privacy is our foundational principle. This Privacy Policy describes how your information is handled when you use the MyMedi mobile application ("App").

---

## 1. Zero-Knowledge Architecture (No Personal Data Collection)

MyMedi is designed from the ground up as a **zero-cloud, zero-backend, offline-first** application:

* **No Accounts or Logins**: We do not ask for, collect, or store your name, email address, phone number, or credentials.
* **No Cloud Servers**: Your medications, dosage times, inventory quantities, adherence logs, and doctor notes are stored strictly on your device inside an embedded SQLite database.
* **No Proprietary Telemetry or Tracking**: We do not build, operate, or maintain our own analytics servers, user tracking systems, or behavioral monitoring tools.
* **Anonymous Crash & Diagnostic Reports**:
  * **Android Vitals / Google Play**: Like all standard Android applications, if an unexpected error or crash occurs, Android OS may collect anonymous diagnostic crash data (such as stack trace, device manufacturer/model, and OS version) via Google Play services to help developers fix bugs. This data contains no personally identifiable or medical information.
  * **AdMob Performance & Diagnostics**: As detailed in Section 3, the third-party Google Mobile Ads SDK may gather technical performance and diagnostic logs (e.g., ad load latency, SDK errors, and pseudonymous device identifiers) strictly for ad delivery, fraud prevention, and service stability. None of your medical, pill, or scheduling data is ever shared with or accessible to AdMob.

---

## 2. Permissions Required & Justification

MyMedi requests only the minimum operating system permissions strictly necessary to execute its core reminder features:

1. **Exact Alarms (`SCHEDULE_EXACT_ALARM`, `USE_EXACT_ALARM`)**:
   Required to trigger high-priority medication reminders at exact scheduled minute intervals.
2. **Post Notifications (`POST_NOTIFICATIONS`)**:
   Required on Android 13+ to display dose reminder notification alerts and low-stock refill warnings.
3. **Boot Completed (`RECEIVE_BOOT_COMPLETED`)**:
   Required to re-register scheduled medication alarms if your device powers down or reboots.
4. **Vibration & Wake Lock (`VIBRATE`, `WAKE_LOCK`)**:
   Required to momentarily wake the device display and sound reminder alerts when doses are due.

---

## 3. Advertising & Third-Party SDKs

MyMedi is sustained through non-intrusive bottom banner advertising provided by **Google AdMob**:

* Google AdMob may collect and process pseudonymous identifiers (such as Google Advertising ID / IDFA) to serve relevant advertisements, in compliance with Google Play Developer Policies.
* **User Messaging Platform (UMP)**: For users in the European Economic Area (EEA), the UK, and California, MyMedi presents the Google UMP consent dialogue, enabling you to accept, decline, or configure personalized ad tracking.
* For more information on how Google processes ad data, please review [Google's Privacy & Terms](https://policies.google.com/technologies/ads).

---

## 4. Data Deletion & Local Backups

Because MyMedi has no user accounts and no cloud backend, all data deletion is executed directly on your device:

* **How to Delete Data**:
  1. Open the **MyMedi** app.
  2. Go to **Settings**.
  3. Scroll down to the **Danger Zone** section.
  4. Tap **Clear All Data** and confirm.
* **What is Deleted**: All medications, dose records, adherence logs, notes, and preferences are permanently and immediately erased from your local SQLite database. No copies exist on any external server.
* **Uninstallation**: Uninstalling the MyMedi app immediately and permanently purges all app data from your device.
* **Local Backups**: You can export an unencrypted or tamper-verified `.mymedi` local JSON backup file to your own storage at any time via **Settings > Backup & Restore**.

---

## 5. Children's Privacy

MyMedi is designed for adults, seniors, and caregivers. We do not knowingly collect any personally identifiable information from children under the age of 13.

---

## 6. Contact Us

If you have questions or concerns regarding this Privacy Policy or MyMedi's offline architecture, please contact us via our public repository:
* **GitHub Repository**: [https://github.com/ParikshitGupta/MyMedi_App](https://github.com/ParikshitGupta/MyMedi_App)
