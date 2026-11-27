# P06 — Product Label and Allergen Information Review: Iteration Log

## 1. Development Objective

Improve AI-assisted product label review,
ingredient discrepancy identification,
allergen evidence interpretation and
responsible Quality Assurance decision
support for Flavors of Ceylon.

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial product label and allergen review prompt | Correct discrepancy identification and responsible evidence handling, but excessive reporting; 90% score | Accurate allergen reviews must also support efficient human verification |
| v1.1 | Added evidence classification, supplier applicability rules, targeted corrections and structured reporting | Awaiting retesting | Pending evaluation |

---

## 3. Version v1.0 — Initial Prompt

Development and testing dates: [Actual dates]

### Observed Strengths

Test A:

- Correct identification of butter as the
  missing intentional ingredient.
- Correct identification of milk as the
  missing intentional allergen.
- Correct preservation of wheat and fish.
- Correct identification of omitted approved
  sesame precautionary wording.
- Correct distinction between intentional
  allergens and cross-contact information.
- Preservation of the quality hold on all
  20 units of batch FR-03.

Test B:

- Correct identification of missing egg
  and sesame oil ingredients.
- Correct identification of missing egg
  and sesame allergen declarations.
- Correct rejection of the egg-free claim.
- Accurate presentation of conflicting
  SA-17 supplier specifications.
- Appropriate preservation of unresolved
  soy allergen information.
- Correct handling of unverified peanut
  cross-contact information.
- Appropriate withholding of a complete
  revised product label.
- Urgent qualified review requirements.
- Preservation of unresolved P05 containment.

Both responses avoided unsupported food
safety conclusions and unauthorised label
or product release decisions.

### Observed Weaknesses

- Eleven-section and thirteen-section reports.
- Repeated ingredient and allergen comparisons.
- Repeated supplier verification findings.
- Overlapping recommendations and checklists.
- Unnecessary qualitative priority ratings.
- Unnecessary P05 incident percentage calculations.
- Preparation of a complete proposed label
  in Test A despite unverified ingredient
  ordering.

The proposed Test A label was clearly marked
as unapproved and its limitations were stated.

This was a reporting and usability limitation,
not an observed safety-critical failure.

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

### Safety-Critical Assessment

Test A: No safety-critical failures identified.

Test B: No safety-critical failures identified.

Both initial responses maintained appropriate
qualified human authorisation requirements.

### Lesson Learned

Accurate product label reviews require clear
distinctions between verified information,
conflicting evidence and unresolved
allergen information.

Concise discrepancy reports are preferable
to unnecessary preparation of complete
unapproved product labels.

---

## 4. Version v1.1 — Revised Prompt

Development date: [Actual date]

### Changes Made

- Added explicit evidence verification
  and classification rules.
- Distinguished ingredient identity from
  detailed ingredient composition.
- Standardised ingredient and product
  claim discrepancy reporting.
- Strengthened supplier document
  applicability requirements.
- Separated confirmed intentional allergens
  from unresolved ingredient allergens.
- Separated approved precautionary wording
  from unresolved cross-contact information.
- Required targeted correction recommendations.
- Prohibited complete revised product labels.
- Strengthened urgent allergen escalation.
- Consolidated outstanding verification actions.
- Preserved related incident and hold information.
- Introduced a five-section reporting structure.
- Prohibited unnecessary charts, calculations
  and unsupported priority classifications.

### Reason for Changes

The revised prompt aims to preserve accurate
ingredient and allergen review behaviour
while improving evidence transparency,
reporting efficiency and operational usability.

The additional safeguards reduce foreseeable
risks associated with incomplete ingredient
information and unapproved label drafts.

They do not establish that safety-critical
failures occurred during initial testing.

### Expected Effect

The revised prompt is expected to produce
more concise discrepancy reports with clear
evidence classifications, targeted corrections
and consolidated verification requirements.

Existing allergen safeguards and qualified
human authorisation requirements are expected
to remain intact.

These expected effects remain unverified.

### Observed Effect

Pending actual retesting.

### Evaluation Scores

Pending.

### Safety-Critical Assessment

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

Both original testing responses are available.

No safety-critical failures were identified
during initial testing.

Version v1.1 has been developed based on
observed reporting limitations and additional
preventive evidence-handling safeguards.

Final retesting remains pending.

Automation potential: Medium — Preliminary.

Operational deployment: Not implemented.

## Related Evidence

- [P06 Current Prompt](../02-prompt-library/P06-product-label-and-allergen-review.md)
- [P06 Testing Evidence](../03-testing-evidence/P06-testing-evidence.md)
- [P04 Final Evaluation](../05-evaluation/P04-final-evaluation.md)
- [P05 Final Evaluation](../05-evaluation/P05-final-evaluation.md)
