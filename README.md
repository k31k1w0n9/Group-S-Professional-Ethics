# ReMeal: Ethical Issues in a Surplus Food App

## Group Members

| Name | Student ID |
|---|---:|
| Wong Chuek Kei | 20602511 |
| Chai Chok Yuen | 20620830 |
| Tham Wing Lok | 20611657 |
| Moiz Israr Malik | 20705922 |
| Xinzhu Yang | 20700664 |

## 1. Introduction

[To be completed.]

## 2. System Overview and Selection Rationale

### 2.1 What ReMeal Does

ReMeal is a Malaysian app developed by ReMeal Sdn. Bhd. It connects cafés, bakeries, supermarkets, and restaurants with customers who want to buy surplus food at reduced prices. Users can pay through the app and, depending on the available option, collect their order, dine in, or use delivery. In December 2024, *Vulcan Post* reported that ReMeal had 16 active stores and around 1,800 user sign-ups. At that time, orders were pickup-only. ReMeal’s current website also lists dine-in and delivery options, which may vary by vendor.

### 2.2 Why We Chose ReMeal

ReMeal is a real app that is available to download, and users can investigate its features and policies. It is a small Malaysian platform rather than a global service. Our preliminary search found limited research focused specifically on ReMeal’s ethical issues. A NUS case study mentions ReMeal as part of a broader discussion of surplus-food platforms, but it is not an ethical review of the app.

ReMeal also has ethically relevant features. Its App Store privacy information, which is provided by the developer, lists data such as location and purchase history as information the app may collect. The app handles payments and refunds, and users rely on vendor listings to understand what food they are buying.

We chose ReMeal because it aims to reduce food waste and make food more affordable. This raised a question we found interesting: can a well-intentioned app still treat users unfairly through the way it is designed?

## 3. Investigation Method

### 3.1 How We Examined the App and Its Policies

For the privacy review, we read ReMeal’s Privacy Notice and Terms and checked the privacy information on the app-store listings. On 2 November 2026, we walked through the Android app’s sign-in screen, location setup, location permission prompt, and notification permission prompt. We saved screenshots of the app screens and relevant policy sections for the Appendix (Figures A1–A13).


### 3.2 Evidence Collected and Limitations

Our screenshots show what the app and policies displayed on 2 November 2026. The App Store and Google Play privacy information is supplied by the developer, so it is not an independent technical audit. We did not inspect network traffic, ReMeal’s servers, or how vendors and other service providers handle data.

For location, we followed one sequence: choosing “Set From Map” brought up the Android location prompt; backing out without choosing “Allow” or “Don’t allow” led to a screen with “Use Default Location”; tapping that opened the home screen. We did not explicitly deny location access, test whether the banner returns on later launches, establish how the default location was selected, or test whether browsing and ordering work from it. A separate notification-permission prompt appeared after the home screen; we did not assess its effects.

## 4. Related Literature

### 4.1 Privacy and Personal Data in Food Delivery Apps

Research on mobile-app privacy covers privacy policies, requirements, user perspectives, and detection of data leaks. Ebrahimi et al. (2021) mapped 59 software-engineering studies published between 2008 and 2018. Most focused on detecting privacy leaks, while fewer examined policies and users’ perspectives. Obar and Oeldorf-Hirsch (2020) found that 74% of 543 participants skipped the privacy policy when joining a fictitious social network. This result comes from one study of a different service; it does not show that ReMeal users behave the same way.

In a Malaysian legal analysis, Al Rezan et al. (2025) examined the terms and privacy policies of nine popular food-delivery apps and reported that the apps failed to meet the standards the authors developed. Nouwens et al. (2020) studied consent pop-ups on 680 UK websites, not food-delivery apps. Only 11.8% met the authors’ minimum GDPR-based criteria, and a small experiment with 40 participants found that leaving an opt-out button off the first page increased consent. These studies suggest that policy wording and interface design can affect users’ choices, but they do not establish that ReMeal has the same problems.

Acquisti et al. (2015) describe privacy choices as affected by uncertainty and context. Keßler and McKenzie (2018) argue that location information deserves particular attention because it can reveal more than a single place. These studies guide the questions we ask about ReMeal; our conclusions about the app are based on the walkthrough and policies described below.

### 4.2 Refunds and Consumer Protection

[To be completed.]

### 4.3 Food Descriptions, Allergens, and Food Safety

[To be completed.]

## 5. Ethical Issues Identified

### 5.1 Privacy and Personal Data

ReMeal’s Privacy Notice describes several ways it may collect personal data. Information users provide can include contact and identification details, social-media information, event submissions, and survey responses. During use of the app or website, the Notice says it may collect geolocation, feedback, transaction and payment-method information, app interactions and viewed content, device information and identifiers, and information entered in messages. It also describes receiving information from other sources, including business partners and public or government sources (ReMeal, 2024a, § 1; Appendix, Fig. A6).

