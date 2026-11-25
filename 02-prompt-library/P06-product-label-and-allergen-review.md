# P06 — Product Label and Allergen Information Review

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Business Function | Product Quality |
| Workflow | Food Safety and Product Quality |
| Current Version | v1.0 |
| Status | Initial Draft — Not Yet Tested |
| Prompting Strategy | Contextual and constraint-based prompting |

---

## 1. Prompt Text

> You are a product information review assistant
> for Flavors of Ceylon.
>
> Compare the supplied draft product label with
> the approved ingredient specifications and
> verified allergen information.
>
> Identify missing ingredients, inconsistencies,
> unclear statements and information requiring
> further verification.
>
> Present the findings in a table showing the
> label information, supplied evidence, identified
> issue and recommended review action.
>
> Do not invent ingredient information, allergen
> declarations or cross-contact information.
>
> Do not guarantee allergen safety or certify
> regulatory compliance. The draft must be reviewed
> by appropriate quality assurance personnel.

## 2. Intended Workflow or Task

This prompt supports preliminary product label review.

- Trigger: A new or updated product label is prepared.
- Input: Draft label and verified product specifications.
- Output: List of discrepancies and verification requirements.
- Responsible person: Quality assurance officer.
- Next step: Qualified review before label approval.

## 3. Problem Being Solved

Manual product information reviews may overlook
ingredient inconsistencies, incomplete declarations
and other labelling errors.

## 4. Automation Potential

Level: Medium — Preliminary assessment.

AI can assist with comparing supplied documents
and identifying inconsistencies. Final product
labelling decisions require qualified human review.

## 5. Risks and Limitations

| Risk | Mitigation |
|---|---|
| Incorrect allergen information | Verify approved specifications |
| Missing cross-contact data | Flag for further investigation |
| Outdated regulatory information | Consult current official guidance |
| False compliance assurance | Prohibit AI-only label approval |

AI must not guarantee that a product is allergen-free
or suitable for customers with particular allergies.

---

## Version History

| Version | Change | Status |
|---|---|---|
| v1.0 | Initial prompt development | Not yet tested |

## Testing Evidence

Pending practical testing in Stage 04.
