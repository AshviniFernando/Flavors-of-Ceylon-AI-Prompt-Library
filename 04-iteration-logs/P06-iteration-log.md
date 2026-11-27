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
| v1.0 | Initial product label and allergen review prompt | Correct discrepancy identification but excessive reporting; 90% score | Accurate allergen reviews must support efficient human verification |
| v1.1 | Added evidence classification, supplier applicability rules, targeted corrections and structured reporting | Clearer evidence handling and reporting structure; 95% score | Explicit evidence classifications and authorisation boundaries improve responsible label review |

---

## 3. Version v1.0 — Initial Prompt

Development and testing dates: [Actual dates]

### Observed Strengths

Test A:

- Correct identification of missing butter.
- Correct identification of missing milk.
- Correct preservation of wheat and fish.
- Correct identification of omitted approved
  sesame precautionary wording.
- Appropriate separation of intentional
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

### Observed Weaknesses

- Eleven-section and thirteen-section reports.
- Repeated ingredient and allergen comparisons.
- Repeated supplier verification findings.
- Overlapping recommendations and checklists.
- Unnecessary qualitative priority ratings.
- Unnecessary P05 incident calculations.
- Preparation of a complete proposed label
  in Test A despite unverified ingredient
  ordering.

The proposed Test A label was clearly marked
as unapproved. This represented a reporting
and usability limitation rather than a
safety-critical failure.

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

No safety-critical failures were identified
in either initial response.

### Lesson Learned

Accurate product label reviews require clear
distinctions between verified information,
conflicting evidence and unresolved allergens.

Targeted discrepancy reports are preferable
to unnecessary preparation of complete
unapproved labels.

---

## 4. Version v1.1 — Revised Prompt

Development and testing dates: [Actual dates]

### Changes Made

- Added explicit evidence classification.
- Distinguished ingredient identity from
  detailed ingredient composition.
- Standardised ingredient and product
  claim discrepancy reporting.
- Strengthened supplier document
  applicability requirements.
- Separated confirmed intentional allergens
  from unresolved allergen information.
- Separated approved precautionary wording
  from unresolved cross-contact information.
- Required targeted correction recommendations.
- Prohibited complete revised product labels.
- Strengthened urgent allergen escalation.
- Consolidated outstanding verification actions.
- Preserved related incident and hold information.
- Introduced a five-section report structure.
- Prohibited unnecessary calculations and
  unsupported priority classifications.

### Reason for Changes

The revised prompt aimed to retain accurate
ingredient and allergen review behaviour
while improving evidence transparency,
reporting efficiency and operational usability.

The additional safeguards were preventive
improvements rather than responses to
observed safety-critical failures.

### Expected Effect

More concise discrepancy reports with clear
evidence classifications, targeted corrections
and consolidated verification requirements.

Existing allergen safeguards and qualified
human authorisation requirements were
expected to remain intact.

### Observed Effect

Test A correctly identified all three
material label discrepancies:

- Missing butter ingredient.
- Missing milk allergen declaration.
- Missing approved sesame precautionary wording.

The existing hold on all 20 units of batch
FR-03 was preserved.

Test B correctly identified missing egg and
sesame oil ingredients, missing egg and sesame
allergen declarations and the contradictory
egg-free claim.

Conflicting supplier records remained
unresolved pending applicable verification.

Soy presence and absence remained unverified.

Peanut cross-contact remained undetermined.

Both revised responses withheld complete
revised product labels and prominently
identified urgent qualified review.

The existing P05 containment requirements
were preserved.

Numbered principal report sections decreased
from 11 to five in Test A and from 13 to five
in Test B.

Unsupported risk classifications, unnecessary
incident calculations and overlapping
verification checklists were removed.

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

### Safety-Critical Assessment

No safety-critical failures were identified
in either revised response.

Both responses maintained qualified human
review and avoided unauthorised label,
product disposition or release decisions.

### Remaining Limitations

- Some repeated findings and approval
  information remain.
- Test B contains minor introductory wording
  imprecision concerning sesame oil.
- Actual label review time savings have
  not been measured.
- Multiple simultaneous supplier conflicts
  have not been directly tested.
- Changes in approved recipes and complex
  compound ingredient hierarchies remain untested.
- Actual regulatory labelling compliance
  has not been assessed.
- Repeat-run reliability remains unverified.
- Qualified allergen and food safety review
  remains necessary.

### Lesson Learned

An approved ingredient identity does not
necessarily establish verified composition
or a complete allergen profile.

Supplier document dates alone do not establish
applicability to current ingredient stock.

Intentional allergens and potential
cross-contact information must remain separate.

Prompt refinement can improve evidence
classification and reporting structure
without changing correct factual findings.

Label approval, incident closure and
product release require separate
authorised human decisions.

---

## 5. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 9/10 | 18/20 (90%) |
| v1.1 | 9/10 | 10/10 | 19/20 (95%) |

Absolute improvement: 5 percentage points.

Relative improvement in evaluation score: 5.56%.

### Reporting Structure

| Scenario | Initial Sections | Final Sections | Reduction |
|---|---:|---:|---:|
| Test A | 11 | 5 | 54.55% |
| Test B | 13 | 5 | 61.54% |

Section reductions do not establish measured
administrative time savings.

## 6. Final Version Selection

Version v1.1 is selected as the final prompt.

The revised version maintains accurate
ingredient and allergen review behaviour
while improving evidence classification,
reporting structure and authorisation boundaries.

No safety-critical failures were identified
in either revised test.

The remaining minor reporting limitations
do not justify further iteration within
the current academic scope.

Automation potential: Medium.

Development status: Completed.

Operational deployment: Not implemented.

## Related Evidence

- [P06 Final Prompt](../02-prompt-library/P06-product-label-and-allergen-review.md)
- [P06 Testing Evidence](../03-testing-evidence/P06-testing-evidence.md)
- [P06 Final Evaluation](../05-evaluation/P06-final-evaluation.md)
- [P04 Final Evaluation](../05-evaluation/P04-final-evaluation.md)
- [P05 Final Evaluation](../05-evaluation/P05-final-evaluation.md)
- [Iteration Log Index](README.md)
