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
| v1.1 | Added explicit financial rules, purchasing eligibility controls, structured reporting and separate approvals | Improved document organisation and approval transparency; 95% score | Structured outputs and explicit approval boundaries improve procurement decision support |

---

## 3. Version v1.0 — Initial Prompt

Development and testing dates: [Actual dates]

### Observed Strengths

- Correct ingredient quantities and prices.
- Correct Test A purchase value of AUD 162.00.
- Appropriate GST-inclusive pricing treatment.
- Correct exclusion of provisional purchases.
- Correct Test B known priced-line amount
  of AUD 12.00.
- Appropriate withholding of incomplete totals.
- No invented supplier information.
- Professional draft supplier emails.
- Appropriate human approval safeguards.

### Observed Weaknesses

- Lengthy nine-section and ten-section reports.
- Repeated financial information and summaries.
- Overlapping procurement approval checklists.
- Unnecessary AI-generated self-assessment.
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

### Lesson Learned

Correct calculations and responsible purchasing
recommendations should be supported by concise,
practical procurement documentation.

---

## 4. Version v1.1 — Revised Prompt

Development and testing dates: [Actual dates]

### Changes Made

- Added explicit purchasing eligibility rules.
- Standardised financial calculations.
- Defined GST and missing-price handling.
- Consolidated purchase order financial summaries.
- Introduced a four-section reporting structure.
- Introduced concise supplier email requirements.
- Separated communication and order approvals.
- Prohibited unnecessary AI self-assessment.

### Reason for Changes

The revised prompt aimed to retain numerical
accuracy and responsible procurement behaviour
while improving reporting efficiency and
approval transparency.

### Expected Effect

More structured procurement documents with
clearer financial and approval boundaries.

### Observed Effect

Test A retained the correct proposed purchase
value of AUD 162.00.

Test B correctly included only approved
purchasing quantities of 11 kg and excluded
20 kg of provisional requirements.

The known priced-line subtotal of AUD 12.00
was calculated correctly, while the final
purchase order total remained pending.

Both outputs followed the four principal
reporting sections.

Separate approval requirements for supplier
communication and purchase order issue were
clearly presented.

The unnecessary self-assessment observed
during initial testing was removed.

### Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 2 |
| Business Relevance | 1 | 2 |
| Responsible AI | 2 | 2 |
| Total | 9/10 | 10/10 |

Combined score: 19/20 (95%).

### Remaining Limitations

- Some repeated financial and approval
  information remains.
- Actual procurement time savings have not
  been measured.
- GST-exclusive pricing scenarios have not
  been directly tested.
- Discounts, multiple suppliers and minimum
  order constraints have not been tested.
- Repeat-run reliability has not been established.
- Supplier information and financial calculations
  still require human verification.

### Lesson Learned

Prompt refinement can improve document
organisation and operational decision boundaries
without changing numerical results.

Separate approvals for communication and
purchase order issue help prevent unauthorised
commercial commitments.

---

## 5. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 9/10 | 18/20 (90%) |
| v1.1 | 9/10 | 10/10 | 19/20 (95%) |

Absolute improvement: 5 percentage points.

Relative improvement in evaluation score: 5.56%.

## 6. Final Version Selection

Version v1.1 is selected as the final prompt.

The revised version retains numerical accuracy
and responsible AI safeguards while improving
document organisation and approval transparency.

Minor repetition does not justify further
refinement within the current assessment scope.

Automation potential: High for document
preparation, not autonomous procurement.

Development status: Completed.

Operational deployment: Not implemented.

## Related Evidence

- [P03 Final Prompt](../02-prompt-library/P03-supplier-purchase-order.md)
- [P03 Testing Evidence](../03-testing-evidence/P03-testing-evidence.md)
- [P03 Final Evaluation](../05-evaluation/P03-final-evaluation.md)
- [P02 Final Evaluation](../05-evaluation/P02-final-evaluation.md)
- [Iteration Log Index](README.md)
