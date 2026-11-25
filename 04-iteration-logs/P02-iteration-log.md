# P02 — Ingredient Inventory and Replenishment: Iteration Log

## 1. Development Objective

Improve ingredient inventory assessment,
replenishment calculations, expiry management
and responsible purchasing recommendations
for Flavors of Ceylon.

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial role-based inventory management prompt | Correct numerical results but inconsistent purchasing classifications and repeated information | Accurate calculations alone do not guarantee clear operational recommendations |
| v1.1 | Added eligibility rules, purchasing classifications, FEFO terminology and concise reporting | Awaiting retesting | Pending evaluation |

---

## 3. Version v1.0 — Initial Prompt

Development and testing dates: [Actual dates]

### Observed Strengths

- Correct inventory and replenishment calculations.
- Correct conversion of grams into kilograms.
- Appropriate exclusion of expired inventory.
- Appropriate handling of missing expiry information.
- Recognition of stock expiring before planned usage.
- Identification of shortages and excess inventory.
- Human verification and purchasing approval.

### Observed Weaknesses

- Incorrect FEFO terminology.
- Inconsistent description of provisional shortages.
- Combined purchasing total without separate
  established and provisional subtotals.
- Subjective risk classifications.
- Lengthy reports with repeated information.

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

AI can perform correct inventory calculations
while presenting purchasing recommendations
that require greater classification clarity.

Explicit stock eligibility rules and purchasing
decision boundaries can improve business
usability and responsible AI behaviour.

---

## 4. Version v1.1 — Revised Prompt

Development date: [Actual date]

### Changes Made

- Added explicit inventory eligibility categories.
- Standardised measurement unit validation.
- Defined established and provisional purchasing
  requirements.
- Required separate purchasing subtotals.
- Corrected FEFO terminology.
- Strengthened food safety decision boundaries.
- Introduced a concise five-section report.

### Reason for Changes

The changes address observed weaknesses in
purchasing classification, terminology and
reporting efficiency.

### Expected Effect

The revised prompt is expected to retain
numerical accuracy while improving purchasing
clarity, stock eligibility assessment and
management usability.

This expected effect remains unverified.

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
| v1.0 | 9/10 | 8/10 | 17/20 (85%) |
| v1.1 | Pending | Pending | Pending |

## 6. Current Development Status

v1.0 testing and evaluation are complete.

Version v1.1 has been developed based on the
observed limitations.

Final retesting remains pending.

## Related Evidence

- [P02 Current Prompt](../02-prompt-library/P02-inventory-and-replenishment.md)
- [P02 Testing Evidence](../03-testing-evidence/P02-testing-evidence.md)
