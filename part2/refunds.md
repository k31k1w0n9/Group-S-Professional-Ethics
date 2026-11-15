# Part 2: Refunds and Cancellations

[Back to the report](../README.md) · [Part 1 refunds](../issues/refunds.md) · [Screenshot evidence](../appendix/screenshot-evidence.md)

## Evidence available so far

ReMeal's Terms allow customers to cancel through in-app support before a vendor accepts the order. Under §§ 5.7–5.8, a customer who chooses to cancel after acceptance is not entitled to a refund (ReMeal, 2024b). In our Part 1 walkthrough on 3 November 2026, the delivery cart and checkout screens did not display this restriction before the "Proceed to Payment" button (Appendix, Figs. A18–A20). We did not enter the payment stage or place an order, so we cannot say whether a warning appears later or whether customers can see when a vendor accepts an order.

ReMeal's seller guide also describes full refunds for cancellations and partial refunds when part of an order cannot be fulfilled. It gives an example of a refund after completion when an item was left out (ReMeal, n.d.-d). These are different from a customer simply changing their mind. It would therefore be inaccurate to say that ReMeal never refunds orders after acceptance.

## SE Code analysis: refunds

**Clause 1.06, fairness and honest communication: partially meets.** ReMeal publishes its cancellation rules in the Terms, which is a positive step. However, the absence of a warning on the screens we examined raises a question about whether customers are given the restriction where it matters most. This does not prove deception, since the payment stage remains untested (IEEE-CS/ACM Joint Task Force, 1999).

**Clause 3.01, making trade-offs clear: partially meets.** The restriction has a reasonable purpose. Vendors may already be preparing food when an order is accepted, and late cancellations could leave them with unsold food. The trade-off is that customers risk losing their payment once acceptance takes place. Unless the app explains this point clearly and shows the order's status, users may not know when their options have changed. We need to check the order-status screens before making a final judgement.

**Clause 2.07, reporting concerns: relevant to improvement.** Engineers who find that customers cannot understand or check the cancellation cut-off should document the problem and raise it with the team responsible for the ordering process. Our screenshots identify a concern worth testing, not evidence of a confirmed Code breach.

## Comparison with Malaysian consumer rules

The Consumer Protection (Electronic Trade Transaction) Regulations 2024 require online marketplace suppliers to disclose terms and conditions of sale (reg. 3 and the Schedule). Regulation 6 requires an appropriate way to correct order errors before or after confirmation, while regulation 7 requires marketplace operators to provide a complaint channel. ReMeal publishes its Terms and provides in-app support (ReMeal, 2024b). What remains unclear is how easily customers can find and use these protections during an order. The Regulations do not explicitly require a separate cancellation warning beside the payment button or give an unrestricted right to cancel after acceptance. Our evidence is insufficient to conclude that ReMeal has breached them.

## Proposed recommendations for the four issues

1. **Privacy:** Give users a clear choice between manual location entry and device location access, and explain what each option changes. This supports informed choice under Kantian deontology; the privacy team's planned tests will determine what is already available.
2. **Refunds:** Show the cancellation cut-off before payment, then display vendor acceptance clearly in the order status and provide an obvious route to support. This supports Kantian informed choice while protecting vendors from late cancellations.
3. **Descriptions and photos:** Ask vendors to identify what a photo includes, correct conflicting collection times, and label illustrative images. This follows Kantian duties of honest communication without removing the flexibility of surplus-food offers.
4. **Allergens:** Provide separate fields for known allergens, possible cross-contact and information that the vendor cannot confirm. This follows utilitarian reasoning by reducing avoidable safety risks while allowing vendors to state uncertainty rather than invent details.

## Still to check

- Inspect the next payment screen without entering payment details or placing an order. Record whether the policy is displayed.
- Check whether customers can see vendor acceptance and how to request cancellation or report an incorrect order. Record screenshots and dates.
- Review refund-related feedback in the group's shared app-store sample. Record the review text, date and context; do not treat unverified complaints as established facts.

## References

- Consumer Protection (Electronic Trade Transaction) Regulations 2024 (Malaysia), P.U. (A) 449. https://repositori.kpdn.gov.my/bitstream/123456789/5299/1/PERATURAN%20URUSNIAGA%20PERDAGANGAN%20DALAM%20ELEKTRONIK%202024.pdf
- IEEE-CS/ACM Joint Task Force. (1999). *Software Engineering Code of Ethics and Professional Practice*. https://www.computer.org/education/code-of-ethics
- ReMeal. (n.d.-d). *Refunds and payouts*. https://remeal.app/guides/refunds-and-payouts
- ReMeal. (2024b). *Terms and Conditions*. https://remeal.app/terms-and-conditions
