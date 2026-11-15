# Part 2 Privacy: Evidence Plan and PDPA Comparison

[Report](../README.md) · [Part 1 privacy section](../issues/privacy.md)

Working file for the privacy issue in Part 2. It records what we still need to test in the app, how each test will be recorded, and how ReMeal's published documents compare with the Personal Data Protection Act 2010 (PDPA) as amended in 2024.

## 1. Hands-on tests

Part 1 left four privacy questions untested (README § 3.2). Each test below uses a test account on one Android phone. For every step, take a screenshot and note the date, device and app version.

| # | Question | Steps | What to record | Status |
|---|---|---|---|---|
| T1 | Can a guest place an order? | Continue as guest → open a listing → add to cart → go to checkout. Stop before payment. | The exact screen where the app asks for sign-in, if it does, and what it asks for | Not started |
| T2 | Does the app work with location denied? | Clear app data → choose “Use Current Location” → tap “Don’t allow” on the Android prompt → try to browse and add to cart. Repeat with “Set From Map”. | Whether the app blocks, repeats the prompt, or falls back to the default location; whether a manual area or address can be entered | Not started |
| T3 | What consent options does the sign-up form offer? | Open the account-creation form → note every field and whether it is required → look for tick boxes, marketing opt-ins and links to the policies. | Required and optional fields; any consent control and whether it is pre-ticked; whether sign-up can finish without accepting marketing | Not started |
| T4 | Can choices be changed later? | In the account settings, look for marketing or notification preferences and a delete-account option. | Which controls exist in the app, and which need an email to ReMeal | Not started |

T4 is new. The Privacy Notice says withdrawal and deletion requests go by email, and the Malay version mentions app settings for marketing preferences, so the app itself needs checking.

We will not submit real identity documents or payment card details, and we will not place an order only to test privacy behaviour.

## 2. Document findings so far

Read on 12 November 2026 from the live Privacy Notice (last updated 9 June 2024) and Terms and Conditions (last updated 21 May 2024).

| Finding | Source | Why it matters |
|---|---|---|
| The Terms say an account is needed to use the Platform, and the word “guest” does not appear. The app offers guest access. | Terms § 2.1; Fig. A1 | The documents and the app disagree about who can use the service. |
| Consent is attached to providing data and to accessing the Platform. | Notice preamble; Terms §§ 1.0, 11.0 | No separate act of consent is described. |
| The Notice lists selfie images for identity checks, device identifiers such as IMEI, emergency contacts, and sharing with credit bureaus. | Notice §§ 1.A–1.C, 3.C | We saw no feature using these in the Part 1 walkthrough. To be checked again in T3. |
| Health information that a user volunteers, with allergies given as the example, is processed on “legitimate interests”. | Notice § 1.D | Health data is sensitive personal data under the PDPA. In-app messages are also collected (§ 1.B). |
| Withdrawal of consent and other requests go to a data protection officer by email. Account deletion is also by email. | Notice §§ 8, 10; Terms § 2.2 | Consent is given in the app, but withdrawn outside it. |
| Marketing can arrive by SMS, WhatsApp, push notification, call or email, with an unsubscribe link as the opt-out. | Notice § 2.F | Compare with what T3 and T4 show. |
| The Notice is published in English and Bahasa Malaysia. | Notice, both versions | Positive finding. |
| The Malay version appears to add details that the English version lacks, such as app settings for marketing preferences. | Notice § 2.F (Malay) | To confirm with a side-by-side screenshot before using. |
| No retention period is stated; data is kept as long as “necessary”. | Notice § 4 | Users cannot tell how long location or order history is kept. |

## 3. Comparison with the PDPA

The amendment provisions below were checked against Act A1727 and the commencement gazette, P.U. (B) 522. The wording of the principal Act (ss 6, 7, 38 and 40) and of the 2013 Regulations still needs checking against the 2026 reprint before it is quoted in the report.

| Provision | Requirement in brief | ReMeal's documents | Our reading |
|---|---|---|---|
| s 6, General Principle | Consent to processing; data should be needed for a lawful purpose and not excessive | Consent tied to use of the Platform; wide list of data categories | Open. Depends on T3. |
| s 7, Notice and Choice | Written notice of purposes, disclosures and how to limit processing, in the national and English languages | Bilingual notice; limiting processing is mostly by email | Language requirement appears met. Choice is weak. |
| s 38, Withdrawal of consent | A data subject may withdraw consent by written notice | Email to the data protection officer | Appears consistent with the Act, but not easy to use. |
| s 40, Sensitive personal data | Explicit consent for sensitive data such as health information | Volunteered health data processed on “legitimate interests” | Possible gap. Needs care: we are comparing texts, not giving legal advice. |
| s 12A, Data protection officer (in force 1 June 2025) | A data controller appoints a data protection officer and notifies the Commissioner | A data protection officer is mentioned, not named; contact by email | Cannot verify the appointment from outside. |
| s 12B, Breach notification (in force 1 June 2025) | Notify the Commissioner of a breach, and data subjects where significant harm is likely | Not mentioned in the Notice | The Act does not require the Notice to cover this. Noted only. |
| s 43A, Data portability (in force 1 June 2025) | A data subject may ask for data to be sent to another controller | A similar right is described in § 8 | Appears covered. |
| s 129, Transfers abroad (amended 1 April 2025) | Transfers allowed to places with similar law or adequate protection, among other conditions | Overseas transfer stated, no countries named | Cannot verify. |

## 4. Sources to add to the reference list

- Personal Data Protection Act 2010 (Malaysia), Act 709. https://www.pdp.gov.my/en/akta/pdp-act-2010-en/
- Personal Data Protection (Amendment) Act 2024 (Malaysia), Act A1727. https://www.pdp.gov.my/wp-content/uploads/2024/11/Act-A1727.pdf
- Personal Data Protection (Amendment) Act 2024: Appointment of Date of Coming into Operation, P.U. (B) 522 (Malaysia). https://www.pdp.gov.my/wp-content/uploads/2024/12/PENETAPAN-TARIKH-PERMULAAN-KUAT-KUASA.pdf
