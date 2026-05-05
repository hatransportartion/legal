---
title: Terms of Service
layout: default
permalink: /terms/
---

# End-User License Agreement & Terms of Service

**Effective date:** 2026-05-05
**Publisher:** Alpha Accounts
**Governing law:** India
**Contact:** sandeep@alphalionlogistics.com

---

## Plain-English summary

Alpha Accounts is a behind-the-scenes integration that copies selected data from your QuickBooks Online company into an Airtable base you control. By installing the app or connecting your QuickBooks company, you agree to these terms. **You keep ownership of your data. You're responsible for making sure you have the right to connect the QuickBooks company you're connecting and for the security of your Airtable base. The Service is provided "as is" — verify anything important against QuickBooks itself. Our liability is capped, and disputes are resolved by arbitration in India. You can leave anytime by disconnecting in QuickBooks → Apps → Disconnect.**

---

## 1. Acceptance of Terms

These End-User License Agreement and Terms of Service (together, the "Terms") are a legal agreement between you (or the entity you represent, "Customer" or "you") and Alpha Accounts ("Publisher," "we," "us," or "our").

**By installing Alpha Accounts (the "Service"), connecting a QuickBooks Online company to it, or otherwise using the Service, you accept these Terms and agree to be bound by them.** If you are accepting on behalf of a company or other legal entity, you represent that you have the authority to bind that entity. If you do not agree, do not install or use the Service.

## 2. Definitions

For clarity, the following capitalized terms have the meanings below:

- **"Service"** means Alpha Accounts, the server-side Node.js integration that authenticates to QuickBooks Online via OAuth 2.0 and mirrors selected account-statement data into an Airtable base, including any updates, documentation, and related materials we provide.
- **"Customer"** means the legal entity (or individual, if there is no entity) that installs or operates the Service.
- **"Authorized User"** means an individual employee, contractor, or agent of Customer whom Customer permits to install, configure, or operate the Service.
- **"Customer Data"** means any data accessed, processed, transmitted, or written by the Service on Customer's behalf, including data drawn from the Connected Account and data written into the Output Destination.
- **"Connected Account"** means the QuickBooks Online company that Customer authorizes the Service to access via Intuit's OAuth 2.0 flow.
- **"Output Destination"** means the Airtable base and table that Customer designates to receive synced records.
- **"Intuit"** means Intuit Inc. and its affiliates that operate QuickBooks Online.
- **"Airtable"** means Formagrid, Inc. (d/b/a Airtable) and its affiliates.

## 3. License Grant

Subject to Customer's compliance with these Terms, Publisher grants Customer a **non-exclusive, non-transferable, non-sublicensable, revocable** license to install and use the Service for Customer's **internal business operations** during the term of this agreement.

This license does not transfer any ownership in the Service. All right, title, and interest in the Service — including all source code, designs, documentation, trademarks, and improvements — remain the exclusive property of Publisher.

## 4. Restrictions

Customer will not, and will not permit any Authorized User or third party to:

- **Reverse engineer, decompile, or disassemble** the Service or attempt to derive its source code, except to the extent this restriction is prohibited by applicable law.
- **Resell, rent, lease, sublicense, or commercially redistribute** the Service or access to it.
- **Use the Service to access, mirror, or process data from a QuickBooks company that Customer does not own or does not have written authorization to access.** This is a critical condition; violations may also constitute violations of Intuit's terms and applicable computer-misuse laws.
- **Circumvent or attempt to circumvent** any rate limits, quotas, authentication mechanisms, or other technical restrictions.
- **Engage in automated abuse**, including but not limited to denial-of-service activity, scraping at rates that interfere with Service operation, or running the Service in a way designed to exhaust Intuit or Airtable API quotas in bad faith.
- **Remove, alter, or obscure** any copyright, trademark, or other proprietary notices.
- **Use the Service in a manner that violates** Intuit's Developer Terms of Service, the QuickBooks Online subscription terms, Airtable's Terms of Service, or any applicable law.
- **Interfere with or disrupt** the integrity or performance of the Service.

## 5. Customer Responsibilities

Customer is solely responsible for the following, and Publisher has no obligation or liability with respect to them:

