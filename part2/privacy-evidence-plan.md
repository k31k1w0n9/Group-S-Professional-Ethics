# Part 2 Privacy: Evidence Plan and PDPA Comparison

[Report](../README.md) · [Part 1 privacy section](../issues/privacy.md)

Working file for the privacy issue in Part 2. It records what we still need to test in the app, how each test will be recorded, and how ReMeal's published documents compare with the Personal Data Protection Act 2010 (PDPA) as amended in 2024.

## 1. Hands-on tests

Part 1 left four privacy questions untested (README § 3.2). Each test below uses a test account on one Android phone. For every step, take a screenshot and note the date, device and app version.

| # | Question | Steps | What to record | Status |
|---|---|---|---|---|
| T1 | Can a guest place an order? | Continue as guest → open a listing → add to cart → go to checkout. Stop before payment. | The exact screen where the app asks for sign-in, if it does, and what it asks for | Done on web shop and app (1a, 1b) |
| T2 | Does the app work with location denied? | Clear app data → choose “Use Current Location” → tap “Don’t allow” on the Android prompt → try to browse and add to cart. Repeat with “Set From Map”. | Whether the app blocks, repeats the prompt, or falls back to the default location; whether a manual area or address can be entered | Done on web shop and app (1a, 1b) |
| T3 | What consent options does the sign-up form offer? | Open the account-creation form → note every field and whether it is required → look for tick boxes, marketing opt-ins and links to the policies. | Required and optional fields; any consent control and whether it is pre-ticked; whether sign-up can finish without accepting marketing | Done on web shop and app (1a, 1b) |
| T4 | Can choices be changed later? | In the account settings, look for marketing or notification preferences and a delete-account option. | Which controls exist in the app, and which need an email to ReMeal | Done in app, as guest and signed in (1b) |

T4 is new. The Privacy Notice says withdrawal and deletion requests go by email, and the Malay version mentions app settings for marketing preferences, so the app itself needs checking.

We will not submit real identity documents or payment card details, and we will not place an order only to test privacy behaviour.

## 1a. Web shop results (15 November 2026)

ReMeal also runs a public web shop at https://remeal.app/shop/stores. The tests below were run there in a desktop browser with no account and with the browser's location permission already denied. They do not replace the Android tests above, because the web shop and the app may behave differently. Screenshots still need to be captured for the appendix.

| Test | What happened on the web shop |
|---|---|
| T1 Guest ordering | A guest can browse stores, listings, prices and collection times. Pressing “Add to cart” redirects to the log-in page, and the Cart and Orders pages also redirect to log-in. A guest cannot build a cart or reach checkout. |
| T2 Location denied | With location permission denied, the shop still loaded. It showed “Kuala Lumpur” as the location and listed stores with distances. No location prompt or blocking message appeared. Pressing the location selector redirects to log-in (saved addresses), so a guest cannot change the default area. |
| T3 Sign-up form | The form asks for first name (required), last name, email (required), password (required) and an optional referral code, or sign-up with Google or Apple. It has no tick box, no marketing opt-in and no consent wording. The Terms and Privacy Policy are linked only in the page footer. No phone number is requested, although the Terms list a mobile number for registration (§ 2.1). The form was viewed only; no account was created. |
| T4 Settings | Not tested. It needs an account. |
| Cookies (new) | Before any log-in or consent, the shop set Google Analytics cookies (`_ga`) and Stripe cookies (`__stripe_mid`, `__stripe_sid`). No cookie banner or cookie choice was shown. The Privacy Notice covers cookies in § 6. |

## 1b. Android app results (16 November 2026)

Run on ReMeal 1.1.19 from Google Play, on an Android Studio emulator (Pixel 7a profile, Android 17), first as a guest with no ReMeal account, then signed in to a test account for T4 only. Screenshots are in `appendix/screenshots/part2-privacy/` (e01–e19 and e21–e24). An emulator is not a physical phone, and nothing was purchased.

| Test | What happened in the app | Screenshots |
|---|---|---|
| T1 Guest ordering | “Continue as Guest” opened the app. A guest could open a listing, add it to the cart and view the cart with a subtotal. “Proceed to Checkout” showed “Sorry! You are not logged in” with a “Login to Continue” button. A guest can build a cart but cannot order. | e01, e07–e10 |
| T2 Location denied | “Use Current Location” triggered Android’s prompt, with “Precise” pre-selected. After “Don’t allow”, the app asked for notification permission straight away. After that was also declined, the home screen opened at a default address in Kuala Lumpur City Centre and showed listings with distances. Android confirmed both permissions as not granted. The location selector then showed “Enable location access for a greater experience”, “Use Default Location” and “Set From Map”; the map let a guest pick any address without device location. A banner, “Enable notifications for best experience”, stayed on the home screen. | e02–e06, e18–e19 |
| T3 Sign-up form | Fields: first name, last name, email, password and an optional referral code, or “Sign up with Google”. There is no tick box and no marketing choice. The only consent wording is a line below the form: “By creating an account, you agree to our Terms & Conditions and Privacy Policy.” No phone number is requested. The form was viewed only; no account was created. | e11–e13 |
| T4 Settings (guest) | As a guest, the Account tab lists Profile, Saved Addresses, Notification Settings, Contact Support, Terms & Conditions and Privacy Policy. Notification Settings showed “You are not logged in”. | e15–e17 |
| T4 Settings (signed in) | Notification Settings has two switches, “New Inventory” and “Marketing Notifications”. Both were switched on when first opened. Profile shows name, email and phone (phone was empty) and has a “Delete Account” button, which was not pressed. Nothing was changed. The tester’s name and email are blacked out in e21, e22 and e24. | e21–e24 |
| Declared permissions | Location (fine and coarse), notifications, advertising ID and ad attribution, basic phone state, NFC, network access. | Read from the installed package |

The app and the web shop differ on guests: the app lets a guest fill a cart, while the web shop sends a guest to log-in at “Add to cart”.

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
