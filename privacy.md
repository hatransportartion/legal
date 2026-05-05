---
title: Privacy Policy
layout: default
permalink: /privacy/
---

# Privacy Policy

**Effective date:** 2026-05-05
**Publisher:** Alpha Accounts
**Website:** https://alphalionlogistics.com
**Privacy contact:** sandeep@alphalionlogistics.com

---

## Summary at a glance

- **What we do.** Alpha Accounts copies selected data from your QuickBooks Online company into an Airtable base that you own. You control both endpoints; we sit in the middle.
- **What we never see.** No bank login credentials, no payroll, no employee SSNs, no tax filings, no payment card numbers, no end-user browsing or analytics. OAuth happens between you and Intuit — your password never touches our servers.
- **What we actually store.** OAuth tokens (so we can keep the connection alive) and short-lived copies of the transactions we are in the process of syncing. We do not maintain a long-term database of your QuickBooks records on our infrastructure.
- **Who we share with.** Only Intuit (the source) and Airtable (your chosen destination). We do not sell, rent, trade, or share your data with advertisers, data brokers, or anyone else.
- **How to leave.** Disconnect anytime in QuickBooks → **Apps → Disconnect**. Your tokens are deleted automatically. Email sandeep@alphalionlogistics.com to confirm or to request deletion of any remaining records.

---

## 1. Who this policy covers

This Privacy Policy describes how Alpha Accounts ("we," "us," or "the Publisher"), a company incorporated in Delhi, India, handles personal information when you connect your QuickBooks Online company to Alpha Accounts (the "Service") and the Service mirrors data into your Airtable base.

It applies to the people and businesses ("you" or "Customer") who install or operate the Service. It does not apply to:

- Intuit's handling of your QuickBooks data (see Intuit's privacy notice).
- Airtable's handling of data once it lands in your base (see Airtable's privacy notice).
- Anyone whose information appears inside your QuickBooks records (your customers, vendors, employees) — we are a data processor for that information; you remain the data controller and are responsible for your own privacy disclosures to those individuals.

## 2. What the Service does

Alpha Accounts is a server-side Node.js process. It authenticates to QuickBooks Online using Intuit's OAuth 2.0 flow, listens for webhook notifications and/or polls on a schedule, and writes the resulting transaction records into a table inside an Airtable base that you designate.

There is no end-user user interface beyond the OAuth consent screens hosted by Intuit and Airtable. You install the Service, grant access, point it at your Airtable base, and it runs in the background.

## 3. Data we collect from QuickBooks

When you connect your QuickBooks Online company, the Service receives and processes the following categories of data:

**Authentication data**
- OAuth access token, refresh token, and `realmId` (the identifier for your QuickBooks company).

**Transaction records**, for each synced transaction:
- Transaction date
- Transaction type (Invoice, Bill, Payment, Deposit, Purchase, Journal Entry, Bill Payment)
- Amount and currency
- Account name and account ID
- Memo / description text
- Counterparty name (the customer or vendor on the transaction)

**Chart-of-accounts metadata**
- Account name
- Account type and subtype
- Current balance

**Webhook notifications** from Intuit announcing that a relevant entity has been created, updated, or deleted.

Some of the fields above (counterparty names, memos) may contain personal information about your customers, vendors, or employees. We treat all of it with the safeguards described in Section 7.

## 4. Data we write to Airtable

The Service writes the same transaction fields listed in Section 3 — date, type, amount, currency, account, memo, counterparty — into the table you designate inside your own Airtable base. Once written, that data is governed by Airtable's terms and privacy notice, and by your own Airtable workspace permissions. We do not retain a separate copy of those records once the write is confirmed.

## 5. Data we do NOT collect

We want to be specific about what is **not** in scope:

- **No bank login credentials.** OAuth runs between you and Intuit; we never see banking usernames or passwords.
- **No payroll, employee Social Security numbers, or tax-filing data.** The Service does not request the QuickBooks scopes that would expose payroll or tax data.
- **No payment card numbers.** We do not process payments and never receive PAN, CVV, or related data.
- **No end-user analytics or tracking.** The Service is server-side only. There is no website visitor tracking, no advertising pixels, no behavioral profiling, no device fingerprints.
- **No biometric, geolocation, or health data.**