- **Authority to connect.** Customer represents and warrants that Customer **owns, or has obtained explicit written authorization from the owner of, the Connected Account** before authorizing the Service to access it. If Customer is an accountant, bookkeeper, or service provider acting on behalf of a third-party business, Customer must have engagement-letter-level authorization to do so.
- **Airtable security.** Customer is responsible for the configuration, access controls, sharing settings, and overall security posture of the Output Destination. Publisher has no visibility into or control over who Customer grants access to the Airtable base.
- **Legal and recordkeeping obligations.** Customer is responsible for compliance with **all legal obligations applicable to the data being synced**, including tax recordkeeping requirements, audit trail integrity, retention periods, and any requirements specific to Customer's industry or jurisdiction.
- **Data accuracy.** Customer is responsible for verifying that data written into the Output Destination matches the source of truth in the Connected Account. The Service performs a best-effort mirror; it does not guarantee bit-for-bit accuracy.
- **Authorized Users.** Customer is responsible for the acts and omissions of its Authorized Users, who are bound by these Terms to the same extent as Customer.

## 6. Customer Data Ownership

**Customer retains all right, title, and interest in and to Customer Data**, including data residing in the Connected Account and data written into the Output Destination. Publisher claims **no ownership** of Customer Data.

Customer grants Publisher a limited, non-exclusive, royalty-free license to access, process, transmit, and store Customer Data **solely for the purpose of operating the Service for Customer**. Publisher will not use Customer Data to train machine learning models, sell or share Customer Data with third parties (other than Intuit and Airtable as required to operate the Service), or use Customer Data for any purpose unrelated to operating the Service.

Publisher's handling of personal data within Customer Data is governed by the [Privacy Policy](https://alphalionlogistics.com/privacy) (incorporated into these Terms by reference — see Section 16).

## 7. Intuit & Airtable Terms

The Service relies on third-party platforms operated by Intuit and Airtable. **Customer's use of the Service is also subject to**:

- **Intuit Developer Terms of Service** — https://developer.intuit.com/app/developer/qbo/docs/legal
- **Intuit's QuickBooks Online subscription terms** that apply to Customer's QuickBooks subscription
- **Airtable Terms of Service** — https://airtable.com/terms

If there is a direct conflict between these Terms and the terms of Intuit or Airtable as they apply to Customer's use of those platforms, the third-party terms prevail with respect to that platform. These Terms continue to govern Customer's relationship with Publisher.

Publisher is not affiliated with, endorsed by, or sponsored by Intuit or Airtable. The Service is an independent integration.

## 8. Service Availability & Modifications

We provide the Service on a **best-effort basis with no service-level commitment** unless a separate written agreement specifies otherwise. The Service depends on third-party APIs (Intuit, Airtable) whose availability is outside Publisher's control. Outages, rate limits, scheduled maintenance, and upstream errors will affect sync timeliness from time to time.

We may **modify, add to, or discontinue features** of the Service. For changes that materially reduce functionality Customer is actively using, we will provide reasonable advance notice — typically at least 30 days — by email to Customer's primary contact, where feasible.

## 9. Fees & Payment

The Service is provided **free of charge** at this time. Publisher reserves the right to introduce fees in the future. If Publisher does so, Publisher will provide Customer with at least **30 days' written notice** by email before fees take effect, and Customer may disconnect before the fees apply at no charge.

Late payments may accrue interest at the lesser of 1.5% per month or the maximum rate permitted by law. Publisher may suspend the Service for non-payment after providing written notice and a reasonable cure period.

## 10. Term & Termination

**Term.** These Terms begin on the date Customer first accepts them (per Section 1) and continue until terminated as described below.

**Termination by Customer.** Customer may terminate at any time by **disconnecting the Service in QuickBooks → Apps → My Apps → Alpha Accounts → Disconnect**. Customer may also terminate by emailing sandeep@alphalionlogistics.com from a verifiable Customer address.

**Termination by Publisher.** Publisher may terminate or suspend the Service:
- For Customer's material breach of these Terms (including any restriction in Section 4), with at least 14 days' notice and an opportunity to cure where the breach is curable;
- Immediately, if continued provision of the Service would, in Publisher's reasonable judgment, expose Publisher to legal liability or violate the terms of Intuit or Airtable;
- For convenience, with at least 30 days' written notice.

**Effects of termination.**
- The Service stops syncing data immediately.
- **OAuth tokens are deleted from Publisher's systems within 30 days** of termination, typically much sooner.
- Data already written into the Output Destination **remains under Customer's control**; Publisher does not delete it.
- Any fees accrued before termination remain due.

**Surviving sections.** The following sections survive termination: 4 (Restrictions), 6 (Customer Data Ownership), 11 (Disclaimer of Warranties), 12 (Limitation of Liability), 13 (Indemnification), 15 (Confidentiality), 18 (Governing Law & Dispute Resolution), 19 (General), and any payment obligations accrued before termination.

## 11. Disclaimer of Warranties

