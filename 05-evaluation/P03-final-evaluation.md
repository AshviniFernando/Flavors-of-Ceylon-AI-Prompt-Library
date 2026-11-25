# P03 — Supplier Purchase Order Preparation: Final Evaluation

## 1. Evaluation Information

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Food Manufacturing and Hospitality |
| Prompt ID | P03 |
| Business Function | Procurement |
| Initial Version | v1.0 |
| Final Selected Version | v1.1 |
| Evaluation Status | Completed |
| Data Type | Synthetic business data |
| Automation Potential | High — Document preparation |
| Operational Deployment | Not implemented |

## 2. Evaluation Objective and Methodology

Evaluate the ability of generative AI to prepare
accurate draft purchase orders, calculate financial
amounts and generate professional supplier emails.

Two synthetic scenarios were used:

- Test A: Complete purchasing and supplier information.
- Test B: Missing commercial information and
  unapproved purchasing requirements.

Both prompt versions were tested using the same
original datasets without supplying expected answers.

The evaluation considered accuracy, completeness,
consistency, business relevance and responsible AI,
using a zero-to-two scoring scale for each criterion.

## 3. Prompting Strategies

- Role-based prompting.
- Contextual prompting.
- Constraint-based prompting.
- Rule-based purchasing classification.
- Explicit mathematical instructions.
- Structured-output prompting.
- Human-in-the-loop decision support.

## 4. Version Performance

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 9/10 | 18/20 (90%) |
| v1.1 | 9/10 | 10/10 | 19/20 (95%) |

Absolute improvement: 5 percentage points.

Relative improvement in evaluation score: 5.56%.

## 5. Final Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 2 |
| Business Relevance | 1 | 2 |
| Responsible AI | 2 | 2 |
| Total | 9/10 | 10/10 |

Final combined score: 19/20 (95%).

The Test A business relevance deduction reflects
remaining repetition in the procurement document.

The score represents response quality under
selected synthetic scenarios rather than actual
commercial procurement performance.

## 6. Key Testing Results

### Test A — Standard Procurement

| Ingredient | Quantity | Unit Price (AUD) | Line Amount (AUD) |
|---|---:|---:|---:|
| Wheat flour | 15 kg | 2.40 | 36.00 |
| Chicken | 12 kg | 9.50 | 114.00 |
| Ingredient subtotal | | | 150.00 |
| Delivery charge | | | 12.00 |
| Total proposed purchase value | | | 162.00 |

Prices were inclusive of any applicable GST.

Requested delivery: 4 December 2026.

Supplier availability and delivery acceptance
remained pending confirmation.

### Test B — Challenging Procurement

| Ingredient | Quantity | Purchasing Status | Line Amount (AUD) |
|---|---:|---|---:|
| Wheat flour | 5 kg | Included in draft | 12.00 |
| Grated coconut | 6 kg | Included; price pending | Pending |
| Rice | 5 kg | Excluded — provisional | Not applicable |
| Chicken | 15 kg | Excluded — provisional | Not applicable |
| Eggs | 0 units | Excluded — unnecessary | Not applicable |

| Indicator | Result |
|---|---|
| Approved draft quantity | 11 kg |
| Excluded provisional quantity | 20 kg |
| Known priced-line subtotal | AUD 12.00 |
| Complete ingredient subtotal | Pending |
| GST treatment | Pending verification |
| Delivery charges | Pending |
| Final purchase order total | Pending |
| Supplier email recipient | Pending verification |
| Procurement approval | Pending |

The AI correctly withheld incomplete financial
totals and excluded unauthorised purchases.

## 7. Observed Improvements

- Standardised financial calculations.
- Clearer purchasing eligibility rules.
- Consolidated financial reporting.
- Four-section document organisation.
- Separate communication and order approvals.
- Removal of unnecessary AI self-assessment.
- Preservation of missing-data safeguards.
- Retention of correct numerical calculations.

## 8. Business Workflow Integration

P03 receives purchasing requirements from
P02 Ingredient Inventory and Replenishment
after human approval.

Provisional replenishment requirements remain
excluded until inventory verification and
purchasing approval are completed.

Approved purchase orders and confirmed supplier
deliveries may subsequently support P04 Food
Production and Batch Planning.

Draft orders and requested delivery dates must
not be treated as confirmed available ingredients.

## 9. Automation Potential

Classification: High — Document preparation.

AI can assist with purchase order drafting,
financial calculations, missing information
identification and supplier email preparation.

However, supplier verification, communication
authorisation and purchasing commitments
require human approval.

High automation potential does not authorise
autonomous purchasing.

## 10. Potential Business Value

| Business Area | Potential Benefit |
|---|---|
| Procurement | More consistent draft purchase orders |
| Finance | Transparent financial calculations |
| Administration | Reduced repetitive document preparation |
| Supplier Management | More structured supplier communications |
| Risk Management | Reduced risk of unapproved purchasing |
| Production Planning | Improved visibility of pending ingredient deliveries |

Actual time savings, cost savings and commercial
performance improvements have not been measured.

## 11. Risks and Limitations

| Risk or Limitation | Mitigation |
|---|---|
| Incorrect financial calculations | Independently verify prices and totals |
| Missing prices or charges | Withhold incomplete purchase totals |
| Incorrect GST treatment | Verify applicable tax information |
| Unapproved purchasing requirements | Exclude from orders and supplier emails |
| Unverified supplier details | Confirm before external communication |
| Unconfirmed deliveries | Obtain supplier confirmation |
| Repeated document content | Apply approved procurement templates |
| Food quality concerns | Verify approved ingredient requirements |
| Unauthorised purchasing | Require procurement manager approval |

GST-exclusive pricing, discounts, multiple
suppliers and minimum order constraints have
not been directly tested.

Repeat-run reliability remains unverified.

## 12. Human-in-the-Loop Requirements

Responsible procurement personnel must:

1. Verify approved purchasing requirements.
2. Confirm supplier information and quotations.
3. Independently verify financial calculations.
4. Approve supplier communication before sending.
5. Confirm ingredient availability, quality
   requirements and delivery acceptance.
6. Authorise the final purchase order.

AI must not independently issue orders,
send emails, authorise dispatch or certify
ingredient suitability.

## 13. Critical Reflection

The initial prompt produced correct financial
calculations but generated lengthy reports with
repeated information.

The revised prompt introduced explicit financial
rules, structured reporting and separate
approval boundaries.

These changes improved the challenging scenario
without changing the underlying financial results.

Minor repetition remains, demonstrating that
AI-generated procurement documents may still
require human editing.

## 14. Final Recommendation

Version v1.1 is selected as the final P03 prompt.

It is recommended for supervised purchase order
preparation and supplier communication drafting.

Automation potential remains High for document
preparation, subject to human approval.

The prompt has not been commercially deployed.

## 15. Supporting Evidence

- [Final Prompt](../02-prompt-library/P03-supplier-purchase-order.md)
- [Testing Evidence](../03-testing-evidence/P03-testing-evidence.md)
- [Iteration History](../04-iteration-logs/P03-iteration-log.md)
- [P02 Final Evaluation](P02-final-evaluation.md)
- [Evaluation Index](README.md)
- [Main Portfolio](../README.md)

---

**Final Status: P03 Completed — Version v1.1**

Final evaluation score: 19/20 (95%).
