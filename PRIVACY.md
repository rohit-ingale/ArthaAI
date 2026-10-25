# Artha AI — Privacy Policy

**Effective date:** October 25, 2026
**Previous version:** September 4, 2026

Artha AI ("Artha", "we", "us", or "our") is operated by Rohit Ingale, an individual developer based in Nashik, Maharashtra, India, and is a personal-finance application built for adults in India. This Privacy Policy explains what information the app processes, why, where it is kept, for how long, and the choices available to you. It is intended to comply with the Digital Personal Data Protection Act, 2023 ("DPDPA") and the Digital Personal Data Protection Rules, 2025, and, to the extent still applicable, the Information Technology Act, 2000 and the rules made under it.

For the purposes of the DPDPA, Rohit Ingale is the **Data Fiduciary** for the personal data described below, and you are the **Data Principal**.

**By downloading, installing, or using Artha, you agree to this policy. If you do not agree, do not use the App.**

## Summary

- Your financial data (transactions, budgets, loans, investments, cards, parsed SMS) is stored **only on your phone**. We do not upload it to our servers.
- Bank SMS are read and parsed **on your phone**. They are never sent to us, except a single masked message you explicitly choose to send in the optional template-learning flow.
- AI features send only what a request needs, **after you agree to it**, with card/account numbers, Aadhaar, PAN, phone numbers, IFSC codes, email addresses and UPI IDs removed first.
- The optional cloud backup is **encrypted on your phone with a passphrase only you know** and stored in your own Google Drive. We cannot read it.
- Artha is for people **aged 18 or older**.
- You can delete your account, and your cloud backup, from inside the app.

## Information we process

- **Account information:** name, email address, authentication identifiers, and sign-in provider details when you create or sign in to an account.
- **Age confirmation:** the date and time you confirmed you are 18 or older and accepted these terms. Stored on your phone.
- **Financial information:** transactions, budgets, investments, loans, credit-card details that you enter, categories, notes, account identifiers such as masked last-four digits, and related preferences. **This data is stored only on your device and is not synced to or held on Artha's servers** — the only exception is the optional encrypted backup described below.
- **Receipt and profile images:** images you choose to scan or use as a profile photo, together with OCR results and scan history. Stored on your phone.
- **Bank SMS information:** if you grant SMS permission on Android, Artha reads SMS messages to detect transaction alerts from recognized bank and NBFC sender IDs (Indian banks notify customers of transactions by SMS; there is no public API for this data).
  - When you first grant the permission, Artha reads transaction SMS from **the last six months, starting from the 1st of that month** (or from an earlier date you had already scanned from, for example one restored from your backup). You can choose a different start date, up to five years back, in Settings.
  - After that, new transaction SMS are read as they arrive, including when the app is closed.
  - Parsing happens entirely on your device using a local template engine covering 50+ Indian bank formats. Messages that do not match a recognized bank or NBFC sender are skipped and are never parsed, stored, or transmitted.
  - Parsed transaction records and the source message text are stored on your device so you can review, edit, or delete them.
  - Artha does not request Call Log permission and does not use SMS access for messaging, backup of messages, or OTP autofill.
- **AI requests:** when you use AI insights or chat (where enabled), Artha sends the financial context that request needs (for example category totals for the period you ask about) and any message you type to our backend, which passes it to Google Gemini to generate a response. See "AI features" below.
- **AI feedback you choose to send:** if you report an AI answer, Artha sends that answer, the reason you picked, and any note you add, with identifiers removed. See "AI features".
- **Optional SMS template learning:** if you explicitly choose "Send" in the template-learning flow (a premium, opt-in feature), Artha sends the displayed masked SMS text and the bank sender ID. Amounts, account numbers, and names are replaced with placeholders before submission. No SMS content is ever sent without this explicit, per-message action.
- **Device and diagnostic information:** push-notification tokens, app/device information, performance information, crash reports, and technical logs supplied by Firebase services. Crash reports are collected only in released versions of the app.
- **Purchase information:** subscription and entitlement information processed through RevenueCat and Google Play. We do not receive or store your full payment-card number.

## Consent and legal basis

We process your personal data on the basis of your consent, given for a specific purpose:

- **Sensitive Android permissions** (SMS, camera, notifications, biometrics) are requested only when relevant to a feature you are using. Granting a permission through the Android system dialog is your consent to the processing described for that feature in this policy.
- **AI features:** before Artha sends anything to the AI service for the first time, it shows you a notice of what is sent, to whom, and where, and asks you to agree. Nothing is sent until you tap "Agree".
- **Optional uploads** (encrypted backup, SMS template learning, AI feedback) happen only when you turn them on or tap to send.

