# P03 — Supplier Purchase Order Preparation

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Business Function | Procurement |
| Workflow | Planning and Manufacturing |
| Current Version | v1.0 |
| Status | Initial Draft — Not Yet Tested |
| Prompting Strategy | Role-based and structured-output prompting |

---

## 1. Prompt Text

> You are a procurement assistant for Flavors of
> Ceylon, an Australian food production business.
>
> Using the supplied approved purchasing requirements
> and supplier information, prepare a draft purchase
> order for the required food ingredients.
>
> Include ingredient names, quantities, measurement
> units, available prices, requested delivery dates
> and supplier information.
>
> Prepare a professional supplier email in Australian
> English. Use AUD for financial information.
>
> Identify missing information and do not invent
> prices, supplier details or delivery commitments.
>
> The purchase order must remain a draft requiring
> procurement approval.

## 2. Intended Workflow or Task

This prompt supports ingredient procurement.

- Trigger: Replenishment requirements are approved.
- Input: Approved ingredient list and supplier information.
- Output: Draft purchase order and supplier email.
- Responsible person: Procurement officer.
- Next step: Human approval and supplier confirmation.

## 3. Problem Being Solved

Preparing repetitive purchase orders and supplier
emails manually consumes staff time and may result
in inconsistent or incomplete order information.

## 4. Automation Potential

Level: High — Preliminary assessment.

AI can prepare structured purchase order drafts
and supplier communications. Procurement staff
must verify details and authorise all commitments.

## 5. Risks and Limitations

| Risk | Mitigation |
|---|---|
| Incorrect order quantities | Check approved requirements |
| Incorrect prices or totals | Verify supplier quotations |
| Invented delivery terms | Confirm with the supplier |
| Unauthorised commitments | Require procurement approval |

AI must not independently place orders or authorise
supplier payments.

---

## Version History

| Version | Change | Status |
|---|---|---|
| v1.0 | Initial prompt development | Not yet tested |

## Testing Evidence

Pending practical testing in Stage 04.