## 6. Why we collect this data and our legal basis

We collect the data described in Section 3 for one purpose only: **to operate the sync you asked us to operate.** Specifically:

- OAuth tokens — so we can call the QuickBooks API on your behalf and refresh access without asking you to log in again every hour.
- Transaction and account data — so we can mirror it into your Airtable base.
- Webhook notifications — so we know when something has changed and the sync needs to run.

For users in jurisdictions covered by the EU/UK General Data Protection Regulation (GDPR), our legal bases are:

- **Performance of a contract** (GDPR Art. 6(1)(b)) — you have asked us to provide the Service; we need this data to provide it.
- **Consent** (GDPR Art. 6(1)(a)) — you grant access through the Intuit OAuth consent screen, and you can withdraw that consent at any time by disconnecting (see Section 11).
- **Legitimate interests** (GDPR Art. 6(1)(f)) — for security logging and abuse prevention, balanced against your privacy interests.

For California residents and others covered by the California Consumer Privacy Act (CCPA/CPRA), we are a "service provider" (or "business," depending on your role) and we process personal information solely to perform the Service.

## 7. Storage and security

**OAuth tokens.** Tokens are stored on the server filesystem in a file named `.qbo-tokens.<env>.json`, where `<env>` identifies the deployment environment (e.g., `production`, `sandbox`). File permissions are restricted to the application user account; the file is not world-readable. Access tokens expire approximately every 60 minutes and are auto-refreshed before expiry using the refresh token.

**Transit security.** All communication with Intuit and Airtable APIs uses HTTPS over TLS 1.2 or higher. We do not accept insecure connections.

**Webhook authenticity.** Incoming webhook payloads from Intuit are verified using the HMAC-SHA256 signature in the `intuit-signature` header before any data is processed. Unsigned or invalidly-signed payloads are rejected.

**Server location.** The Service runs from servers located in us-east-1 (Northern Virginia, USA). Logs and OAuth token files reside in that same region.

**Operational practices.**
- Access to production servers is limited to authorized engineers and uses key-based authentication.
- Application logs are retained for 30 days and avoid recording transaction-level personal data.
- Dependencies are monitored for known vulnerabilities and patched on a regular cadence.

No system is perfectly secure, but we apply industry-standard safeguards proportional to the sensitivity of the data we handle.

## 8. Data retention

- **OAuth tokens** are retained for as long as you keep the QuickBooks app connected. When you disconnect (in QuickBooks → Apps → Disconnect, or by emailing us), tokens are deleted from our systems within 30 days, typically much sooner.
- **Transaction data in transit.** Transaction records exist on our servers only briefly while a sync is in flight. We do not maintain a persistent database of your QuickBooks transactions on our infrastructure.
- **Airtable.** Data written to your Airtable base is retained according to your Airtable workspace settings — we have no control over and do not access that data after writing it.
- **Logs.** Operational logs are retained for 30 days and then automatically purged.
- **Email correspondence.** Emails you send to sandeep@alphalionlogistics.com are retained for as long as needed to handle your request and to comply with our recordkeeping obligations.

## 9. Sharing with third parties

We share data only with the two services that make the Service possible:

- **Intuit, Inc.** — operator of QuickBooks Online and the source of the data. Governed by Intuit's privacy notice at https://www.intuit.com/privacy/.
- **Airtable, Inc.** — operator of the destination base you choose. Governed by Airtable's privacy notice at https://airtable.com/privacy.

We do not sell your personal information. We do not share it with advertisers, data brokers, marketing partners, or analytics providers. We do not use your data to train machine learning models, our own or anyone else's.

We may disclose data if compelled by valid legal process (subpoena, court order) or to protect rights, property, or safety. If this happens and we are legally permitted to notify you, we will.

## 10. International data transfers

