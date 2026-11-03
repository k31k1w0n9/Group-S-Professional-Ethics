# ReMeal: Ethical Issues in a Surplus Food App

## Group Members

| Name | Student ID |
|---|---:|
| Wong Chuek Kei | 20602511 |
| Chai Chok Yuen | 20720830 |
| Tham Wing Lok | 20611657 |
| Moiz Israr Malik | 20705922 |
| Xinzhu Yang | 20700664 |

## Report Map

| Sections | File |
|---|---|
| 1–3, 7–8, References | This README |
| 4.1/5.1 | [Privacy](issues/privacy.md) |
| 4.2/5.2 | [Refunds](issues/refunds.md) |
| 4.3/5.3/5.4 | [Food and allergens](issues/food-listings-and-allergens.md) |
| 6 | [Ethics](ethical-analysis.md) |
| Appendix | [Screenshots](appendix/screenshot-evidence.md) |

## 1. Introduction

This proposal sets up our ethical review of ReMeal, a Malaysian app that sells surplus food from local vendors at reduced prices. ReMeal has a worthwhile aim: less food waste and cheaper meals. We ask whether an app with a good purpose can still treat its users unfairly through its design and policies. Section 2 explains our choice of system, and Section 3 describes how we are investigating it. Section 4 reviews related research. Section 5 reports four issues: privacy, refunds and cancellations, food descriptions, and allergen information. Section 6 proposes our ethical framework, and Section 8 sets out our plan for Part 2.

## 2. System Overview and Selection Rationale

### 2.1 What ReMeal Does

ReMeal is a Malaysian app developed by ReMeal Sdn. Bhd. It connects cafés, bakeries, supermarkets, and restaurants with customers who want to buy surplus food at reduced prices. Users can pay through the app and, depending on the available option, collect their order, dine in, or use delivery. In December 2024, *Vulcan Post* reported that ReMeal had 16 active stores and 1,800 user sign-ups, and described a model in which users collected food from vendors rather than receiving deliveries (Kasinathan, 2024). ReMeal’s current website also lists dine-in and delivery options, which may vary by vendor (ReMeal, n.d.-a).

### 2.2 Why We Chose ReMeal

ReMeal is a real app that is available to download, and users can investigate its features and policies. It is a small Malaysian platform rather than a global service. Our preliminary searches found press coverage and ReMeal’s own pages, but no academic studies of the app.

ReMeal also has ethically relevant features. Its App Store privacy information, which is provided by the developer, lists data such as location and purchase history as information the app may collect. The app handles payments and refunds, and users rely on vendor listings to understand what food they are buying.

We chose ReMeal because it aims to reduce food waste and make food more affordable. This raised a question we found interesting: can a well-intentioned app still treat users unfairly through the way it is designed? Surplus food also differs from ordinary food delivery. What is available depends on what vendors have left, so customers rely heavily on listings to know what they are buying. Responsibility is shared between ReMeal and independent vendors, which may make it unclear who answers for a refund, a misleading description or a missing allergen warning. The food-app research we found mainly concerns delivery platforms (e.g. Al Rezan et al., 2025), so a small surplus-food app lets us test whether their known problems appear in a different business model.

## 3. Investigation Method

### 3.1 Investigation Plan

Each issue has one owner and uses at least one first-hand method alongside reading the policies:

| Issue | Methods |
|---|---|
| Privacy and data | Privacy Notice and Terms; Android permission audit; app-store data-safety labels |
| Refunds and cancellations | Terms on order acceptance, cancellation and refunds; walkthrough of the order flow up to payment |
| Food descriptions and photos | Structured review of a sample of listings against a fixed checklist (photo, contents, quantity, price, collection time, vendor) |
| Allergens and food safety | Terms on allergens; the same listing sample checked for ingredient and allergen details |

Across all issues, we check the walkthrough for dark patterns and code public app-store reviews by theme. We follow three evidence rules. First, every screenshot is dated and numbered in the Appendix. Second, we treat developer-provided disclosures as claims, not verified facts. Third, we do not call a listing inaccurate unless we can verify it.

### 3.2 How We Examined the App and Its Policies

For the privacy review, we read ReMeal’s Privacy Notice and Terms and checked the privacy information on the app-store listings. On 2 November 2026, we walked through the Android app’s sign-in screen, location setup, location permission prompt, and notification permission prompt. We saved screenshots of the app screens and relevant policy sections for the Appendix (Figures A1–A17).


