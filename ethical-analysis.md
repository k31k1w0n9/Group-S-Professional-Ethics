# 6. Ethical Analysis

[Back to the report](README.md) · [Privacy](issues/privacy.md) · [Refunds](issues/refunds.md) · [Listings and allergens](issues/food-listings-and-allergens.md)

### 6.1 Relevant ACM/IEEE Code Principles

Clause **3.12** requires engineers to develop software and documents that respect affected users’ privacy. Clause **3.13** says data should be accurate, obtained by ethical and lawful means, and used only in properly authorised ways, and **1.03** says software should be approved only when engineers have a well-founded belief that it does not diminish privacy. Clause **1.06** calls for fair, non-deceptive statements; we note the difference between the Terms’ “required” location and the app’s “greater experience” wording without alleging deception. Clauses **2.07** and **2.09** guide engineers to document and raise significant concerns, including with an appropriate authority if a higher ethical concern is compromised (IEEE-CS/ACM Joint Task Force, 1999).

## 6.2 Applying Ethical Theories

### 6.2.1 Utilitarianism

**Utilitarianism** (Mill, 1863) suits ReMeal’s trade-offs. Its benefits (less waste, cheaper food and vendor income) must be weighed against harms to individual users, such as a refused refund or a reaction to an undisclosed allergen. Store pages display CO₂e savings estimates, but we have not verified how they are calculated.

For privacy, location data helps show nearby vendors but risks unwanted sharing or exposure. Users reached the home screen without granting device access, but we did not test checkout from the default location.

### 6.2.2 Kantian Deontology

**Kantian deontology** (Kant, 1785/1998) suits the issues of information and consent: whether users can make informed choices about their data, money and food. Misleading or withholding information is wrong even if the app does net good, so a worthy cause cannot excuse it.

For privacy, the Terms call a location “required”, while the app calls device access a “greater experience”. This mismatch may weaken informed consent. We did not establish whether the Terms mean manual entry or device permission, or whether users can control optional data uses.

### 6.3 Where the Code May Not Fully Address an Issue

The Code does not specify what location data is needed or whether consent is meaningful if refusing access limits service. It also leaves the privacy–convenience trade-off unresolved. These choices may sit with product management, outside an individual engineer’s control, so applying the Code requires evidence and ethical judgement.

The food listings show a related risk pathway: ReMeal controls how listing information is displayed, while vendors provide food details and prepare the orders. Customers rely on those listings but are directed to contact vendors about allergens and inspect orders at collection. If allergen information is missing, the customer faces the immediate health risk, while practical disclosure and food-handling responsibilities sit with the vendor. This describes how the platform design may distribute operational risk; it does not establish legal liability. The Code does not set out marketplace-specific duties for checking vendor information or governing platform–vendor safety responsibilities.
