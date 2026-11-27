# P07 — Customer Enquiry Response: Iteration Log

## 1. Development Objective

Improve AI-assisted customer communication,
pricing accuracy, product availability reporting,
ordering and delivery information handling,
allergen enquiry management and responsible
customer service decision support for
Flavors of Ceylon.

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial customer enquiry response prompt | Accurate responses and responsible allergen handling but excessive reporting; 90% score | Customer service automation must prioritise usable customer communication |
| v1.1 | Added customer-first reporting, approved-information controls, concise verification notes and explicit escalation boundaries | Awaiting retesting | Pending evaluation |

---

## 3. Version v1.0 — Initial Prompt

Development and testing dates: [Actual dates]

### Observed Strengths

Test A:

- Correct product names and pack sizes.
- Correct calculation of 12 vegetable rolls
  and 10 pol sambol sachets.
- Correct product subtotal of AUD 38.00.
- Correct delivery charge of AUD 8.00.
- Correct estimated total of AUD 46.00.
- Correct minimum order assessment.
- Accurate delivery date, window and deadline.
- Appropriate ordering and payment instructions.
- Clear distinction between availability,
  reservation and confirmed order acceptance.
- Friendly Australian English communication.

Test B:

- Correct communication that chicken kottu
  contains egg and is not egg-free.
- Accurate confirmed wheat and sesame information.
- Appropriate preservation of unresolved
  soy and peanut cross-contact information.
- No unsupported allergy-safe alternative.
- Correct indicative listed value of AUD 56.00.
- Preservation of active ordering restrictions.
- No invented delivery or restocking commitments.
- Appropriate separation of internal and
  customer-facing information.
- Preservation of P05 containment requirements.
- Preservation of P06 allergen restrictions.
- Qualified review requirements maintained.

Both responses remained drafts requiring
human approval.

### Observed Weaknesses

- Ten numbered principal sections in both tests.
- Repeated product and pricing assessments.
- Repeated stock and delivery information.
- Extensive internal verification reports.
- Overlapping human approval checklists.
- An unnecessary AI-generated PASS checklist
  in Test B.
- Suggested formal priority categories without
  a supplied classification framework.
- Test B could provide a more actionable
  qualified review pathway for the customer.
- Minor internal wording imprecision concerning
  sesame oil, although the subsequent recipe
  entry correctly identified the ingredient.

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

Test A: No failures identified.

Test B: No failures identified.

Both responses maintained appropriate ordering,
allergen communication and human approval
boundaries.

### Lesson Learned

Accurate customer service responses should be
easy for staff to review and appropriate
for direct customer communication.

Detailed internal management reports are
unnecessary for routine customer enquiries.

Sensitive allergen enquiries require clear
uncertainty handling, appropriate escalation
and separation of internal operational data.

---

## 4. Version v1.1 — Revised Prompt

Development date: [Actual date]

### Changes Made

- Prioritised the customer-facing email draft.
- Introduced a three-section output structure.
- Added approved customer-information
  validation rules.
- Standardised price and quantity calculations.
- Clarified GST and minimum order requirements.
- Strengthened stock reservation and order
  acceptance boundaries.
- Strengthened delivery confirmation rules.
- Added actionable customer next steps.
- Preserved unresolved allergen information.
- Clarified internal information restrictions.
- Consolidated verification and escalation notes.
- Added an approximate 150-250-word target
  for the customer-facing email, with flexibility
  for essential safety information.
- Introduced a target of no more than six
  grouped internal follow-up actions.
- Removed repeated approval checklists.
- Prohibited AI-generated self-assessments.

### Reason for Changes

The initial prompt successfully answered
the customer enquiries but produced extensive
internal reporting.

The revised prompt aims to improve practical
customer service usability while retaining
accurate information, appropriate escalation
and responsible operational safeguards.

The additional safeguards are preventive
improvements rather than responses to
observed safety-critical failures.

### Expected Effect

The revised prompt is expected to generate
concise customer-facing email drafts with
accurate prices, clear availability information,
appropriate allergen communication and
practical next steps.

Internal verification requirements are
expected to be grouped into a shorter
separate section.

Human approval and operational restrictions
are expected to remain intact.

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
|---|---:|---:|---|
| v1.0 | 9/10 | 9/10 | 18/20 (90%) |
| v1.1 | Pending | Pending | Pending |

## 6. Current Development Status

Initial v1.0 testing and evaluation are complete.

Both original testing responses are available.

No safety-critical failures were identified
during initial testing.

Version v1.1 has been developed based on
observed reporting limitations and preventive
customer communication safeguards.

Final retesting remains pending.

Automation potential: High — Preliminary,
for supervised customer response preparation.

Sensitive allergen enquiries and operational
commitments remain subject to human review.

Operational deployment: Not implemented.

## Related Evidence

- [P07 Current Prompt](../02-prompt-library/P07-customer-enquiry-response.md)
- [P07 Testing Evidence](../03-testing-evidence/P07-testing-evidence.md)
- [P04 Final Evaluation](../05-evaluation/P04-final-evaluation.md)
- [P05 Final Evaluation](../05-evaluation/P05-final-evaluation.md)
- [P06 Final Evaluation](../05-evaluation/P06-final-evaluation.md)
