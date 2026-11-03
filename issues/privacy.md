# Issue 1: Privacy and Personal Data

[Back to the report](../README.md) · [Ethical analysis](../ethical-analysis.md) · [Screenshot evidence](../appendix/screenshot-evidence.md)

## 4.1 Privacy and Personal Data in Food Delivery Apps

Privacy studies show limits to notice-and-consent. Ebrahimi et al. (2021) mapped 59 software-engineering studies, mostly on leak detection. Obar and Oeldorf-Hirsch (2020) found 74% of 543 participants skipped a policy for a fictitious social network. Nouwens et al. (2020) found 11.8% of 680 UK sites using five consent platforms met minimum criteria; the sample was not representative. Al Rezan et al. (2025) found nine Malaysian food apps failed the authors’ standards. Acquisti et al. (2015) and Keßler and McKenzie (2018) highlight context and location. These guide our checks, not findings about ReMeal.

## 5.1 Privacy and Personal Data

ReMeal says it may collect contact, location, transaction, app, device and message data; share orders with vendors, contact details for marketing/chat, and data with service providers; and transfer data overseas (ReMeal, 2024a, §§ 1, 3–5; Appendix, Figs. A6–A9). Its notice also treats provision of personal data as agreement to processing (§ 1; Fig. A11).

Sign-in offers guest access but links account creation with agreement to the Terms and Privacy Policy; no separate consent control is visible (Fig. A1). The Terms require an account (§ 2.1), treat platform use as consent to processing (§ 1.0), and require deletion requests by email (§ 2.2; Figs. A4–A5). The account form and guest ordering were not tested.

The Terms require a location to show vendors (§ 5.5; Fig. A10), while the app calls device access a “greater experience.” “Set From Map” triggered Android’s prompt; backing out offered “Use Default Location” and opened the home screen without a grant (Figs. A2–A3, A12). We did not test ordering from the default, so GPS necessity is unknown.

Apple’s developer-provided App Store summary says Purchases, Location, Contact Info, Identifiers and Usage Data may be linked to users, while Diagnostics may be collected without being linked (Apple App Store, n.d.; Appendix, Fig. A16). The Google Play label says data “isn’t encrypted” (ReMeal, n.d.-b; Fig. A8); Google defines this field as encryption in transit, not at rest (Google Play, n.d.). These disclosures are not independent audits. We found no evidence of misuse; our concern is whether users understand the scope and choices.
