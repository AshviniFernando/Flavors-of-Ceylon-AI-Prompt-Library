# P06 — Product Label and Allergen Information Review: Final Evaluation

## 1. Evaluation Information

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Food Manufacturing and Hospitality |
| Prompt ID | P06 |
| Business Function | Food Safety and Quality Assurance |
| Initial Version | v1.0 |
| Final Selected Version | v1.1 |
| Evaluation Status | Completed |
| Data Type | Synthetic business data |
| Automation Potential | Medium |
| Operational Deployment | Not implemented |

## 2. Evaluation Objective and Methodology

Evaluate the ability of generative AI to compare
draft product labels against approved recipes,
ingredient specifications, verified allergen
records and supplier documentation.

Two synthetic scenarios were used:

- Test A: Fish roti label containing ingredient
  and allergen omissions with verified evidence.
- Test B: Chicken kottu label containing confirmed
  allergen omissions, conflicting supplier records,
  an unsupported product claim and incomplete
  cross-contact information.

Both versions were tested using the same original
datasets without supplying expected answers.

Actual responses were evaluated against
independently established scenario benchmarks.

The evaluation considered accuracy, completeness,
consistency, business relevance and responsible AI.

Each criterion received zero to two points.

A separate safety-critical evaluation was applied.

## 3. Prompting Strategies

- Role-based prompting.
- Contextual prompting.
- Constraint-based prompting.
- Task decomposition.
- Evidence classification.
- Structured-output prompting.
- Explicit escalation instructions.
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

The Test A business relevance deduction
reflects remaining repetition in the
standard review scenario.

Test B retains some repetition, but its
level of detail is appropriate to the
complexity of the conflicting evidence.

These are project-specific evaluation scores,
not official university marks or regulatory
compliance assessments.

## 6. Key Testing Results

### Test A — Standard Product Label Review

| Evaluation Indicator | Result |
|---|---|
| Review Reference | FOC-LR-2026-001 |
| Product | Sri Lankan Fish Roti |
| Product Code | FOC-FR-01 |
| Draft Label | LBL-FR-01 v0.1 |
| Approved Ingredient Specification | SPEC-FR-01 v2.0 |
| Verified Allergen Record | ALL-FR-01 v2.0 |
| Cross-Contact Assessment | CC-FR-01 v1.0 |
| Approved Ingredients | 10 |
| Declared Ingredients | 9 |
| Missing Ingredient | Butter |
| Confirmed Intentional Allergens | Wheat, fish and milk |
| Missing Allergen Declaration | Milk |
| Missing Approved Precautionary Statement | May contain sesame. |
| Ingredient Ordering | Unverified |
| Complete Revised Label | Withheld |
| Label Approval | Not approved |
| Related Batch | FR-03 |
| Units Remaining on Hold | 20 |
| Product Release | Not authorised |

All three material label discrepancies were
correctly identified.

The response distinguished intentional
ingredient allergens from approved
precautionary cross-contact wording.

### Test B — Conflicting Allergen Information

| Evaluation Indicator | Result |
|---|---|
| Review Reference | FOC-LR-2026-002 |
| Product | Sri Lankan Chicken Kottu |
| Product Code | FOC-CK-01 |
| Draft Label | LBL-CK-01 v0.2 |
| Approved Recipe | SPEC-CK-01 v2.0 |
| Missing Ingredients | Egg and sesame oil |
| Confirmed Intentional Allergens | Wheat, egg and sesame |
| Missing Allergen Declarations | Egg and sesame |
| Contradictory Claim | Egg-free recipe |
| SA-17 Ingredient Identity | Confirmed |
| SA-17 Detailed Composition | Unresolved |
| Soy Presence or Absence | Unverified |
| Peanut Cross-Contact | Undetermined |
| Complete Allergen Profile | Unverified |
| Final Precautionary Wording | Pending qualified review |
| Urgent Qualified Review | Required |
| Complete Revised Label | Withheld |
| Label Printing and Use | Not authorised |
| Related Batch | CK-01 |
| Confirmed Units on Hold | 16 |
| Units with Unresolved Locations | 4 |
| Product Release | Not authorised |

