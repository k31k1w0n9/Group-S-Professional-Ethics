# 6. Ethical Analysis

[Back to the report](README.md) · [Privacy](issues/privacy.md) · [Refunds](issues/refunds.md) · [Listings and allergens](issues/food-listings-and-allergens.md)

### 6.1 Relevant ACM/IEEE Code Principles

Clause **3.12** requires engineers to develop software and documents that respect affected users’ privacy. Clause **3.13** says data should be accurate, obtained by ethical and lawful means, and used only in properly authorised ways, and **1.03** says software should be approved only when engineers have a well-founded belief that it does not diminish privacy. Clause **1.06** calls for fair, non-deceptive statements; we note the difference between the Terms’ “required” location and the app’s “greater experience” wording without alleging deception. Clauses **2.07** and **2.09** guide engineers to document and raise significant concerns, including with an appropriate authority if a higher ethical concern is compromised (IEEE-CS/ACM Joint Task Force, 1999).

## 6.2 Applying Ethical Theories

### 6.2.1 Utilitarianism

**Utilitarianism** (Mill, 1863) suits the trade-offs. ReMeal produces real benefits: less waste, cheaper food and extra income for vendors. A fair judgement must weigh these against harms to individual users, such as money lost on a refused refund or a reaction to an undisclosed allergen. Store pages display CO₂e savings estimates, but we have not verified how they are calculated.

Under **utilitarianism**, we weigh the benefits of location data, such as showing nearby vendors, against risks such as unwanted sharing or exposure. Our test shows users could reach the home screen without granting device-location access; we did not test browsing or checkout from the default location.

### 6.2.2 Kantian Deontology

**Kantian deontology** (Kant, 1785/1998) suits the issues of information and consent. It asks whether users can make informed choices about their data, their money and what they eat. On this view, misleading or withholding information is wrong even when the app does more good than harm overall. This stops us from excusing a problem because the cause is worthy.

Under **Kantian deontology**, users need enough information to consent knowingly. The guest and default-location options show some choice, but not whether users can order or control optional data uses. The Terms call location provision “required”, while the app describes device access as a “greater experience” and provides a default-location path. This difference may weaken users’ ability to make a rational, informed choice; we did not establish whether the Terms refer to manual location entry or device permission.

### 6.3 Where the Code May Not Fully Address an Issue

The Code does not specify what location data is needed or whether consent is meaningful if refusing access limits service. It also leaves the privacy–convenience trade-off unresolved. These choices may sit with product management, outside an individual engineer’s control, so applying the Code requires evidence and ethical judgement.

We expect a similar gap for refunds and allergen information. Vendors, not ReMeal’s engineers, prepare the food and may supply much of each listing. The Code addresses engineers and their software, so it says little about how responsibility should be shared between a platform and its vendors. We will test this expectation in Sections 5.2–5.4.

The food listings show a related risk pathway: ReMeal controls how listing information is displayed, while vendors provide food details and prepare the orders. Customers rely on those listings but are directed to contact vendors about allergens and inspect orders at collection. If allergen information is missing, the customer faces the immediate health risk, while practical disclosure and food-handling responsibilities sit with the vendor. This describes how the platform design may distribute operational risk; it does not establish legal liability. The Code does not set out marketplace-specific duties for checking vendor information or governing platform–vendor safety responsibilities.