You may withdraw consent at any time, as easily as you gave it: revoke a permission in your device Settings, turn off **Settings → Artha AI → Share data with Artha AI**, or turn off **Backup to Cloud**. Withdrawal stops the related processing going forward; it does not affect processing already carried out.

## How we use information

We use information to provide and secure Artha; authenticate accounts; store your finance data on your device; import and categorize transactions; scan receipts; generate insights; deliver reminders and notifications; manage subscriptions; enforce fair-use limits on AI requests; prevent abuse; troubleshoot crashes and performance; and improve parsing and AI quality when you opt in to an optional submission.

## AI features

Where AI features are enabled:

- **Consent first:** nothing is sent until you agree to the in-app notice. You can withdraw in **Settings → Artha AI** at any time.
- **Minimum data:** each request sends only the context that question needs, not your full ledger.
- **Identifiers removed:** before a request leaves your phone, Artha removes card and account numbers, Aadhaar numbers, phone numbers, PAN, IFSC codes, email addresses and UPI IDs from the text. Our backend removes them again before calling the AI model.
- **Processing:** requests go to our Cloud Function (Google Cloud, United States) and Google Gemini. We do not keep a standing copy of the request or the answer.
- **Usage counts:** to enforce monthly limits, we store a count of AI requests per feature per month against your account identifier.
- **Reported answers:** if you report an AI answer, we store that answer, the reason, and your note or question (identifiers removed) to review AI quality. These reports are **deleted automatically after 90 days**.
- **Not advice:** AI output is general information and may be wrong; see the Terms of Service.

## Where information is stored and shared

**Your financial data (transactions, budgets, investments, loans, credit cards, categories, and parsed SMS records) is stored only in a local database on your device. Artha does not upload, sync, or hold this data on our servers.** We hold only what is needed to run account-level and infrastructure services:

| What | Where | Why |
|---|---|---|
| Account email, name, sign-in identifiers | Firebase Authentication (Google) | So you can sign in |
| Crash reports, performance data, push-notification tokens | Firebase Crashlytics, Performance Monitoring, Cloud Messaging (Google) | Fix crashes, deliver notifications |
| AI request context and messages, in transit only | Our Cloud Function (Google Cloud, United States) and Google Gemini | Generate the AI answer |
| Monthly AI usage counts | Cloud Firestore (Google) | Enforce fair-use limits |
| Reported AI answers (90 days) | Cloud Firestore (Google) | Review AI quality |
| Masked SMS text you choose to send | Our backend (Google Cloud) | Improve SMS parsing |
| Subscription status | RevenueCat and Google Play | Manage your subscription |
| Encrypted backup (optional) | A hidden app folder in **your own** Google Drive | Restore your data on a new phone |

**Optional encrypted cloud backup:** if you turn on Backup to Cloud, Artha encrypts your data on your phone (AES-256-GCM, with a key derived from your passphrase using Argon2id) before uploading it to a hidden app folder in your own Google Drive. The backup contains your financial records (including records you deleted, so they stay deleted after a restore) and your in-app settings (currency, monthly budget, fiscal-year start, ignored SMS accounts and cards, account order, and the date SMS were scanned from). Your passphrase never leaves your phone; nobody at Artha, and not Google, can read the backup. If you forget the passphrase, the backup cannot be recovered. You can delete it at any time in **Settings → Data → Delete cloud backup**.

We do not sell your personal information and do not share your financial records with advertisers. We may disclose information to the service providers above that operate the app, when required by law, or when necessary to protect the security and rights of Artha or its users.

### Cross-border data processing

