# P02 — Ingredient Inventory and Replenishment: Iteration Log

## 1. Development Objective

Improve ingredient inventory assessment,
replenishment calculations, expiry management
and responsible purchasing recommendations
for Flavors of Ceylon.

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial role-based inventory management prompt | Correct calculations but inconsistent purchasing classifications and FEFO terminology; 85% score | Correct calculations alone do not guarantee clear operational recommendations |
| v1.1 | Added eligibility rules, purchasing classifications, correct FEFO terminology and structured reporting | Improved purchasing transparency and inventory assessment; 95% score | Explicit classification rules improve business usability and responsible decision support |

---

## 3. Version v1.0 — Initial Prompt

Development and testing dates: [Actual dates]

### Observed Strengths

- Correct inventory and replenishment calculations.
- Correct conversion of grams into kilograms.
- Appropriate exclusion of expired inventory.
- Appropriate handling of missing expiry information.
- Recognition of stock expiring before planned usage.
- Identification of shortages and surplus inventory.
- Human verification and purchasing approval.

### Observed Weaknesses

- Incorrect FEFO terminology.
- Inconsistent description of provisional shortages.
- Combined purchasing total without separate
  established and provisional subtotals.
- Subjective risk classifications.
- Repeated information across lengthy reports.

### Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 1 | 1 |
| Completeness | 2 | 2 |
| Consistency | 2 | 1 |
| Business Relevance | 2 | 2 |
| Responsible AI | 2 | 2 |
| Total | 9/10 | 8/10 |

Combined score: 17/20 (85%).

### Lesson Learned

Accurate calculations must be supported by clear
purchasing classifications and appropriate
inventory eligibility rules.

---

## 4. Version v1.1 — Revised Prompt

Development and testing dates: [Actual dates]

### Changes Made

- Added explicit inventory eligibility categories.
- Standardised measurement unit validation.
- Defined established and provisional purchasing
  requirements.
- Required separate purchasing subtotals.
- Corrected FEFO terminology.
- Strengthened food safety decision boundaries.
- Introduced a five-section reporting structure.

### Reason for Changes

The changes address observed weaknesses in
purchasing classification, terminology and
reporting efficiency.

### Observed Effect

Test A correctly identified established
replenishment requirements of 27 kg.

Test B correctly separated the total indicative
replenishment of 31 kg into:

- Established requirements: 11 kg.
- Provisional requirements: 20 kg.

All ten inventory batches were classified
correctly in Test B.

Missing measurement units and expiry information
were not invented or assumed.

Correct FEFO terminology was maintained, and
purchasing decisions remained subject to
human approval.

Both reports followed the requested five
principal reporting sections.

### Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 1 |
| Business Relevance | 2 | 2 |
| Responsible AI | 2 | 2 |
| Total | 10/10 | 9/10 |

Combined score: 19/20 (95%).

### Remaining Limitations

- Subjective action priority classifications
  remain without defined thresholds.
- Some repeated information remains.
- Physical inventory accuracy has not been tested.
- Supplier lead times and purchasing costs
  were not available.
- Additional purchasing constraints were
  not directly tested.
- Repeat-run reliability has not been established.
- Food safety and purchasing decisions still
  require qualified human verification.

### Lesson Learned

Explicit inventory eligibility rules and
purchasing classifications improve operational
decision support without changing the underlying
numerical replenishment calculations.

Separating established and provisional requirements
helps management understand which quantities
require additional verification.

A final prompt can remain useful even when minor
limitations exist.

---

## 5. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 8/10 | 17/20 (85%) |
| v1.1 | 10/10 | 9/10 | 19/20 (95%) |

Absolute improvement: 10 percentage points.

Relative improvement in evaluation score: 11.76%.

## 6. Final Version Selection

Version v1.1 is selected as the final prompt.

The revised version successfully addresses the
main weaknesses identified during initial testing.

The remaining minor reporting limitations do
not justify another development iteration
within the current assessment scope.

Automation potential: Medium.

Development status: Completed.

Operational deployment: Not implemented.

## Related Evidence

- [P02 Final Prompt](../02-prompt-library/P02-inventory-and-replenishment.md)
- [P02 Testing Evidence](../03-testing-evidence/P02-testing-evidence.md)
- [P02 Final Evaluation](../05-evaluation/P02-final-evaluation.md)
- [Iteration Log Index](README.md)
