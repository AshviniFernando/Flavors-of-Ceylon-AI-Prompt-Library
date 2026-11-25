# P03 — Supplier Purchase Order Preparation: Iteration Log

## 1. Development Objective

Improve AI-assisted purchase order preparation,
financial accuracy, supplier communication
and procurement decision boundaries for
Flavors of Ceylon.

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial role-based procurement prompt | Correct calculations and purchasing safeguards, but lengthy reports; 90% score | Accurate procurement documents must also be practical and efficient |
| v1.1 | Added explicit financial rules, purchasing eligibility controls, concise reporting and separate approvals | Awaiting retesting | Pending evaluation |

---

## 3. Version v1.0 — Initial Prompt

Development and testing dates: [Actual dates]

### Observed Strengths

- Correct ingredient quantities and prices.
- Correct Test A purchase value of AUD 162.00.
- Correct GST-inclusive pricing treatment.
- Appropriate exclusion of provisional purchases.
- Correct Test B known priced-line amount of
  AUD 12.00.
- Appropriate withholding of incomplete totals.
- No invented supplier information.
- Professional draft supplier emails.
- Appropriate human approval safeguards.

### Observed Weaknesses

- Lengthy nine-section and ten-section reports.
- Repeated financial calculations and summaries.
- Overlapping procurement approval checklists.
- Unnecessary AI-generated self-assessment
  in Test Case B.
- Financial and purchasing eligibility rules
  were less explicitly defined in the prompt.

### Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 2 |
| Business Relevance | 1 | 1 |
| Responsible AI | 2 | 2 |
| Total | 9/10 | 9/10 |

Combined score: 18/20 (90%).

Business relevance deductions reflect the
repetition and length of the generated documents,
not numerical inaccuracies.

### Lesson Learned

Correct financial calculations and responsible
AI behaviour are necessary but should also be
supported by concise and practical procurement
documentation.

---

## 4. Version v1.1 — Revised Prompt

Development date: [Actual date]

### Changes Made

- Added explicit purchasing eligibility rules.
- Standardised financial calculations.
- Defined GST and incomplete-price handling.
- Consolidated purchase order financial information.
- Introduced a four-section reporting structure.
- Introduced a concise supplier email requirement.
- Distinguished supplier communication approval
  from purchase order issue approval.
- Removed unnecessary self-assessment requirements.

### Reason for Changes

Initial testing demonstrated strong numerical
accuracy and responsible procurement behaviour.

The revised prompt aims to preserve these strengths
while improving document efficiency, consistency
and approval transparency.

### Expected Effect

The revised prompt is expected to generate
more concise purchase orders and supplier emails
without reducing financial accuracy or
responsible AI safeguards.

This expected effect has not yet been verified.

### Observed Effect

Pending actual retesting.

### Evaluation Scores

Pending.

### Remaining Limitations

Pending final evaluation.

### Lesson Learned

Pending final evaluation.

---

## 5. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 9/10 | 18/20 (90%) |
| v1.1 | Pending | Pending | Pending |

## 6. Current Development Status

Initial v1.0 testing and evaluation are complete.

The v1.1 prompt has been developed based on the
observed opportunities for improvement.

Final retesting remains pending.

Automation potential: High — Preliminary.

Operational deployment: Not implemented.

## Related Evidence

- [P03 Current Prompt](../02-prompt-library/P03-supplier-purchase-order.md)
- [P03 Testing Evidence](../03-testing-evidence/P03-testing-evidence.md)
- [P02 Final Evaluation](../05-evaluation/P02-final-evaluation.md)