**THE SERVICE IS PROVIDED "AS IS" AND "AS AVAILABLE," WITH ALL FAULTS AND WITHOUT WARRANTY OF ANY KIND.** To the maximum extent permitted by applicable law, Publisher disclaims all warranties, whether express, implied, statutory, or otherwise, including without limitation:

- Implied warranties of **merchantability**, **fitness for a particular purpose**, **non-infringement**, **title**, and **quiet enjoyment**;
- Warranties arising from course of dealing, course of performance, or trade usage;
- Warranties that the Service will be **uninterrupted, error-free, secure, or free of harmful components**;
- Warranties that data synced to the Output Destination will be **accurate, complete, current, or in the same state as the source data in the Connected Account**.

**Customer acknowledges that the Connected Account in QuickBooks Online is the source of truth for Customer's accounting data and that Customer is responsible for verifying any data in the Output Destination against the Connected Account before relying on it for tax, audit, financial, or legal purposes.**

Some jurisdictions do not allow the exclusion of certain warranties; in those jurisdictions, the exclusions above apply to the maximum extent permitted.

## 12. Limitation of Liability

**TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW:**

**(a) Cap on aggregate liability.** Publisher's total aggregate liability arising out of or related to these Terms or the Service, regardless of the form of action (whether contract, tort, statute, or otherwise), is limited to the **greater of (i) the amount of fees Customer paid Publisher for the Service in the twelve (12) months immediately preceding the event giving rise to the claim, or (ii) one hundred U.S. dollars (USD $100)**.

**(b) Excluded damages.** Under no circumstances will Publisher be liable for any **indirect, incidental, consequential, special, exemplary, or punitive damages**, or for **lost profits, lost revenue, lost data, loss of goodwill, business interruption, or cost of substitute services**, even if Publisher has been advised of the possibility of such damages.

**(c) Basis of the bargain.** Customer acknowledges that the limitations in this Section 12 are an essential basis of the bargain between the parties, that the fees (if any) charged for the Service reflect those limitations, and that Publisher would not provide the Service without these limitations.

Some jurisdictions do not allow the limitation or exclusion of certain damages; in those jurisdictions, Publisher's liability is limited to the maximum extent permitted by law.

## 13. Indemnification

Customer will defend, indemnify, and hold harmless Publisher and its officers, directors, employees, agents, and affiliates from and against any third-party claims, damages, losses, liabilities, judgments, settlements, and reasonable attorneys' fees and costs arising out of or related to:

- Customer's **misuse of the Service**;
- Customer's **unauthorized access to a QuickBooks company** or use of the Service to access a Connected Account Customer did not own or have authorization to access;
- Customer's **violation of these Terms** or of any applicable law;
- Customer's **violation of any third party's rights**, including intellectual property or privacy rights, in connection with Customer's use of the Service;
- The **content of Customer Data**, including any claim that Customer Data infringes a third party's rights or violates applicable law.

