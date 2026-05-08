# Privacy Policy — Zplit

**Last updated:** <<DATA_PUBLICACAO>>

> The Portuguese version is the legally binding text. This English translation is provided for convenience. See [/pt/privacidade](../pt/privacidade).

---

## §1 About us

Zplit (`<<NOME_FANTASIA>>`) is an application developed and operated by **<<RAZAO_SOCIAL>>**, a Brazilian company registered under CNPJ no. **<<CNPJ>>**, headquartered in **<<CIDADE_UF>>**, Brazil. For any matter related to this Privacy Policy or the processing of your personal data, the official contact channel is the email **<<EMAIL_SUPORTE>>**.

Under the terms of **Brazilian Resolução CD/ANPD nº 2/2022**, Zplit operates as a **small-scale data processing agent**. For this reason, **we have not appointed a formal Data Protection Officer (DPO)**; the email **<<EMAIL_SUPORTE>>** is the official communication channel with data subjects and with the Brazilian National Data Protection Authority (ANPD), as permitted by the simplified regime.

## §2 Scope

This Privacy Policy describes how we process your personal data when you use the **Zplit application** (Android, iOS and Windows) and its associated services, which include:

- The **Supabase-hosted backend** (authentication, database, RPCs);
- The **receipt-import flow** powered by artificial intelligence.

This policy applies to all Zplit users, regardless of device or app language.

## §3 Data we collect

We collect only the data strictly necessary for the application to function. We organize it into four groups:

### 3.a Account data

- **Email** — used for login, password recovery, and as your account identifier.
- **Name** — displayed in the app and in WhatsApp messages you send.
- **Phone** (optional) — only if you choose to fill it in your profile.

### 3.b Data about your participants (third parties)

When you add participants to an event, you provide their names and phone numbers. **You are the controller of that third-party data under Brazilian LGPD / EU GDPR; Zplit acts as the processor (operator)**, processing it on your instructions. The legal relationship is as follows:

- **You are the controller of that data.** You decide which participants to add, what data to provide, and for what purpose.
- **Zplit acts as the processor (operator)**, handling that data strictly according to your instructions (storing it, calculating expense splits, generating reminder messages via WhatsApp).
- **You are responsible** for obtaining each participant's consent before adding them, as well as for informing them that the data is being processed by Zplit on your behalf.

We recommend not adding participants without their knowledge.

### 3.c Receipt images

When you use the **import items from a receipt** feature, the image is sent to **Google (Gemini API)** for automatic item extraction. Important:

- The original image is **not stored** after processing.
- We keep only an **audit record** (`receipt_imports`) with the operation status (success, failure, failure reason) for **up to 30 days**, exclusively for usage-limit enforcement and abuse prevention.
- The extracted items become part of the event as any other expense, under your control.

### 3.d What we do NOT collect

To make clear what is out of scope for Zplit:

- **We do not use third-party analytics** (Google Analytics, Firebase Analytics, Mixpanel, Amplitude, etc.).
- **We do not use advertising networks** (AdMob, Meta Audience Network, etc.).
- **We do not access your device contacts.**
- **We do not collect location data** (GPS, IP-geolocation, etc.).
- **We do not collect biometric data** (face, fingerprint, etc.).
- **We do not process payment data** or credit card information — Zplit only calculates amounts; transfers between you and your participants happen outside the app.

## §4 How we use your data

Each processing purpose is mapped to a legal basis under both **Brazilian LGPD Art. 7** and **EU GDPR Art. 6**:

- **Allow registration, login, password recovery and account deletion** — legal basis: **performance of a contract** (LGPD Art. 7 V / GDPR Art. 6(1)(b)).
- **Save and display your events, participants, expenses and split calculations** — legal basis: **performance of a contract** (LGPD Art. 7 V / GDPR Art. 6(1)(b)).
- **Import items from a receipt** (sending the image to the Gemini API) — legal basis: **performance of a contract** (LGPD Art. 7 V / GDPR Art. 6(1)(b)) — you expressly requested this operation.
- **Prevent abuse, fraud, and violations of these Terms** (usage limits, audit records) — legal basis: **legitimate interests** (LGPD Art. 7 IX / GDPR Art. 6(1)(f)).
- **Respond to data-subject rights requests** (LGPD Art. 18 / GDPR Chapter III) — legal basis: **compliance with a legal obligation** (LGPD Art. 7 II / GDPR Art. 6(1)(c)).

We do not process your data for any purpose other than those above without first updating this Policy and notifying you in the app.

## §5 With whom we share your data

Zplit shares personal data only with the following named processors, and exclusively for the purposes described:

| Third party | Role | Data shared | Policy |
|---|---|---|---|
| **Supabase, Inc.** | Infrastructure (authentication, database, hosting) | All application data (account, events, participants, expenses) | https://supabase.com/privacy — DPA: https://supabase.com/legal/dpa |
| **Google LLC (Gemini API)** | Receipt-image processing | Image you submit + extracted text | https://policies.google.com/privacy |
| **WhatsApp** (Meta) | Sending a message **initiated by you** via deep link | Only the content of the message you choose to send | https://www.whatsapp.com/legal/privacy-policy |

