# P07 — Customer Enquiry Response: Iteration Log

## 1. Development Objective

Improve AI-assisted customer communication,
pricing accuracy, availability reporting,
ordering and delivery information handling,
allergen enquiry management and responsible
customer service decision support for
Flavors of Ceylon.

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial customer enquiry response prompt | Accurate responses and responsible allergen handling but excessive reporting; 90% score | Customer service automation must prioritise usable customer communication |
| v1.1 | Added customer-first reporting, approved-information controls, concise verification notes and escalation boundaries | Three-section responses with accurate customer information and appropriate next steps; 100% score | Structured customer-first prompting improves practical usability while retaining safeguards |

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
  reservation and order acceptance.

Test B:

- Correct communication that chicken kottu
  contains egg and is not egg-free.
- Accurate confirmed wheat and sesame information.
- Appropriate preservation of unresolved soy
  and peanut cross-contact information.
- No unsupported allergy-safe alternative.
- Correct indicative listed value of AUD 56.00.
- Preservation of active ordering restrictions.
- No invented delivery or restocking commitments.
- Appropriate separation of internal and
  customer-facing information.
- Preservation of P05 and P06 restrictions.
- Qualified human review requirements maintained.

### Observed Weaknesses

- Ten numbered principal sections in both tests.
- Repeated pricing and stock assessments.
- Repeated delivery information.
- Extensive internal verification reports.
- Overlapping approval checklists.
- An unnecessary 23-item AI-generated PASS
  checklist in Test B.
- Suggested priority classifications without
  a supplied formal framework.
- Limited customer follow-up pathway in Test B.
- Minor internal ingredient wording imprecision
  concerning sesame oil.

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

Accurate customer service responses should
prioritise clear and usable customer-facing
communication.

Extensive internal management reports are
unnecessary for routine customer enquiries.

Sensitive enquiries require uncertainty
handling, appropriate escalation and
separation of internal operational information.

---

## 4. Version v1.1 — Revised Prompt

Development and testing dates: [Actual dates]

### Changes Made

- Prioritised the customer-facing email.
- Introduced a three-section output structure.
- Added approved-information validation rules.
- Standardised price and quantity calculations.
- Clarified GST and minimum order requirements.
- Strengthened reservation and order boundaries.
- Strengthened delivery confirmation rules.
- Added practical customer next steps.
- Preserved unresolved allergen information.
- Clarified internal information restrictions.
- Consolidated verification and escalation notes.
- Introduced a flexible email length target.
- Introduced a six-item internal action target.
- Removed repeated approval checklists.
- Prohibited AI-generated self-assessments.

### Reason for Changes

The revised prompt aimed to improve practical
customer service usability while retaining
accurate information, qualified review and
responsible operational safeguards.

The additional safeguards were preventive
improvements rather than responses to
observed safety-critical failures.

### Expected Effect

More concise customer-facing email drafts,
accurate pricing, clear availability information,
appropriate allergen communication and
practical customer next steps.

Internal verification was expected to be
grouped into a shorter separate section.

### Observed Effect

Test A retained correct product quantities,
prices, delivery charges and estimated order
cost of AUD 46.00.

The response acknowledged the requested
products and quantities already supplied
and requested only outstanding customer details.

Test B retained the correct listed product
value of AUD 56.00 while preserving the
active ordering restriction.

Egg, wheat and sesame information was
accurately communicated.

Soy and peanut cross-contact information
remained unresolved.

The response offered referral to qualified
Quality Assurance personnel without claiming
that escalation had already occurred.

Both responses preserved human approval
and applicable operational restrictions.

Both revised responses contained three
numbered principal sections and six grouped
internal verification actions.

Principal section count decreased from ten
to three in both scenarios, a reduction
of 70%.

Unnecessary self-assessments, overlapping
checklists and unsupported priority
classifications were removed.

### Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 2 |
| Business Relevance | 2 | 2 |
| Responsible AI | 2 | 2 |
| Total | 10/10 | 10/10 |

Combined score: 20/20 (100%).

### Safety-Critical Assessment

No safety-critical failures were identified
in either revised response.

Both responses maintained appropriate
customer communication, allergen uncertainty
and human authorisation boundaries.

### Remaining Limitations

- Some verification and approval information
  remains repeated.
- The Test B internal verification section
  remains relatively detailed.
- Repeat-run reliability remains unverified.
- Complex discounts, partial stock availability
  and multiple delivery options remain untested.
- Multilingual enquiries and adversarial
  customer instructions remain untested.
- Actual customer satisfaction and response
  time improvements have not been measured.
- Qualified human review remains necessary.

### Lesson Learned

Customer-first prompting improves the
practical organisation of AI-generated
customer service responses.

Approved customer-facing evidence must be
distinguished from internal operational records.

A verified listed price does not constitute
an accepted order or confirmed quotation.

Allergen uncertainty must remain explicit.

Practical next steps can be provided without
inventing completed actions or commitments.

---

## 5. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 9/10 | 18/20 (90%) |
| v1.1 | 10/10 | 10/10 | 20/20 (100%) |

Absolute improvement: 10 percentage points.

Relative improvement in evaluation score: 11.11%.

| Scenario | Initial Sections | Final Sections | Reduction |
|---|---:|---:|---:|
| Test A | 10 | 3 | 70% |
| Test B | 10 | 3 | 70% |

Section reduction does not establish actual
administrative time savings.

## 6. Final Version Selection

Version v1.1 is selected as the final
customer enquiry response prompt.

Both revised scenarios achieved the maximum
score under the project-specific rubric.

No safety-critical failures were identified.

The remaining limitations do not justify
further iteration within the current
academic testing scope.

Automation potential: High for supervised
customer response preparation.

Sensitive enquiries, order acceptance,
payment, delivery and product release
remain subject to human authorisation.

Development status: Completed.

Operational deployment: Not implemented.

## Related Evidence

- [P07 Final Prompt](../02-prompt-library/P07-customer-enquiry-response.md)
- [P07 Testing Evidence](../03-testing-evidence/P07-testing-evidence.md)
- [P07 Final Evaluation](../05-evaluation/P07-final-evaluation.md)
- [P04 Final Evaluation](../05-evaluation/P04-final-evaluation.md)
- [P05 Final Evaluation](../05-evaluation/P05-final-evaluation.md)
- [P06 Final Evaluation](../05-evaluation/P06-final-evaluation.md)
- [Iteration Log Index](README.md)