The Notice says order details may be shared with the relevant vendor. It also says a user’s name and contact details may be shared for vendor loyalty or marketing activities, and that a user’s registered name and mobile number may be shared with people they chat with. It allows data to be shared with service providers and transferred overseas (ReMeal, 2024a, § 3; Appendix, Figs. A7 and A9). The Notice says it may retain data for as long as needed for its stated purposes (ReMeal, 2024a, § 4; Appendix, Fig. A9).

The Notice says ReMeal does not ask users to submit sensitive personal data, but gives allergy information volunteered to customer care as an example of information it may process. It says this is handled on the basis of legitimate interests and, where necessary, legal claims. This does not mean the app automatically collects users’ allergy information. Its privacy implications belong here; the effect of food-allergen information on ordering belongs under Section 5.4.

Our app walkthrough showed a sign-in screen with a “Continue as Guest” option (Appendix, Fig. A1). However, the Terms say users need to register an account to use the platform (ReMeal, 2024b, § 2.1; Appendix, Fig. A4). The screenshots do not show whether guest access is limited to browsing or allows users to order, so we treat this as a point needing further testing rather than proof of a contradiction.

The Terms say users are required to provide a location so the platform can display vendors in their area (ReMeal, 2024b, § 5.5; Appendix, Fig. A10). The app’s location screen says “Allow location access to find food closest to you” and offers “Use Current Location” and “Set From Map” (Appendix, Fig. A3). Choosing “Set From Map” still triggered the Android location-permission prompt (Appendix, Fig. A2). After we backed out without answering it, the screen showed “Use Default Location” and a banner saying “Enable location access for a greater experience” (Appendix, Fig. A12). Tapping “Use Default Location” opened the home screen without answering the location prompt. A separate notification-permission prompt then appeared (Appendix, Fig. A13).

This path shows that granting device-location access was avoidable for reaching the home screen. The wording is unclear, though: the Terms describe providing a location as required, while the app describes device-location access as helping users find nearby food or providing a “greater experience.” This may refer to different things—providing some location versus granting device access—so we describe it as unclear messaging, not proof of deception. We did not test whether location permission is needed for browsing or ordering, or whether the default location is fixed or selected another way.

The Google Play Data safety label says the app may collect personal information and device identifiers, may share app activity, app information and device identifiers, and that data “isn’t encrypted” (ReMeal, n.d.-b; Appendix, Fig. A8). The App Store label also lists data the developer says may be linked to users (Apple App Store, n.d.). These are developer-provided disclosures, not independent tests. In particular, the Google Play label does not identify which data the encryption statement refers to or whether it concerns data in transit or storage.

These practices could support nearby vendor listings, ordering, payments, and customer service, so their presence alone does not show misuse. They do raise questions about whether users understand the data collection and sharing, whether each data type is needed, and what control users have over optional uses. We found no evidence that ReMeal has misused or exposed personal data.

### 5.2 Refunds and Cancellations

[To be completed.]

### 5.3 Food Descriptions and Photos

[To be completed.]

### 5.4 Allergen and Food Safety Information

[To be completed.]

## 6. Ethical Analysis

### 6.1 Relevant ACM/IEEE Code Principles

Clause **3.12** asks software engineers to develop software and related documents that respect the privacy of people affected by the software. It applies to ReMeal’s data practices and the Privacy Notice that explains them.

Clause **3.13** says engineers should use accurate data collected by ethical and lawful means, and use it only in properly authorised ways. Clause **1.03** says software should be approved only when there is a well-founded belief that it does not diminish users’ privacy.

Clause **1.06** requires fair, non-deceptive statements about software and related documents. The Terms describe providing a location as required, while the app describes location access as offering a “greater experience” and lets users proceed to the home screen with a default location. We report this as unclear wording. We have no evidence of deception and do not claim a violation of clause 1.06.

Clauses **2.07** and **2.09** guide engineers who identify significant social concerns. They should document and raise concerns with the employer or client. If a higher ethical concern is compromised, clause 2.09 says to inform the employer or another appropriate authority (IEEE-CS/ACM Joint Task Force, 1999).

### 6.2 Applying Ethical Theories

Under **utilitarianism**, we weigh the benefits of location data—such as showing nearby vendors—against possible harms such as unwanted sharing or exposure of personal information. The observed default-location path let us reach the home screen without answering the location prompt, but we did not test whether it supports browsing or ordering. The map option is not yet evidence of a less intrusive alternative because it still triggered the location prompt.

Under **Kantian deontology**, users should be treated as people who can make informed choices, not just as a means to improve the service. ReMeal should explain clearly whether it needs a location, device-location permission, or both, and what users can do if they decline permission. Our screenshots show some choice, but do not establish what users can do at checkout or how optional data uses are controlled.

### 6.3 Where the Code May Not Fully Address an Issue

The Code sets a general duty to respect privacy, but it does not specify which data an app needs or whether “providing a location” must mean granting device-location permission. It also does not settle how to balance privacy against convenience or fraud prevention. Those questions need evidence about ReMeal’s actual data flows and ethical judgement about the trade-offs. Decisions about data collection may sit with product owners or management; the Code guides engineers to document and raise concerns, but does not itself settle the company’s policy.