About WhatsApp: Zplit **never sends messages on your behalf**. When you tap "Send via WhatsApp", Zplit only **opens the WhatsApp app** installed on your device with the message pre-filled. The sending is performed by your own WhatsApp app, under your credentials and your responsibility.

**We do not sell your data. We do not share your data for advertising purposes.** We have no commercial partnerships or affiliate programs that involve the transfer of personal data.

## §6 Where your data is stored

Your data is stored on the **Supabase** infrastructure, in the **<<SUPABASE_REGION>>** region. Receipt images are processed during parsing by **Google (Gemini API)**, whose infrastructure is located in the **United States**.

Because international data transfers occur, we adopt the **Standard Contractual Clauses (SCCs)** included in the **Supabase Data Processing Addendum (DPA)** as the transfer safeguard. We rely on these SCCs for both LGPD purposes (Art. 33, international transfer based on specific contractual safeguards) and GDPR purposes (Chapter V, Articles 44-46), in line with international data-protection best practices.

## §7 How long we keep your data

- **Personal data and event data**: kept while your account is active.
- **Upon deletion of your account** (Profile → Delete account): all associated data (events, participants, expenses, payments) is deleted **immediately and in cascade**. The operation is irreversible.
- **Receipt-import audit log** (`receipt_imports`): kept for **up to 30 days** for usage-limit enforcement and abuse prevention. After this period, it is automatically deleted.
- **Backups**: the Supabase infrastructure keeps short-term backups for service-continuity purposes; after account deletion, data is removed from backups according to the Supabase retention policy.

## §8 Your rights

Under **Brazilian LGPD Art. 18**, you have the following rights regarding your personal data:

1. **Confirmation** of the existence of processing;
2. **Access** to your data;
3. **Correction** of incomplete, inaccurate or outdated data;
4. **Anonymization, blocking or deletion** of unnecessary, excessive or non-compliant data;
5. **Portability** of your data to another provider;
6. **Deletion** of personal data processed with your consent;
7. **Information** about the public and private entities with which Zplit has shared your data;
8. **Information** about the possibility of withholding consent and the consequences of doing so;
9. **Withdrawal of consent**, at any time.

**If you are an EU/EEA resident**, in addition to the rights above, you have the rights granted by the EU General Data Protection Regulation (GDPR), including the right to access, rectify, erase, restrict, port and object to the processing of your data. **You also have the right to lodge a complaint with the data protection supervisory authority in your country of residence** if you believe our processing of your data does not comply with applicable law.

**How to exercise:** send an email to **<<EMAIL_SUPORTE>>**. We respond within **15 calendar days**. For **account deletion**, you can also use the self-service flow at **Profile → Delete account**, which executes the deletion immediately without waiting for our reply.

There is no cost for exercising your rights.

## §9 Children

Zplit **has no minimum-age restriction** for access. Users under 18 may use the application provided that they have the **consent and supervision of their parents or legal guardians**.

The **processing of personal data of children (under 12 years of age)** is performed **only with the specific and prominent consent** of at least one of the parents or legal guardians, in accordance with **LGPD Art. 14**. We do not condition a child's participation in the app on the provision of data beyond what is strictly necessary.

Parents or legal guardians may, at any time, request the **deletion of the data** of the child or adolescent in their care by emailing **<<EMAIL_SUPORTE>>**. Requests are addressed within 15 days.

## §10 Security

We adopt technical and administrative measures appropriate to the scale of our operation to protect your personal data:

- **HTTPS (TLS) communication** on all requests between the app and the backend.
- **Encryption at rest** within the Supabase infrastructure.
- **Data isolation via Row Level Security (RLS)**: each user can only access their own data; the database is configured to refuse cross-user access, even in the event of an application bug.
- **Cascade deletion** when removing an account: all associated data is deleted in the same transaction.
- **Usage limits** (rate limits) on sensitive operations, to reduce the risk of abuse and fraud.

No system is absolutely secure. In the event of a **security incident that may pose relevant risk or harm** to data subjects, we will notify the **ANPD and affected data subjects** within a reasonable period, as required by **LGPD Art. 48**, and any equivalent supervisory authorities under applicable foreign law.

## §11 Cookies, analytics and advertising

**We currently do not use cookies, third-party analytics, or advertising networks.** The Zplit application does not integrate Google Analytics, Firebase Analytics, Mixpanel, Amplitude, AdMob, Meta Audience Network, Sentry, Crashlytics, or any similar tool.

If we begin to use any of these technologies in the future, we will update this Privacy Policy and notify users in the app before deployment, with reasonable time for you to review and, if you prefer, close your account.

## §12 Changes to this policy

We may update this Privacy Policy from time to time to reflect changes in law, operational practices, or app functionality. The date in **"Last updated"** (at the top of the document) will always reflect the most recent version.

In case of **material changes** (for example, a new sub-processor, a new processing purpose, or a change in legal basis), we will display a **prominent in-app notice** before the new version takes effect, with reasonable time for your review.

## §13 Contact

For any question about this Policy, exercise of data-subject rights, incident report, or any other matter related to personal data, please contact us at:

**<<EMAIL_SUPORTE>>**

---

**Last updated:** <<DATA_PUBLICACAO>>
