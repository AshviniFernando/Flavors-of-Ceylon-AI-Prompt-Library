# P04 — Food Production and Batch Planning: Iteration Log

## 1. Development Objective

Improve AI-assisted production planning, batch
allocation, ingredient resource management and
operational scheduling for Flavors of Ceylon.

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial production planning prompt | Correct production and resource calculations, but excessive reporting; 90% score | Numerical accuracy must be supported by practical management reporting |
| v1.1 | Added explicit allocation rules, daily scheduling validation and concise reporting | Awaiting retesting | Pending evaluation |

---

## 3. Version v1.0 — Initial Prompt

Development and testing dates: [Actual dates]

### Observed Strengths

- Correct Test A production allocation of 325 units.
- Correct allocation of 15 batches and 625 minutes.
- Correct Test B production allocation of 185 units.
- Correct allocation of nine batches and 370 minutes.
- Correct ingredient consumption and remaining stock.
- Appropriate handling of shared ingredient resources.
- Correct production priority allocation.
- Appropriate exclusion of unconfirmed deliveries.
- Correct staffing and production capacity assessment.
- No overlapping batches or unauthorised production.
- Appropriate human approval safeguards.

### Observed Weaknesses

- Thirteen-section and eighteen-section reports.
- Repeated calculations and management summaries.
- Unrequested visualisations and production timelines.
- Illustrative inventory utilisation thresholds.
- Qualitative risk ratings without approved rules.
- Unnecessary AI-generated compliance assessments.

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

Business relevance deductions reflect reporting
length and repetition rather than numerical errors.

### Lesson Learned

Correct production calculations must be supported
by concise scheduling information and clearly
defined operational decision boundaries.

---

## 4. Version v1.1 — Revised Prompt

Development date: [Actual date]

### Changes Made

- Added explicit production data validation.
- Standardised ingredient requirement calculations.
- Defined priority-based resource allocation.
- Required shared ingredient stock reconciliation.
- Strengthened daily batch scheduling validation.
- Distinguished theoretical capacity from feasible
  daily production capacity.
- Separated full-target shortages from actual
  scheduled ingredient consumption.
- Introduced a five-section reporting structure.
- Prohibited unsupported risk classifications.
- Removed unnecessary charts and self-assessment.

### Reason for Changes

Initial testing demonstrated correct numerical
calculations and responsible production planning.

The revised prompt aims to preserve these strengths
while improving reporting efficiency, allocation
transparency and operational usability.

### Expected Effect

The revised prompt is expected to produce more
structured production schedules, transparent
resource calculations and concise management
recommendations without reducing accuracy.

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
| v1.0 | 9/10 | 9/10 | 18/20 (90%) |
| v1.1 | Pending | Pending | Pending |

## 6. Current Development Status

Initial v1.0 testing and evaluation are complete.

Version v1.1 has been developed based on observed
reporting and usability limitations.

Final retesting remains pending.

Automation potential: Medium — Preliminary.

Operational deployment: Not implemented.

## Related Evidence

- [P04 Current Prompt](../02-prompt-library/P04-production-and-batch-planning.md)
- [P04 Testing Evidence](../03-testing-evidence/P04-testing-evidence.md)
- [P01 Final Evaluation](../05-evaluation/P01-final-evaluation.md)
- [P02 Final Evaluation](../05-evaluation/P02-final-evaluation.md)
- [P03 Final Evaluation](../05-evaluation/P03-final-evaluation.md)