### 3.3 Evidence Collected and Limitations

Our app and policy screenshots show what was displayed on 2 November 2026; the App Store summary was captured on 3 November. App-store privacy information is supplied by the developer, so it is not an independent technical audit. We did not inspect network traffic, ReMeal’s servers, or how vendors and other service providers handle data.

For location, we followed one sequence: choosing “Set From Map” brought up the Android location prompt; backing out without choosing “Allow” or “Don’t allow” led to a screen with “Use Default Location”; tapping that opened the home screen. We did not explicitly deny location access, test whether the banner returns on later launches, establish how the default location was selected, or test whether browsing and ordering work from it. A separate notification-permission prompt appeared after the home screen; we did not assess its effects.

## 4. Related Literature

- [4.1 Privacy](issues/privacy.md#41-privacy-and-personal-data-in-food-delivery-apps)
- [4.2 Refunds](issues/refunds.md#42-refunds-and-consumer-protection)
- [4.3 Food descriptions, allergens and safety](issues/food-listings-and-allergens.md#43-food-descriptions-allergens-and-food-safety)

## 5. Ethical Issues Identified

- [5.1 Privacy](issues/privacy.md#51-privacy-and-personal-data)
- [5.2 Refunds and cancellations](issues/refunds.md#52-refunds-and-cancellations)
- [5.3 Food descriptions and photos](issues/food-listings-and-allergens.md#53-food-descriptions-and-photos)
- [5.4 Allergen and food safety information](issues/food-listings-and-allergens.md#54-allergen-and-food-safety-information)

## 6. Ethical Analysis

See [Section 6](ethical-analysis.md) for the Code principles, ethical theories and their limits.

## 7. Conclusion

ReMeal is a small, real and little-studied app whose good aims make its ethical issues worth examining. Our first-hand evidence includes policy, app walkthrough and selected listing reviews. Users can reach the home screen without granting location access, but the Terms and the app explain location in different ways, and the Privacy Notice allows wide sharing. We have not found evidence of misuse. Part 2 will test whether ReMeal’s design gives users the information and control they need.

## 8. Plan for Part 2

1. **Close the gaps in our evidence.** Test whether guest users can order. Explicitly deny location access and check whether browsing and checkout still work. Repeat the listing review on different days and at different times.
2. **Extend our methods.** Code a larger sample of app-store reviews for complaints about refunds, listings and allergens. Ask ReMeal directly how data is shared and how refund disputes are handled.
3. **Compare against the law.** Compare ReMeal’s policies with Malaysia’s Personal Data Protection Act 2010 (as amended) and the relevant consumer-protection and food-labelling rules.
4. **Complete the ethical analysis.** Apply both theories to every issue and test where the SE Code is insufficient.
5. **Recommend changes.** Propose practical recommendations for ReMeal’s developers.
6. **Respond to feedback** from Part 1.

We will also avoid harming vendors through our own testing. We will not place orders and then cancel them only to observe the refund process, because this could cost vendors food or sales.

## Appendix

- [App and policy screenshot evidence](appendix/screenshot-evidence.md)

## References

- Abenoh, N. A., Mat Hassan, N. H., & Rahmat, S. M. (2019). Home-based business food delivery in Malaysia: Legal protection for e-consumers. In *20th Kuala Lumpur International Business Economics and Law Conference* (pp. 361–368). [Repository record](https://shdl.mmu.edu.my/9585/)
- Acquisti, A., Brandimarte, L., & Loewenstein, G. (2015). Privacy and human behavior in the age of information. *Science, 347*(6221), 509–514. https://doi.org/10.1126/science.aaa1465
- Al Rezan, M. I., Hosain, M. M., & Karim, M. E. (2025). User acceptance of terms and conditions and privacy policy: A legal analysis of the position of food delivery mobile apps in the Malaysian context. *UUM Journal of Legal Studies, 16*(1), 130–149. https://doi.org/10.32890/uumjls2025.16.1.8
- Apple App Store. (n.d.). *ReMeal – Rescue Surplus Food*. https://apps.apple.com/my/app/remeal-rescue-surplus-food/id6499340832
- Consumer Protection (Electronic Trade Transaction) Regulations 2024 (Malaysia), P.U. (A) 449. https://repositori.kpdn.gov.my/bitstream/123456789/5299/1/PERATURAN%20URUSNIAGA%20PERDAGANGAN%20DALAM%20ELEKTRONIK%202024.pdf
- Ebrahimi, F., Tushev, M., & Mahmoud, A. (2021). Mobile app privacy in software engineering research: A systematic mapping study. *Information and Software Technology, 133*, 106466. https://doi.org/10.1016/j.infsof.2020.106466
- Food Act 1983 (Malaysia), Act 281.
- Food Regulations 1985 (Malaysia), P.U. (A) 437/85. [Ministry of Health Malaysia](https://hq.moh.gov.my/fsq/peraturanperaturan-makanan-1985)
- Google Play. (n.d.). *Provide information for Google Play’s Data safety section*. https://support.google.com/googleplay/android-developer/answer/10787469?hl=en
- IEEE-CS/ACM Joint Task Force. (1999). *Software Engineering Code of Ethics and Professional Practice*. https://www.computer.org/education/code-of-ethics
- Kant, I. (1998). *Groundwork of the metaphysics of morals* (M. Gregor, Trans.). Cambridge University Press. (Original work published 1785)
- Kasinathan, S. (2024, December 2). Learning from “failed” biz models, these M’sians are tackling a persistent F&B pain point. *Vulcan Post*. https://vulcanpost.com/876339/remeal-malaysia-startup-food-surplus-app-reduce-waste
- Keßler, C., & McKenzie, G. (2018). A geoprivacy manifesto. *Transactions in GIS, 22*(1), 3–19. https://doi.org/10.1111/tgis.12305
- Koidis, T., Jia, W., Stoikidou, T., Walker, M., & Gowland, M. H. (2024). *Food allergy awareness champions: Improving food safety standards in online food procurement for people with food hypersensitivities*. Food Standards Agency. https://doi.org/10.46756/sci.fsa.zzx336
- Mill, J. S. (1863). *Utilitarianism*. Parker, Son, and Bourn.
- Nouwens, M., Liccardi, I., Veale, M., Karger, D., & Kagal, L. (2020). Dark patterns after the GDPR: Scraping consent pop-ups and demonstrating their influence. In *Proceedings of the 2020 CHI Conference on Human Factors in Computing Systems*. ACM. https://doi.org/10.1145/3313831.3376321
- Obar, J. A., & Oeldorf-Hirsch, A. (2020). The biggest lie on the internet: Ignoring the privacy policies and terms of service policies of social networking services. *Information, Communication & Society, 23*(1), 128–147. https://doi.org/10.1080/1369118X.2018.1486870
- Personal Data Protection Department, Malaysia. (2024). *Personal Data Protection (Amendment) Act 2024*. https://www.pdp.gov.my/en/akta/personal-data-protection-amendment-act-2024/
- ReMeal. (n.d.-a). *ReMeal*. https://remeal.app/
- ReMeal. (n.d.-b). *ReMeal – Rescue Surplus Food* [Google Play listing]. https://play.google.com/store/apps/details?id=app.remeal.user
- ReMeal. (n.d.-c). *Making your first sale*. https://remeal.app/guides/making-your-first-sale
- ReMeal. (n.d.-d). *Refunds and payouts*. https://remeal.app/guides/refunds-and-payouts
- ReMeal. (2024a). *Privacy Notice*. Last updated 9 June 2024. https://remeal.app/privacy-policy
- ReMeal. (2024b). *Terms and Conditions*. Last updated 21 May 2024. https://remeal.app/terms-and-conditions
- Siali, F., Abdu Shakur, M. B. M., & Mohd Shukri, M. H. (2024). Consumer rights and customer loyalty of online food delivery services among consumers in Sarawak. *International Journal of Business and Society, 25*(Special Issue), 39–53. https://doi.org/10.33736/ijbs.8195.2024
- Soon, J. M. (2018). Food allergen labelling: “May contain” evidence from Malaysia. *Food Research International, 108*, 455–464. https://doi.org/10.1016/j.foodres.2018.03.068
- Tan, A. L., Trupp, A., & Tan, J. X. (2023). Dining out safely with food allergies: A comparative perspective from restaurant managers and servers in Malaysia. *International Food Research Journal, 30*(3), 750–763. https://doi.org/10.47836/ifrj.30.3.17
- Valenta, R., Hochwallner, H., Linhart, B., & Pahr, S. (2015). Food allergies: The basics. *Gastroenterology, 148*(6), 1120–1131.e4. https://doi.org/10.1053/j.gastro.2015.02.006