Publisher will give Customer prompt notice of any claim subject to indemnification, allow Customer to control the defense and settlement (provided no settlement may impose obligations on Publisher without Publisher's prior written consent), and reasonably cooperate at Customer's expense.

## 14. Compliance with Laws

Customer warrants that Customer's use of the Service will comply with all applicable laws and regulations, including:

- **Data protection laws** such as the EU/UK General Data Protection Regulation (GDPR), the California Consumer Privacy Act / California Privacy Rights Act (CCPA/CPRA), and any other privacy law applicable to Customer Data;
- **Tax recordkeeping and audit-trail laws** applicable to the financial records Customer is mirroring;
- **Export controls and sanctions laws**, including those of the United States. Customer represents that Customer is not located in, organized under the laws of, or ordinarily resident in any country or region subject to comprehensive U.S. sanctions, and is not on any U.S. government denied-party list.

If Customer is acting as a "data processor" under GDPR with respect to data flowing through the Service, Customer is responsible for ensuring an appropriate processing relationship with the relevant data controllers.

## 15. Confidentiality

In the course of using the Service, each party may receive information from the other that is marked confidential or that a reasonable person would understand to be confidential ("Confidential Information"). Each party agrees to:

- Use the other party's Confidential Information **only as necessary to perform under these Terms**;
- Protect it with **at least the same degree of care** the party uses to protect its own confidential information of similar sensitivity, and in no event less than reasonable care;
- Not disclose it to third parties except to employees, contractors, and advisors who have a need to know and are bound by confidentiality obligations at least as protective as these.

These obligations do not apply to information that is or becomes publicly known through no fault of the receiving party, was independently developed without use of the disclosing party's Confidential Information, or is required to be disclosed by law (in which case the receiving party will give prompt notice where legally permitted).

Customer Data is treated as Customer's Confidential Information and is also governed by the Privacy Policy.

## 16. Privacy

Publisher's collection, use, and disclosure of personal information in connection with the Service is governed by Publisher's Privacy Policy, available at [https://alphalionlogistics.com/privacy], which is **incorporated into these Terms by reference**. By using the Service, Customer acknowledges that Customer has reviewed the Privacy Policy.

## 17. Modifications to Terms

We may update these Terms from time to time. When we make changes:

- The **Effective date** at the top of this document will be updated.
- For **material changes** — for example, changes to fees, liability, dispute resolution, or restrictions on use — we will **notify Customer's primary contact by email at least 30 days before the changes take effect** and post the updated Terms at [https://alphalionlogistics.com/terms].
- For non-material changes (typo corrections, clarifications), the updated Terms take effect when posted.

If Customer does not agree to a material change, Customer's sole remedy is to terminate by disconnecting the Service before the change takes effect. Continued use after the effective date of a change constitutes acceptance.

## 18. Governing Law & Dispute Resolution

**Governing law.** These Terms are governed by the laws of India, without regard to its conflict-of-laws principles. The United Nations Convention on Contracts for the International Sale of Goods does not apply.

**Binding arbitration.** Any dispute, claim, or controversy arising out of or relating to these Terms or the Service that cannot be resolved through good-faith informal negotiation will be resolved by **binding arbitration administered by the Indian Council of Arbitration (ICA) under its Rules of Arbitration of the Indian Council of Arbitration, read with the Arbitration and Conciliation Act, 1996** then in effect. Arbitration will be conducted in New Delhi, India, by a single arbitrator. Judgment on the award may be entered in any court of competent jurisdiction.

**Carve-out for injunctive relief.** Notwithstanding the arbitration clause, **either party may seek injunctive or other equitable relief in a court of competent jurisdiction for actual or threatened infringement, misappropriation, or violation of intellectual property rights or confidentiality obligations.**

**Class action waiver.** **The parties agree that any arbitration or court proceeding will be conducted only on an individual basis and not as a class, consolidated, or representative action.** If a court determines this class action waiver is unenforceable in a particular dispute, the arbitration agreement is severable from these Terms with respect to that dispute, and that dispute will be resolved in court — but the waiver remains enforceable for all other disputes.

**Opt-out (where required).** If applicable law gives Customer a right to opt out of arbitration, Customer may do so by emailing sandeep@alphalionlogistics.com within 30 days of first accepting these Terms with the subject line "Arbitration Opt-Out."

## 19. General

**Entire agreement.** These Terms, together with the Privacy Policy and any order form or written agreement signed by both parties, constitute the entire agreement between the parties regarding the Service and supersede all prior or contemporaneous agreements on the same subject.

**Severability.** If any provision of these Terms is held unenforceable, the remaining provisions remain in full force and effect, and the unenforceable provision will be modified to the minimum extent necessary to make it enforceable while preserving its intent.

**No waiver.** A party's failure to enforce a provision is not a waiver of its right to do so later.

**Assignment.** Customer may not assign these Terms or any rights under them without Publisher's prior written consent, except that either party may assign these Terms in connection with a **merger, acquisition, reorganization, or sale of substantially all of its assets** without the other party's consent. Any prohibited assignment is void.

**Force majeure.** Neither party is liable for failure or delay caused by events beyond its reasonable control, including acts of God, natural disasters, war, terrorism, civil unrest, labor disruptions, internet or utility outages, governmental actions, or failures of third-party services on which the Service depends (such as Intuit or Airtable).

**Notices.** Notices to Publisher must be sent to sandeep@alphalionlogistics.com and, for legal notices, also by mail to the address in Section 20. Notices to Customer will be sent to the email associated with Customer's account or to the contact email Customer provides.

**Independent contractors.** The parties are independent contractors. These Terms do not create a partnership, joint venture, agency, or employment relationship.

**Headings.** Section headings are for convenience only and do not affect interpretation.

## 20. Contact

**Alpha Accounts**
[Add your registered address before publishing]
Delhi, India

- **General & support:** sandeep@alphalionlogistics.com
- **Privacy:** sandeep@alphalionlogistics.com
- **Legal notices:** sandeep@alphalionlogistics.com
- **Website:** https://alphalionlogistics.com

---

*By installing or connecting Alpha Accounts, you confirm that you have read, understood, and agreed to these Terms.*
