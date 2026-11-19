# Part 2: Privacy and Personal Data

[Report](../README.md) · [Part 1 privacy section](../issues/privacy.md) · [Evidence plan and test results](privacy-evidence-plan.md)

## SE Code Analysis: Privacy

We re-read ReMeal’s Privacy Notice and Terms on 12 November 2026, tested the web shop on 15 November and the Android app (version 1.1.19) on 16 November. Screenshots e01–e19 and e21–e24 are in `appendix/screenshots/part2-privacy/`.

### Clauses 3.12 and 1.06: documents that match the software — does not meet

Clause 3.12 covers software “and related documents”, and clause 1.06 asks for statements about software that are fair and not deceptive (IEEE-CS/ACM Joint Task Force, 1999). ReMeal’s documents do not describe the app accurately, in either direction.

They understate it in three places. The Terms say an account is needed to use the Platform and never mention guests (ReMeal, 2024b, § 2.1), yet in the app a guest can browse and fill a cart, and is stopped only at checkout (e07–e10). The Terms say accounts are deleted by email (§ 2.2), yet the Profile screen has a “Delete Account” button (e24). They also list a phone number for registration, which neither sign-up form requests (e12–e13).

The Notice overstates it. It lists selfie images, device identifiers such as IMEI, emergency contacts and sharing with credit bureaus (ReMeal, 2024a, §§ 1.A–1.C, 3.C), none of which matched a feature we saw. We found no sign this is deliberate, so we treat it as inaccurate documentation, not deception.

### Clause 3.13: properly authorised data use — partly meets

Clause 3.13 requires data to be used only “in ways properly authorized”. ReMeal treats using the Platform as consent (ReMeal, 2024b, § 1.0). The app’s sign-up form has no tick box, only a line saying that creating an account means agreeing to both documents (e13). The web shop’s form has no consent wording, and the shop set analytics cookies before any choice was offered.

Marketing shows the weakness most clearly. In our test account, “Marketing Notifications” was already switched on when we first opened the settings (e23). The PDPA requires consent for processing (Personal Data Protection Act 2010, s 6(1)) and requires a “clear and readily accessible means” to exercise choice (s 7(3)). A switch that starts on, inside the Account tab, treats silence as agreement.

Health data needs separate care. The Notice processes volunteered allergy details on “legitimate interests” (§ 1.D; Fig. A6), but section 40 allows sensitive data only on listed conditions, mainly explicit consent. Legitimate interests is not one of them, although defending legal rights, which the Notice also cites, is. Because the Terms send customers to vendors for allergen information (§ 5.3), the safety advice itself may lead users to share health data in chat.

### Clause 1.03: software that does not diminish privacy — largely meets

ReMeal handles location well. After we refused location access, the app opened at a default Kuala Lumpur address, and “Set From Map” let us choose any area without device access (e04–e06, e19). This meets the Terms’ need for a location (§ 5.5) with less data. Two details count against it: because the app requests precise location, Android pre-selected “Precise” (e03), and the app asked for notifications immediately after the refusal and kept a banner urging users to enable them (e05–e06).

### Clause 6.06 and where the Code stops

Clause 6.06 asks engineers to obey the law, and on paper ReMeal may do so. Its Notice is bilingual as section 7(3) requires. Withdrawal by email fits section 38, which allows withdrawal “by notice in writing”, and users can stop direct marketing under section 43.

This is where the Code is insufficient. Default-on marketing can be lawful and still treat silence as consent, and the Code does not say whether a privacy choice should start on or off. That decision also belongs to product managers rather than engineers. For Section 6, utilitarianism can weigh promotions that may support vendors’ income against unwanted messages, while Kantian ethics asks whether consent assumed from inaction respects users’ autonomy.

Across these clauses, we found no evidence that personal data was misused.

## Critical Reflection

Testing corrected our Part 1 view. Part 1 gave location the most attention, but the app already offers the choice we planned to recommend; the sign-up and marketing defaults proved weaker. Our privacy recommendation should move from location to consent defaults.

We also learnt not to treat policies as descriptions of the app: a review based only on documents would have been unfair to ReMeal on guest access and deletion, and too generous on data collection.

Our evidence has limits. We tested an emulator and a desktop browser, not a physical phone, and could not see what the app sends or stores. We did not press “Delete Account”, so deletion itself is untested. Our PDPA comparison sets ReMeal’s wording beside the Act; it is not a legal finding.

Our method had a cost. Testing the settings meant giving ReMeal a name and email, so the review handed data to the system it assessed. Because we went looking for problems, we also recorded what ReMeal does well: guest browsing, working without device location and a bilingual Notice.

## References

- IEEE-CS/ACM Joint Task Force. (1999). *Software Engineering Code of Ethics and Professional Practice*. https://www.computer.org/education/code-of-ethics
- Personal Data Protection Act 2010 (Malaysia), Act 709 (Reprint as at 15 September 2026). https://www.pdp.gov.my/wp-content/uploads/2026/10/Akta-709-cetakan-semula-2026-BI.pdf
- ReMeal. (2024a). *Privacy Notice*. Last updated 9 June 2024. https://remeal.app/privacy-policy
- ReMeal. (2024b). *Terms and Conditions*. Last updated 21 May 2024. https://remeal.app/terms-and-conditions