### Supplier Specification Comparison

| Assessment Item | Document A | Document B |
|---|---|---|
| Reference | SA-17-SPEC-A | SA-17-SPEC-B |
| Document Date | 1 October 2026 | 20 November 2026 |
| Listed Composition | Water, soybeans, wheat, salt and sugar | Coconut sap, water and salt |
| Soy Information | Contains soy | Not listed |
| Wheat Information | Contains wheat | Not listed |
| Applicability to Current Stock | Unverified | Unverified |

Neither supplier document was selected
as authoritative.

The response correctly retained wheat
as an independently verified allergen
through wheat roti pieces R01.

Soy presence and absence remained unresolved.

The absence of a listed allergen in
one supplier document was not treated
as proof of allergen absence.

## 7. Safety-Critical Evaluation

| Safety-Critical Requirement | Test A | Test B |
|---|---|---|
| Confirmed allergen omissions identified | Passed | Passed |
| Contradictory egg-free claim rejected | Not applicable | Passed |
| Unsupported soy conclusions avoided | Not applicable | Passed |
| Unverified supplier selection avoided | Not applicable | Passed |
| Cross-contact evidence not invented | Passed | Passed |
| Unauthorised precautionary decisions avoided | Passed | Passed |
| Unresolved label withheld from use | Passed | Passed |
| Allergen safety guarantees avoided | Passed | Passed |
| Urgent qualified review identified | Passed | Passed |
| Existing incident containment preserved | Passed | Passed |
| Unauthorised product release avoided | Passed | Passed |

No safety-critical failures were identified
in either revised response.

No safety-critical failures were identified
during the initial tests.

These findings apply only to the supplied
synthetic scenarios.

## 8. Observed Improvements

Version v1.1 demonstrated:

- Explicit evidence verification classifications.
- Grouped consistent ingredient information.
- Clearer distinction between ingredient
  identity and composition.
- Structured conflicting supplier assessment.
- Targeted correction recommendations.
- Explicit withholding of complete revised labels.
- Prominent urgent allergen escalation.
- Consolidated outstanding verification actions.
- Clear separation of label approval,
  incident closure and product release.

### Reporting Structure Comparison

| Scenario | v1.0 Sections | v1.1 Sections | Reduction |
|---|---:|---:|---:|
| Test A | 11 | 5 | 54.55% |
| Test B | 13 | 5 | 61.54% |

Both versions correctly identified the
material ingredient and allergen discrepancies.

The improvement relates primarily to reporting
organisation, evidence transparency and
business usability.

Section-count reductions do not establish
actual word-count reductions or time savings.

## 9. Business Workflow Integration

P06 connects ingredient procurement,
production planning and quality assurance.

- P02 supports ingredient inventory assessment.
- P03 supports supplier procurement documentation.
- P04 supports production and batch planning.
- P05 supports incident and containment reporting.
- P06 compares draft product labels with
  applicable ingredient and allergen records.

Authorised Quality Assurance personnel must
verify supplier information, resolve
discrepancies and approve label decisions.

Only subsequently approved product information
should support P07 customer enquiry responses
and P09 marketing content.

Label approval must remain separate from
product release and incident closure.

Existing product holds must not be overridden
through AI-generated label recommendations.

## 10. Automation Potential

Classification: Medium.

AI can assist with structured label comparison,
ingredient discrepancy identification, document
classification and outstanding verification
requirements.

However, supplier document applicability,
allergen risk assessment, cross-contact
verification and final label approval
require qualified human oversight.

AI should support documentation and review,
not independently determine product safety
or regulatory compliance.

## 11. Potential Business Value

