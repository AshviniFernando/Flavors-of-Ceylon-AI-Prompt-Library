# P04 — Food Production and Batch Planning: Iteration Log

## 1. Development Objective

Improve AI-assisted production planning, batch
allocation, ingredient resource management and
operational scheduling for Flavors of Ceylon.

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial production planning prompt | Correct calculations but excessive reporting; 90% score | Numerical accuracy must be supported by practical reporting |
| v1.1 | Added allocation rules, daily scheduling validation, consolidated inventory reconciliation and structured reporting | Improved document organisation while retaining numerical accuracy; 95% score | Explicit constraints and structured outputs improve operational decision support |

---

## 3. Version v1.0 — Initial Prompt

Development and testing dates: [Actual dates]

### Observed Strengths

- Correct Test A production allocation of 325 units.
- Correct allocation of 15 batches and 625 minutes.
- Correct Test B production allocation of 185 units.
- Correct allocation of nine batches and 370 minutes.
- Correct ingredient consumption and remaining stock.
- Appropriate shared ingredient allocation.
- Correct production priority allocation.
- Appropriate exclusion of unconfirmed deliveries.
- Correct staffing and capacity assessments.
- No overlapping production batches.
- Appropriate human approval safeguards.

### Observed Weaknesses

- Thirteen-section and eighteen-section reports.
- Repeated calculations and management summaries.
- Unrequested visualisations and timelines.
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

### Lesson Learned

Accurate production calculations should be
supported by concise scheduling information,
clear resource limitations and appropriate
operational decision boundaries.

---

## 4. Version v1.1 — Revised Prompt

Development and testing dates: [Actual dates]

### Changes Made

- Added explicit production data validation.
- Standardised ingredient requirement calculations.
- Defined priority-based resource allocation.
- Required shared ingredient reconciliation.
- Strengthened daily batch scheduling validation.
- Distinguished theoretical and feasible capacity.
- Separated full-target shortages from scheduled
  ingredient consumption.
- Introduced a five-section reporting structure.
- Prohibited unsupported risk classifications.
- Removed unnecessary charts and self-assessment.

### Reason for Changes

The revised prompt aimed to retain numerical
accuracy and responsible production behaviour
while improving reporting efficiency and
operational usability.

### Expected Effect

More structured production schedules, transparent
resource calculations and concise management
recommendations without reducing accuracy.

### Observed Effect

Test A correctly achieved 325 production units
through 15 batches using 625 minutes.

Test B correctly achieved 185 production units
through nine batches using 370 minutes.

The 140-unit production shortfall and 56.92%
target achievement were calculated correctly.

Both responses correctly reconciled ingredient
requirements, scheduled consumption and
remaining inventory.

Unconfirmed supplier deliveries and provisional
purchases remained excluded.

Principal report sections decreased from 13
to five in Test A and from 18 to five in Test B.

Unsupported risk classifications and unnecessary
visualisations were removed.

The five-section structure improved organisation,
although some repeated information remained.

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

- Some repeated production calculations remain.
- Actual administrative time savings have not
  been measured.
- Multiple production stations have not been tested.
- Complex employee qualification and shift
  restrictions have not been tested.
- Invalid recipes and missing essential production
  information have not been directly tested.
- Unexpected equipment failures and dynamic
  rescheduling have not been tested.
- Repeat-run reliability remains unverified.
- Actual manufacturing feasibility and food safety
  require appropriate human verification.

### Lesson Learned

Explicit resource allocation and reconciliation
rules improve the transparency of AI-assisted
production planning.

Distinguishing available station time from
staff-supported feasible production time is
important for realistic scheduling.

Prompt refinement can improve document structure
without changing the underlying numerical results.

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

The revised version retains correct numerical
calculations and responsible operational safeguards
while improving reporting structure and resource
allocation transparency.

The remaining reporting repetition does not justify
another iteration within the current academic scope.

Automation potential: Medium.

Development status: Completed.

Operational deployment: Not implemented.

## Related Evidence

- [P04 Final Prompt](../02-prompt-library/P04-production-and-batch-planning.md)
- [P04 Testing Evidence](../03-testing-evidence/P04-testing-evidence.md)
- [P04 Final Evaluation](../05-evaluation/P04-final-evaluation.md)
- [P01 Final Evaluation](../05-evaluation/P01-final-evaluation.md)
- [P02 Final Evaluation](../05-evaluation/P02-final-evaluation.md)
- [P03 Final Evaluation](../05-evaluation/P03-final-evaluation.md)
- [Iteration Log Index](README.md)