Your QuickBooks data is held by Intuit in the United States and other regions Intuit operates in. The Service runs in us-east-1 (Northern Virginia, USA). Your Airtable data is stored in the region you select inside Airtable.

If you are located in the European Economic Area, the United Kingdom, or Switzerland, transfers of your personal data to the United States rely on appropriate safeguards including the European Commission's Standard Contractual Clauses, where applicable, between us and our subprocessors.

## 11. Your rights

**For everyone — operational rights:**

- **Disconnect at any time.** In QuickBooks, go to **Apps → My Apps → Alpha Accounts → Disconnect**. This revokes our OAuth grant. Your tokens are invalidated immediately at Intuit and deleted from our systems within 30 days.
- **Request deletion.** Email sandeep@alphalionlogistics.com from the email associated with your QuickBooks admin account. We will confirm receipt within 5 business days and complete deletion of any retained data within 30 days, unless we are legally required to keep specific records longer.

**For users covered by GDPR (EU / UK / EEA):**

You have the right to:
- **Access** the personal data we hold about you (Art. 15)
- **Rectification** of inaccurate data (Art. 16)
- **Erasure** ("right to be forgotten") (Art. 17)
- **Restriction** of processing (Art. 18)
- **Data portability** (Art. 20)
- **Object** to processing based on legitimate interests (Art. 21)
- **Withdraw consent** at any time (which you do operationally by disconnecting)
- **Lodge a complaint** with your supervisory authority

To exercise any of these rights, email sandeep@alphalionlogistics.com. We will respond within 30 days.

**For California residents (CCPA/CPRA):**

You have the right to know, delete, correct, and limit the use of sensitive personal information. **We do not sell or share personal information for cross-context behavioral advertising**, so the "right to opt out of sale or sharing" is satisfied by default — there is nothing to opt out of. You also have the right not to be discriminated against for exercising any of these rights.

## 12. Children's privacy

The Service is a B2B accounting integration. It is not directed at children under 16, we do not knowingly collect personal information from children, and we have no expectation that children will use the Service. If you believe a child has somehow provided personal information to us, contact sandeep@alphalionlogistics.com and we will delete it.

## 13. Cookies and tracking

The Service is server-side only and does not host an end-user web interface. **We do not set cookies, web beacons, pixels, or any other client-side tracking technology.** The OAuth consent screens you interact with are hosted by Intuit and Airtable, respectively, and any cookies set there are governed by their privacy notices, not ours.

## 14. Third-party services

The Service depends on the following third-party services. We list them here so you know the full data path:

| Service | Role | Privacy notice |
|---|---|---|
| Intuit QuickBooks Online API | Source of data and OAuth provider | https://www.intuit.com/privacy/ |
| Airtable API | Destination of synced data | https://airtable.com/privacy |

We do not use third-party analytics, advertising, error-tracking SaaS that ingests user data, or any other category of subprocessor beyond what is listed above.

## 15. Breach notification

If we become aware of a security incident that has resulted in unauthorized access to or disclosure of your personal data, we will notify affected Customers by email **within 72 hours of confirming the incident**, consistent with GDPR Art. 33–34 standards. Notification will describe, to the extent known: what happened, what data was involved, what we are doing in response, and what you can do to protect yourself.

## 16. Changes to this policy

We may update this Privacy Policy from time to time. When we do:

- We will update the **Effective date** at the top of this page.
- For **material changes** (changes that expand the categories of data collected, change who we share it with, or weaken your rights), we will email connected Customers at the email on file with at least 30 days' notice before the changes take effect.
- For non-material changes (typo fixes, clarifications), the updated version takes effect when posted.

A short changelog will be appended to the bottom of this page so you can see what changed and when.

## 17. How to contact us

For privacy questions, requests, or complaints:

- **Email:** sandeep@alphalionlogistics.com
- **Postal mail:** Alpha Accounts, [Add your registered address before publishing]

We aim to respond to all privacy inquiries within 5 business days, and to formal rights requests within 30 days as required by law.

---

## Changelog

| Date | Change |
|---|---|
| 2026-05-05 | Initial publication. |