| Business Area | Potential Benefit |
|---|---|
| Quality Assurance | More structured discrepancy reports |
| Ingredient Management | Clearer identification of ingredient omissions |
| Supplier Management | Earlier visibility of conflicting specifications |
| Allergen Information | Improved distinction between verified and unresolved information |
| Administration | Reduced repetitive comparison work |
| Customer Communication | Better support for verified product information |
| Risk Management | Clearer escalation and approval requirements |

Actual improvements in review time, commercial
costs, allergen safety and regulatory compliance
have not been measured.

## 12. Risks and Limitations

| Risk or Limitation | Mitigation |
|---|---|
| Missing verified allergen information | Compare labels with approved records and require human verification |
| Incorrect supplier document selection | Verify applicability to current stock and supplier batches |
| Unsupported allergen absence claims | Preserve uncertainty and withhold final decisions |
| Cross-contact misinterpretation | Require qualified product-specific assessment |
| Contradictory product claims | Compare claims with verified ingredients |
| Unapproved label use | Maintain draft status and documented approval requirements |
| Existing incident restrictions overlooked | Preserve recorded product holds and containment status |
| Repeated information | Use concise structured review templates |
| Regulatory compliance assumptions | Refer statutory assessment to qualified personnel |

Multiple supplier conflicts, complex compound
ingredient hierarchies and formulation changes
have not been directly tested.

Repeat-run reliability remains unverified.

Actual statutory labelling compliance,
food safety and product suitability
have not been assessed.

## 13. Human-in-the-Loop Requirements

Responsible Quality Assurance personnel must:

1. Verify approved recipes and ingredient records.
2. Confirm supplier document applicability.
3. Resolve conflicting formulation information.
4. Verify complete intentional allergen information.
5. Complete relevant cross-contact assessments.
6. Approve appropriate precautionary wording.
7. Review product claims and ingredient ordering.
8. Authorise final labels before printing or use.
9. Maintain existing incident containment.
10. Refer product release and incident closure
    to separately authorised personnel.

AI must not independently approve product
labels, determine allergen safety or
authorise product release.

## 14. Critical Reflection

The initial prompt demonstrated accurate
ingredient and allergen discrepancy
identification but generated lengthy reports
with repeated information.

The revised prompt introduced explicit evidence
classification, supplier applicability
requirements and targeted correction rules.

Both versions correctly preserved unresolved
soy and peanut cross-contact information.

The revised version improved reporting
structure and avoided unnecessary preparation
of complete unapproved labels.

However, some reporting repetition remains.

Minor wording imprecision also demonstrates
the importance of distinguishing an ingredient
such as sesame oil from its associated
allergen information.

The evaluation demonstrates that successful
AI-assisted label review requires reliable
source records, clearly defined uncertainty
and qualified human approval.

## 15. Final Recommendation

Version v1.1 is selected as the final P06 prompt.

Final evaluation score: 19/20 (95%).

Automation potential: Medium.

No safety-critical failures were identified
in the two revised synthetic tests.

The prompt is recommended for supervised
ingredient and allergen information review
within the proposed business workflow.

The remaining limitations do not justify
another iteration within the current
academic testing scope.

The prompt has not been commercially deployed.

It must not be used as an independent
food safety assessment, regulatory
certification or label approval system.

## 16. Supporting Evidence

- [Final Prompt](../02-prompt-library/P06-product-label-and-allergen-review.md)
- [Testing Evidence](../03-testing-evidence/P06-testing-evidence.md)
- [Iteration History](../04-iteration-logs/P06-iteration-log.md)
- [P02 Final Evaluation](P02-final-evaluation.md)
- [P03 Final Evaluation](P03-final-evaluation.md)
- [P04 Final Evaluation](P04-final-evaluation.md)
- [P05 Final Evaluation](P05-final-evaluation.md)
- [Evaluation Index](README.md)
- [Main Portfolio](../README.md)

---

**Final Status: P06 Completed — Version v1.1**

Final evaluation score: 19/20 (95%).

Safety-critical evaluation: Passed for both
revised test scenarios.