The service providers listed above (Google/Firebase, Google Gemini, RevenueCat) process data on servers outside India, including in the **United States** (our Cloud Functions run in Google Cloud's `us-central1` region). This is limited to the account, diagnostic, AI-request and opt-in data described above — never your locally stored financial ledger. The DPDPA permits transfer of personal data outside India except to countries restricted by the Central Government; we do not knowingly transfer data to any such country.

## Retention

| Data | Kept for |
|---|---|
| Financial data, SMS records, images on your phone | Until you delete it, use **Reset app data**, delete your account, or uninstall the app |
| Account (Firebase Authentication) | Until you delete your account |
| Monthly AI usage counts | Until you delete your account |
| Reported AI answers | 90 days, then deleted automatically |
| Crash and performance reports | Kept by Firebase for a limited period under Google's retention settings, then deleted |
| Encrypted backup in your Drive | Until you delete it in the app or in Google Drive |
| Subscription records | As required by RevenueCat, Google Play and tax law |

## Data Principal rights

Subject to the DPDPA and applicable exemptions, you have the right to:

- **Access** a summary of the personal data we hold about you and the processing activities we carry out.
- **Correction, completion and updating** of inaccurate or incomplete personal data.
- **Erasure** of personal data that is no longer necessary for the purpose it was collected, subject to any legal retention obligation.
- **Withdraw consent** at any time, as described above.
- **Grievance redressal**, as described below, before approaching the Data Protection Board of India.
- **Nominate** another individual to exercise these rights on your behalf in the event of your death or incapacity, by writing to us at the contact below.

To exercise any of these rights, contact us using the details in "Grievance redressal" below.

## Your choices and controls

- **Permissions:** decline or revoke SMS, camera, photo, notification, and biometric permissions in your device settings.
- **AI data sharing:** turn off **Settings → Artha AI → Share data with Artha AI**.
- **Your records:** review, edit, or delete transactions and other records in the app; **Settings → Reset app data** erases all financial data on your phone.
- **Cloud backup:** turn off Backup to Cloud, or erase the backup with **Settings → Data → Delete cloud backup**.
- **Delete your account:** **Settings → Delete account** permanently deletes your sign-in account, your AI usage counts and reported AI answers, your purchase record with RevenueCat, and all Artha data on your phone. It does not cancel a Google Play subscription (cancel it in Google Play first) and does not delete a backup in your Google Drive (use **Delete cloud backup** first, or delete it in Google Drive).
- **Notifications:** turn off reminders, alerts and summaries, or hide amounts on the lock screen, in Settings → Notifications.

Uninstalling the app removes data stored on your phone but does not delete your account or your Drive backup.

## Security

Because your financial data lives only on your device, its security depends mainly on your device's own protections — Android's app sandbox and device encryption — together with these measures in Artha:

- **Encrypted backups:** backups are encrypted on your phone before they leave it (AES-256-GCM, passphrase-derived key using Argon2id).
- **App lock:** an optional biometric or device-PIN lock with an auto-lock timer.
- **Screen protection:** released versions block screenshots, screen recording, and the recent-apps preview of Artha's screens.
- **No unencrypted traffic:** the app refuses unencrypted (non-HTTPS) network connections, and Android's automatic app-data backup is turned off so your data is not copied elsewhere unencrypted.
- **Rooted-device warning:** Artha warns you once if your phone appears to be rooted, because rooting removes the app sandbox.
- **Lock-screen privacy:** you can hide amounts in notifications.
- **Server side:** access controls, authenticated requests, App Check where enabled, and Firebase security rules protect the limited data we hold; the AI key is kept on our server, never in the app.

Artha's on-device database is not separately encrypted beyond what Android provides. No method of storage or transmission is completely secure, so please protect your device with a screen lock and keep your account credentials and backup passphrase safe.

### If there is a personal data breach

If a breach affects personal data we hold, we will inform affected users without delay — by email and/or in the app — with a description of what happened, its likely consequences, what we are doing about it, and steps you can take to protect yourself. We will also report it to the Data Protection Board of India, and to CERT-In where required, within the timelines set by law.

## Children

**Artha is only for people aged 18 or older.** When you sign in for the first time, Artha asks you to confirm that you are 18 or older; if you are not, you are signed out. We do not knowingly process personal data of anyone under 18. If you believe a person under 18 is using Artha, contact us and we will delete their account and data.

## Grievance redressal

If you have any concern, question, or complaint about how your personal data is processed, or want to exercise a right listed above, contact:

**Grievance Contact:** Rohit Ingale
**Email:** rohitingale15@gmail.com
**In the app:** Settings → About → Privacy & grievance contact

We will acknowledge your grievance within 7 days and aim to resolve it within 30 days, and in any case within the period required by the DPDP Rules. If you are not satisfied with our response, you may file a complaint with the **Data Protection Board of India** or approach any other competent authority under applicable law.

## Changes to this policy

We may update this Privacy Policy as Artha changes. We will post the updated version here and revise the effective date. For a material change, we will also make reasonable efforts to tell you directly, for example by email or in the app. Your continued use of the app after an update means you accept the revised policy. If you do not accept it, you must stop using the App, and you may delete your account as described above.

## Contact

For privacy questions, grievances, or Data Principal rights requests, write to rohitingale15@gmail.com, use **Settings → About → Privacy & grievance contact** in the app, or contact the project owner through [GitHub](https://github.com/rohit-ingale/ArthaAI).
