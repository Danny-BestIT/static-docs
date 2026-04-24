# Privacy Policy — LS Duet

**Last updated:** April 24, 2026

This Privacy Policy explains how LS Duet ("the App", "we", "our") collects, uses, stores, and protects your information when you use the App. LS Duet is operated by Dan Shor as an individual developer.

By using the App you agree to the practices described below. If you do not agree, please do not use the App.

> **Pilot Notice.** The App is currently offered as a **closed pilot / beta program**, made available to a limited group of invited testers until further notice. Some of the data practices described below — in particular the temporary server-side retention window — reflect this pilot phase and will be revisited before any wider release. We will update this Privacy Policy if and when the pilot ends.

---

## 1. What the App Does

LS Duet is a personal messaging assistant that helps you:

- Translate incoming and outgoing messages between languages on a per-contact basis.
- Schedule messages to be sent at a chosen time.
- Keep a local contacts directory, knowledge base, and task list.

You connect the App to your own WhatsApp account. The App does not create WhatsApp accounts or replace the WhatsApp client.

---

## 2. Information We Collect

We collect only the minimum information needed to provide the features above.

### 2.1 Account Information

When you sign in, we collect:

- **Email address** and **name** (from Firebase Authentication, Google Sign-In, or Sign in with Apple).
- A unique user identifier issued by the authentication provider.

If you sign in with Apple and choose to hide your email, we receive only Apple's anonymized relay address.

### 2.2 WhatsApp Integration

To bridge your WhatsApp account into the App, we process:

- **Your WhatsApp session state** — required to keep your connection active. Stored encrypted in our backend, linked to your account only.
- **Phone numbers and display names** of the contacts and groups you exchange messages with, so conversations can be organized.
- **Message content** — transmitted through our servers so it can be delivered to your device, translated (if you enabled translation for that contact), and displayed.

During the current pilot phase, message content is kept on our servers for a **maximum of 48 hours** and then automatically deleted. This temporary retention is used only to (a) deliver messages reliably to your device even if you are briefly offline, (b) allow us to diagnose and fix issues reported during the pilot, and (c) compute aggregate, non-identifying pilot-program metrics (for example, how many messages were delivered successfully). It is **not** used for advertising, profiling, or any AI training. The 48-hour retention is specific to the pilot phase and will be reviewed before any general release.

We never post, send, or read messages on your behalf outside of actions you explicitly initiate in the App.

### 2.3 Contacts

If you choose to import contacts, we access your **device contacts** (the iOS or Android contacts store) with your explicit permission granted through the operating system prompt.

Imported contacts are stored **locally on your device** (in the App's private database) and on our backend only in the minimum form needed to attach translation settings or scheduled messages to a contact.

### 2.4 User-Generated Content

The following are stored locally on your device and, where required for cross-device use, on our backend linked to your user account:

- Per-contact translation settings (source language, target language, glossary).
- Scheduled messages (phone number, content, scheduled time).
- Knowledge-base items you create.
- Tasks and reminders you create.

### 2.5 Device and Technical Information

- **Push notification token** (Expo Push Token) — used to deliver notifications about new messages. Stored linked to your user account.
- **App language preference** and **device timezone** — stored locally and used to display times correctly.
- **App version and crash logs** — collected through Apple's and Google's standard crash reporting to help us fix issues. This data is not linked to your identity.

### 2.6 What We Do Not Collect

- We do not collect advertising identifiers (IDFA / GAID).
- We do not track you across apps or websites.
- We do not sell your data.
- We do not use your message content to train AI or for analytics.

---

## 3. How We Use Your Information

We use the information collected only to:

- Authenticate you and keep your session active.
- Synchronize messages between your device and the WhatsApp service.
- Translate messages, when you have enabled translation for a contact.
- Schedule and deliver messages at the time you chose.
- Send push notifications about new messages.
- Fix bugs, improve reliability, and protect against abuse.

We do **not** use your information for advertising, profiling, or any purpose unrelated to operating the App.

---

## 4. Third-Party Service Providers

We use a small number of third-party services strictly as infrastructure. They process data on our behalf under their own contractual and legal obligations.

| Provider | Purpose | Data Shared |
|---|---|---|
| **Google Firebase** (Authentication, Firestore, Cloud Functions, Cloud Messaging) | Backend, authentication, push notifications | Email, user ID, push token, ephemeral WhatsApp session and message data (≤48h) |
| **Anthropic** (Claude API) | Message translation when you enable it per contact | Only the specific message text being translated. No user identifiers, phone numbers, or metadata. Anthropic does not retain the text for training. |
| **Apple** | Sign in with Apple (iOS only) | Apple-issued user identifier, email (or anonymized relay), name |
| **Google Identity** | Google Sign-In | Email, user ID, name |

We do not share your data with advertising networks, data brokers, or other parties.

---

## 5. Data Storage and Security

- **Local device storage**: Contacts, messages, tasks, knowledge items, and settings are stored in a private SQLite database inside the App sandbox. On iOS and Android this storage is protected by the OS at the device level.
- **Cloud storage**: Account information, translation settings, scheduled messages, and ephemeral WhatsApp bridging data are stored in Google Firebase (Firestore) under your user account only. Firestore security rules enforce that you are the only authenticated party who can read or write your data.
- **In transit**: All network communication between the App and our backend uses HTTPS/TLS.
- **Retention**: Message content is automatically deleted from our backend within 48 hours. Your account data is kept while your account is active and deleted upon account deletion (see Section 7).

No system is perfectly secure. While we use industry-standard practices, we cannot guarantee absolute security.

---

## 6. International Data Transfers

Our backend runs on Google Cloud infrastructure in the European Union (Firebase region `europe-west3`, Frankfurt, Germany). Your data may be transferred to, processed in, and stored in that region. If you access the App from outside the EU, your data will be transferred to and processed in the EU.

---

## 7. Your Rights

Depending on where you live (EU/EEA, UK, Israel, California, etc.), you may have some or all of the following rights:

- **Access** — request a copy of the personal data we hold about you.
- **Correction** — correct inaccurate data.
- **Deletion** — delete your account and associated data.
- **Portability** — receive your data in a machine-readable format.
- **Withdraw consent** — turn off translation or contacts import at any time in the App.
- **Complain** to a data-protection authority.

To exercise any of these rights, contact us at the email below. We will respond within a reasonable time and at latest within the period required by applicable law.

### Account Deletion

To delete your account and associated data:

1. Inside the App, sign out and uninstall (removes all local device data), **or**
2. Email us at the address below to request complete deletion of your account and backend data.

Backend data is deleted within 30 days of a valid request. Backup copies are purged within 90 days.

---

## 8. Children

LS Duet is not directed at children under 13 (or under 16 in the EU/EEA). We do not knowingly collect personal data from children. If you believe a child has provided us data, contact us and we will delete it.

---

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. When we make material changes, we will notify you through the App (for example, by displaying a notice before you continue using the App) or by email. The "Last updated" date at the top reflects the most recent revision.

---

## 10. Contact

For any question about this Privacy Policy or to exercise any of the rights described above, contact:

**Dan Shor / BestIT**
Email: info@best-it.co.il

---

*This Privacy Policy is provided in English. Translations may be offered for convenience; in case of conflict, the English version governs.*
