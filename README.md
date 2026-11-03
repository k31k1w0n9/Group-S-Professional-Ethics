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

This proposal sets up our ethical review of ReMeal, a Malaysian app selling surplus food from local vendors at reduced prices. We ask whether an app with a worthwhile aim (less food waste and cheaper meals) can still treat users unfairly through its design and policies. We examine four issues: privacy, refunds and cancellations, food descriptions, and allergen information.

## 2. System Overview and Selection Rationale

### 2.1 What ReMeal Does

ReMeal, developed by ReMeal Sdn. Bhd., connects cafés, bakeries, supermarkets and restaurants with customers buying surplus food at reduced prices. Users pay in the app and, depending on the vendor, collect, dine in or use delivery (ReMeal, n.d.-a). In December 2024 it had 16 active stores and 1,800 user sign-ups, and customers collected orders from vendors (Kasinathan, 2024).

### 2.2 Why We Chose ReMeal

ReMeal is real, downloadable and small: our preliminary searches found press coverage and ReMeal’s own pages, but no academic studies of it. It has ethically relevant features. Its developer-provided App Store privacy label lists location and purchase history among the data it may collect, it handles payments and refunds, and customers rely on vendor listings to know what they are buying.

Its good aims raised our question: can a well-intentioned app still treat users unfairly? Surplus food also makes it a new case. Stock depends on what vendors have left, so listings carry more weight. Responsibility is also split between ReMeal and independent vendors. The food-app research we found mainly concerns delivery platforms (e.g. Al Rezan et al., 2025), so ReMeal lets us test whether known problems carry over to a different model.

## 3. Investigation Method

### 3.1 Investigation Plan

Each issue has one owner:

| Issue | Methods |
|---|---|
| Privacy and data | Privacy Notice and Terms; Android app walkthrough of permission prompts; app-store privacy labels |
| Refunds and cancellations | Terms and ReMeal’s seller guides on acceptance, cancellation and refunds |
| Food descriptions and photos | Four listings from two stores, each checked for contents, ingredients, price, availability, collection rules and photos |
| Allergens and food safety | Terms on allergens; the same listings checked for allergen details |

We date and number every screenshot in the Appendix, treat developer disclosures as claims rather than facts, and do not call a listing inaccurate unless we can verify it.

### 3.2 Evidence and Limitations

Our screenshots (Appendix, Figs. A1–A17) show what the app and policies displayed on the dates we captured them. We captured the listings on 1 September 2026, the privacy walkthrough on 2 November and the App Store summary on 3 November. App-store privacy labels are supplied by the developer, not independently audited. We did not inspect network traffic, ReMeal’s servers, or how vendors and service providers handle data. Our location test followed one path. We did not explicitly deny access, test later launches, establish how the default location is chosen, or assess the separate notification prompt.

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

Our evidence so far raises four concerns, none yet proof of wrongdoing. The Terms and the app explain location differently, and the Privacy Notice allows wide sharing. Refunds end once a vendor accepts an order, and we have not yet checked how clearly the app shows this. Listings vary in detail, and allergen information is inconsistent, with responsibility left to vendors. Part 2 will test whether ReMeal gives users the information and control they need.

## 8. Plan for Part 2

1. **Close evidence gaps:** test guest ordering, and browsing and checkout with location denied; check how the app shows vendor acceptance and refund rules; review more listings on different days.
2. **Extend methods:** code app-store reviews by theme, and ask ReMeal how data is shared and refund disputes handled.
3. **Compare with Malaysian law:** the Personal Data Protection Act 2010 (as amended), consumer-protection rules and food-labelling rules.
4. **Complete the analysis:** apply both theories to every issue, respond to Part 1 feedback, and recommend changes to ReMeal’s developers.

We will not place and cancel orders only to test refunds, as this could cost vendors food or sales.

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
