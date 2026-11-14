# Part 2 — Allergens and Food Safety

[Back to the report](../README.md) · [Part 1 allergen findings](../issues/food-listings-and-allergens.md#54-allergen-and-food-safety-information)

## New Evidence: Allergen Survey of All Public Listings

Part 1 reviewed four listings from two stores. To test whether the gaps found there are typical, on 12 November 2026 we reviewed every listing (including sold-out items) at all 18 stores shown on ReMeal’s public web shop, with the location set to Kuala Lumpur (ReMeal, n.d.-e). We recorded any allergen wording in each listing (Appendix, Table B1). The web shop may differ from the mobile app, which we check separately.

**Table 5.1. Allergen information across 178 listings**

| Measure | Result |
|---|---|
| Listings with any allergen statement | 32 of 178 (18%), from 2 of 18 stores |
| Stores with no allergen statement on any listing | 16 of 18 |
| Mystery or surprise items with no allergen statement | 15 of 15 (bakery bags, cakes, bento) |
| Listings sold specifically for children with no allergen statement | 13 of 13 |
| Allergen statements with an unclear or contradictory meaning | 2 of 32 |

Excluding one grocer’s 31 items (raw produce, rice and coffee), the share with an allergen statement is 32 of 147 (22%).

Allergen information is written as free text inside each description, so its format depends on the vendor. Sunset Terrace’s newer set meals separate “Contains” from “May contain” and warn of cross-contamination risk. Its earlier menus list allergens without saying which category applies. Two notes are unclear. One reads “Shelfish,Dairy,Nuts,Gluten free”, which could mean that the dish is free of all four or only of gluten. Another lists “shellfish (razor clam)” and then “no shellfish, fish, egg as ingredients”. Krem Tarik uses a short, consistent line (“Contains dairy”), once misspelt “Contains diary”.

## Analysis Using the SE Code

### Clause 1.04 — Disclose potential dangers: partly meets

**Claim.** ReMeal discloses the general allergen risk, but not where customers decide what to buy.
**Evidence.** The Terms say goods are not guaranteed allergen-free and tell customers to contact the vendor (ReMeal, 2024b, § 5.3). Yet 146 of 178 listings carry no allergen statement or warning.
**Reasoning.** Clause 1.04 asks engineers to disclose potential dangers associated with software or related documents to appropriate persons. A warning placed only in the Terms reaches few users, since most people skip such documents (Obar & Oeldorf-Hirsch, 2020).
**Counterpoint.** The danger comes from the food, not the software, and ReMeal does disclose it. However, listing pages are the documents customers rely on, so a warning there falls within the clause.

### Clause 1.03 — Approve only safe software: partly meets

**Claim.** The listing design leaves safety information entirely to vendors’ free text.
**Evidence.** Formats vary, two notes are contradictory, and misspellings appear. Sunset Terrace shows that clear “Contains / May contain” statements are feasible.
**Reasoning.** Software that publishes a note such as “Shelfish,Dairy,Nuts,Gluten free” without a structured field or a prompt to check it gives no well-founded belief that allergen information is safe to rely on.
**Counterpoint.** Even a perfect field depends on vendors’ knowledge and food handling, which ReMeal cannot verify (Tan et al., 2023). The platform can improve how information is collected, but cannot guarantee it is accurate.

### Clause 1.07 — Consider factors that reduce access: diverges (provisional)

**Claim.** Customers with food allergies get little of ReMeal’s benefit.
**Evidence.** Sixteen of 18 stores give no allergen information. All 15 mystery items and all 13 children’s listings lack it.
**Reasoning.** Clause 1.07 asks engineers to consider factors that diminish access to software’s benefits. Food hypersensitivity is such a factor, and the cheapest items (mystery bags) are the least usable.
**Counterpoint.** Mystery items are uncertain by design, and customers can ask vendors. This shifts the burden to each customer, though, and the verdict stays provisional until we check the app for filters and test how vendors respond.

## Why the Code Cannot Settle This (input for Section 6)

The tension sits inside clause 1.03 itself, which asks for software that is safe and does not harm the environment. Requiring a structured allergen field supports safety, but it may deter small vendors from listing surplus food, which works against waste reduction. Mystery bags are the hardest case: their contents change daily, so an accurate allergen list may be impossible, yet they make up a large share of affordable items. The decision also lies with ReMeal’s management and its vendors rather than with individual engineers. The evidence for the theories section is:

- **Feasibility:** Sunset Terrace (20 detailed statements) and Krem Tarik (12 one-line statements) show that disclosure is possible.
- **Hardest case:** 15 mystery items carry no statement.
- **Who is exposed:** the 13 children’s listings show that the people at risk may not be the people placing the order.

## Still To Do

1. Screenshot in the app the listings quoted above (the two unclear Sunset Terrace notes, a Gula Cakery mystery bag, a Hogan Bakery item, “Contains diary”) for the Appendix.
2. Check whether the app has an allergen filter or field, and whether the § 5.3 warning appears at checkout.
3. Ask one vendor about allergens in a mystery bag through the in-app chat without ordering, and record the reply time and answer.
4. Lead the slides.

## Appendix Table B1. Allergen Statements by Store (web shop, 12 November 2026)

| Store | Type | Listings | With allergen statement | Notes |
|---|---|---:|---:|---|
| Sunset Terrace, Sunway Resort Hotel | Hotel restaurant | 32 | 20 | Set meals only; none on 12 buffets (4 for children) |
| CitraRasa @ Dorsett Putrajaya | Hotel restaurant | 20 | 0 | 5 children’s listings; 1 surprise bento |
| Palms Café, Palm Garden Hotel | Hotel café | 23 | 0 | Some list ingredients (e.g. prawn, egg, cheese); 3 children’s listings |
| Cafe Mint, Cosmo Hotel KL | Hotel café | 5 | 0 | |
| Dorsett Kuala Lumpur | Hotel restaurant | 6 | 0 | 1 children’s listing; 1 surprise pastry bag |
| Miss Shortcakes | Bakery | 22 | 0 | 1 mystery item |
| fivetrees.kl | Café | 10 | 0 | 1 mystery bag |
| El Ocho – KLGCC | Café (sells Gula Cakery bags) | 1 | 0 | Mystery bag |
| Gula Cakery (4 outlets) | Bakery | 4 | 0 | All mystery bags |
| YAFA Restaurant | Restaurant | 2 | 0 | |
| FORUS Farmers Market & Cafe | Grocer | 31 | 0 | Mostly raw produce, rice and coffee |
| Terazza Brasserie, Dorsett Grand Subang | Hotel restaurant | 2 | 0 | |
| Hogan Bakery, Cheras Leisure Mall | Bakery | 6 | 0 | All surprise or mystery items |
| Dorsett Hartamas Kuala Lumpur | Hotel restaurant | 2 | 0 | Breakfast includes a children’s menu |
| Krem Tarik, Kota Damansara | Ice-cream shop | 12 | 12 | “Contains dairy” on all; one “may contain nuts”; one “diary” |
| **Total** | | **178** | **32** | |
