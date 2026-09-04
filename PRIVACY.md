# Artha AI — Privacy Policy

**Effective date:** September 4, 2026

Artha AI ("Artha", "we", "us", or "our") is operated by Rohit Ingale, an individual developer based in Nashik, Maharashtra, India, and is a personal-finance application built for users in India. This Privacy Policy explains what information the app may process, why it is processed, and the choices available to you. It is intended to comply with the Digital Personal Data Protection Act, 2023 ("DPDPA"), and, to the extent still applicable, the Information Technology Act, 2000 and the rules made thereunder.

For the purposes of the DPDPA, Rohit Ingale is the **Data Fiduciary** in respect of the personal data described below, and you are the **Data Principal**.

**By downloading, installing, or using Artha, you agree to this policy. If you do not agree, do not use the App.**

## Information we process

- **Account information:** name, email address, authentication identifiers, and sign-in provider details when you create or sign in to an account.
- **Financial information:** transactions, budgets, investments, loans, credit-card details that you enter, categories, notes, account identifiers such as masked last-four digits, and related preferences. **This data is stored only on your device and is not synced to or held on Artha's servers** — the only exception is the optional, user-initiated encrypted backup described below.
- **Receipt and profile images:** images you choose to scan or use as a profile photo, together with OCR results and scan history.
- **Bank SMS information:** if you grant SMS permission on Android, Artha reads incoming SMS messages to detect transaction alerts from recognized bank and NBFC sender IDs (Indian banks notify customers of transactions exclusively via SMS; there is no public API for this data). Parsing happens entirely on your device using a local template/regex engine covering 50+ Indian bank formats. Messages that do not match a recognized bank or NBFC sender are discarded immediately and are never parsed, stored, or transmitted anywhere. Parsed transaction records and, where applicable, the source message text are stored locally on your device so you can review, edit, or delete them. Artha does not request or use Call Log permission, and does not use SMS access for messaging, backup, or OTP autofill.
- **AI requests:** when you use AI insights or chat (where enabled), Artha sends the selected financial context and any message you submit to our backend so it can generate a response. Do not submit information you do not want processed by an AI service.
- **Optional SMS template learning:** if you explicitly choose "Send" in the template-learning flow (a premium, opt-in feature), Artha sends the displayed masked SMS text and the bank sender ID. Amounts, account numbers, and names are replaced with placeholders before submission. No SMS content is ever sent without this explicit, per-message action.
- **Device and diagnostic information:** push-notification tokens, app/device information, performance information, crash reports, and technical logs supplied by Firebase services when those services are enabled.
- **Purchase information:** subscription and entitlement information processed through RevenueCat and the relevant app-store provider. We do not receive or store your full payment-card number.

## Consent and legal basis

Where Artha requests a sensitive Android permission (e.g. SMS, Camera, Biometric), we ask for it only when relevant to a specific feature you are trying to use, and processing begins only after you grant that permission through the Android system dialog. Granting a permission is your specific, informed, and affirmative consent to the processing described for that feature in this policy. You may withdraw consent at any time by revoking the permission in your device Settings, which stops the related processing going forward (see "Your choices and controls" below); withdrawal does not affect the lawfulness of processing already carried out.

## How we use information

We use information to provide and secure Artha; authenticate accounts; store and synchronize your finance data; import and categorize transactions; scan receipts; generate insights; deliver reminders and notifications; manage subscriptions; prevent abuse; troubleshoot crashes and performance; and improve parsing and product reliability when you opt in to an optional submission.

## Where information is stored and shared

**Your financial data (transactions, budgets, investments, loans, credit cards, categories, and parsed SMS records) is stored only in a local database on your device. Artha does not upload, sync, or hold this data on our servers.** We only ever hold what's necessary to run account-level and infrastructure services:

- **Firebase Authentication:** your account email/identifier and sign-in provider details, so you can sign in.
- **Firebase Crashlytics, Performance Monitoring, and Cloud Messaging:** device/app diagnostic information and push-notification tokens, when those services are enabled.
- **AI requests** (where AI features are enabled): the specific financial context and message you submit for that request are sent to our secured backend and Google Gemini to generate a response. They are not retained as a standing copy of your data.
- **Optional SMS template learning** (opt-in, premium): only the masked message text described above, per explicit submission.
- **Optional encrypted cloud backup:** if you turn on backup to your own Google Drive, your data is encrypted on-device with a passphrase only you know before upload — Google stores only the encrypted blob, in your Drive, and nobody at Artha can read it.
- **Subscription data** is processed by RevenueCat and the applicable app store.

We do not sell your personal information. We do not share your financial records with advertisers. We may disclose information to service providers that operate the app, when required by law, or when necessary to protect the security and rights of Artha or its users.

### Cross-border data processing

The service providers listed above (Firebase/Google Cloud, Google Gemini, RevenueCat) may process data on servers located outside India. Where this occurs, it is limited to the account, diagnostic, and opt-in data described above — never your locally-stored financial ledger. The DPDPA permits transfer of personal data outside India except to countries specifically restricted by the Central Government; we do not knowingly transfer data to any such restricted country.

## Data Principal rights

Subject to the DPDPA and applicable exemptions, you have the right to:

- **Access** a summary of the personal data we hold about you and the processing activities we carry out.
- **Correction and completion** of inaccurate or incomplete personal data.
- **Erasure** of personal data that is no longer necessary for the purpose it was collected, subject to any legal retention obligation.
- **Withdraw consent** at any time, as described above.
- **Grievance redressal**, as described below, before approaching the Data Protection Board of India.
- **Nominate** another individual to exercise these rights on your behalf in the event of your death or incapacity.

To exercise any of these rights, contact us using the details in "Contact" below. We will respond within a reasonable time, and in any case as required by applicable law.

## Your choices and controls

You can decline or revoke camera, photo, SMS, notification, and biometric permissions through your device settings. You can review, correct, or delete records in the app where those controls are available. You may also request access to, correction of, or deletion of account information by contacting us through the [Artha AI GitHub repository](https://github.com/rohit-ingale/ArthaAI). Deleting the app removes locally stored data, but may not delete data already stored in cloud services; contact us to request cloud-account deletion.

## Retention and security

We retain information for as long as needed to provide the service, maintain your account, meet legal obligations, resolve disputes, and enforce agreements. Local data remains until you delete it or uninstall the app.

Because your financial data lives only on your device, its security depends primarily on your device's own protections: Android's app-sandboxing and, if you've enabled it, full-disk encryption, plus Artha's own biometric app-lock as an optional extra layer at the app level. Artha's on-device database is not independently encrypted beyond what the operating system provides. Optional cloud backups are encrypted before they ever leave your device, as described above. We use access controls, authenticated requests, and Firebase security rules to protect the account and diagnostic information we do hold. No method of storage or transmission is completely secure, so please protect your device (e.g. with a screen lock) and account credentials.

## Children

Artha is not directed to children under 13, and we do not knowingly collect personal information from children under 13. If you believe a child has provided information, contact us so we can investigate and delete it where appropriate.

## Grievance redressal

If you have any concern, question, or complaint about how your personal data is processed, contact:

**Grievance Contact:** Rohit Ingale
**Email:** rohitingale15@gmail.com

We will acknowledge and address grievances within a reasonable time. If you are not satisfied with our response, you may file a complaint with the **Data Protection Board of India** or approach any other competent authority under applicable law.

## Changes to this policy

We may update this Privacy Policy as Artha changes. We will post the updated version here and revise the effective date. Your continued use of the app after an update means you accept the revised policy. If you do not accept the revised policy, you must stop using the App.

## Contact

For privacy questions, grievances, or Data Principal rights requests, contact the project owner through [GitHub](https://github.com/rohit-ingale/ArthaAI) or at rohitingale15@gmail.com.