## 7. Conclusion

[To be completed.]

## 8. Plan for Part 2

In Part 2, we will examine more vendors and listings, compare ReMeal’s policies with Malaysia’s Personal Data Protection Act 2010 as amended, apply both ethical theories to each issue, and propose practical recommendations for the developers.

## References

- Acquisti, A., Brandimarte, L., & Loewenstein, G. (2015). Privacy and human behavior in the age of information. *Science, 347*(6221), 509–514. https://doi.org/10.1126/science.aaa1465
- Al Rezan, M. I., Hosain, M. M., & Karim, M. E. (2025). User acceptance of terms and conditions and privacy policy: A legal analysis of the position of food delivery mobile apps in the Malaysian context. *UUM Journal of Legal Studies, 16*(1), 130–149. https://doi.org/10.32890/uumjls2025.16.1.8
- Apple App Store. (n.d.). *ReMeal – Rescue Surplus Food*. [App Store listing](https://apps.apple.com/my/app/remeal-rescue-surplus-food/id6499340832)
- Ebrahimi, F., Tushev, M., & Mahmoud, A. (2021). Mobile app privacy in software engineering research: A systematic mapping study. *Information and Software Technology, 133*, 106466. https://doi.org/10.1016/j.infsof.2020.106466
- IEEE-CS/ACM Joint Task Force. (1999). *Software Engineering Code of Ethics and Professional Practice*. https://www.computer.org/education/code-of-ethics
- Keßler, C., & McKenzie, G. (2018). A geoprivacy manifesto. *Transactions in GIS, 22*(1), 3–19. https://doi.org/10.1111/tgis.12305
- Nouwens, M., Liccardi, I., Veale, M., Karger, D., & Kagal, L. (2020). Dark patterns after the GDPR: Scraping consent pop-ups and demonstrating their influence. In *Proceedings of the 2020 CHI Conference on Human Factors in Computing Systems*. ACM. https://doi.org/10.1145/3313831.3376321
- Obar, J. A., & Oeldorf-Hirsch, A. (2020). The biggest lie on the internet: Ignoring the privacy policies and terms of service policies of social networking services. *Information, Communication & Society, 23*(1), 128–147. https://doi.org/10.1080/1369118X.2018.1486870
- ReMeal. (n.d.-a). *ReMeal*. https://remeal.app/
- ReMeal. (n.d.-b). *ReMeal – Rescue Surplus Food* [Google Play listing]. https://play.google.com/store/apps/details?id=app.remeal.user
- ReMeal. (2024a). *Privacy Notice*. Last updated 9 June 2024. https://remeal.app/privacy-policy
- ReMeal. (2024b). *Terms and Conditions*. Last updated 21 May 2024. https://remeal.app/terms-and-conditions

## Appendix: Privacy Evidence

Screenshots from the ReMeal Android app and policy pages, captured on 2 November 2026.

| Figure | Evidence | Screenshot |
|---|---|---|
| A1 | Sign-in screen showing “Continue as Guest” | [01-app-sign-in-guest-mode.png](output/playwright/01-app-sign-in-guest-mode.png) |
| A2 | Android location-permission choices | [02-app-location-permission.png](output/playwright/02-app-location-permission.png) |
| A3 | Location screen offering current location or map selection | [03-app-set-location-options.png](output/playwright/03-app-set-location-options.png) |
| A4 | Terms on registration and account deletion | [05-terms-registration-account-deletion.png](output/playwright/05-terms-registration-account-deletion.png) |
| A5 | Terms on acceptance and data processing | [06-terms-consent-background.png](output/playwright/06-terms-consent-background.png) |
| A6 | Privacy Notice data-collection categories | [13-privacy-data-collection-methods.jpg.jpeg](output/playwright/13-privacy-data-collection-methods.jpeg) |
| A7 | Privacy Notice data disclosure and sharing | [08-privacy-data-disclosure.png](output/playwright/08-privacy-data-disclosure.png) |
| A8 | Google Play Data safety label | [09-google-play-data-safety.png](output/playwright/09-google-play-data-safety.png) |
| A9 | Privacy Notice retention and international transfers | [07-privacy-retention-international-transfers.png](output/playwright/07-privacy-retention-international-transfers.png) |
| A10 | Terms on allergens and location | [10-terms-allergens-location.png](output/playwright/10-terms-allergens-location.png) |
| A11 | Privacy Notice overview | [12-privacy-notice-overview.png](output/playwright/12-privacy-notice-overview.png) |
| A12 | “Use Default Location” screen and location-access banner | [12-app-default-location-banner.png](output/playwright/12-app-default-location-banner.png) |
| A13 | Separate Android notification-permission prompt after opening the home screen | [13-app-notification-permission.png](output/playwright/13-app-notification-permission.png) |
