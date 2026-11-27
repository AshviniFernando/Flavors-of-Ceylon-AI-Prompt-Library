# P08 — Customer Complaint and Feedback Analysis: Final Evaluation

## 1. Evaluation Information

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Food Manufacturing and Hospitality |
| Prompt ID | P08 |
| Business Function | Customer Experience and Complaint Management |
| Initial Version | v1.0 |
| Final Selected Version | v1.1 |
| Evaluation Status | Completed |
| Data Type | Synthetic business data |
| Automation Potential | Medium |
| Operational Deployment | Not implemented |

## 2. Evaluation Objective and Methodology

Evaluate the ability of generative AI to classify
customer complaints, analyse customer sentiment,
identify recurring operational problems,
reconcile duplicate records and recommend
appropriate management actions.

Two synthetic scenarios were used:

- Test A: Standard feedback involving delivery,
  packaging, communication, positive observations
  and a refund request.
- Test B: Complex complaints involving reported
  illness, a possible allergen incident, suspected
  foreign material, duplicate communications,
  unresolved allergen information and refunds.

Both versions were tested using the same
original datasets without supplying expected answers.

Actual outputs were evaluated against predefined
scenario benchmarks.

The evaluation considered accuracy, completeness,
consistency, business relevance and responsible AI.

Each criterion received zero to two points.

A separate safety-critical evaluation was applied.

## 3. Prompting Strategies

- Role-based prompting.
- Contextual prompting.
- Classification-based prompting.
- Constraint-based prompting.
- Task decomposition.
- Structured-output prompting.
- Evidence-based reconciliation.
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

The Test A business relevance deduction reflects
remaining repetition within a routine feedback
analysis scenario.

Test B retains some repetition, but its level
of detail is proportionate to the investigation
and food safety requirements.

These are project-specific evaluation scores,
not official university marks.

## 6. Key Testing Results

### Test A — Standard Customer Feedback

| Evaluation Indicator | Result |
|---|---:|
| Submitted Feedback Records | 8 |
| Unique Feedback Cases | 8 |
| Confirmed Duplicate Communications | 0 |
| Cases Containing Complaints | 6 |
| Positive-only Cases | 2 |
| Recurring Primary Problem Categories | 3 |
| Urgent Qualified Review Cases | 0 |
| Standard Follow-up Cases | 6 |
| Unique Refund Requests | 1 |
| Known Requested Refund Subtotal | AUD 8.00 |
| Complete Requested Refund Total | AUD 8.00 |
| Authorised Refunds | 0 |

#### Primary Issue Distribution

| Primary Category | Unique Cases | Percentage |
|---|---:|---:|
| Delivery Delay | 2 | 25% |
| Outer Packaging and Presentation | 2 | 25% |
| Customer Communication | 2 | 25% |
| Positive-only Feedback | 2 | 25% |
| Other or Insufficient Information | 0 | 0% |
| Total | 8 | 100% |

#### Sentiment Distribution

| Sentiment | Unique Cases | Percentage |
|---|---:|---:|
| Positive | 2 | 25% |
| Negative | 4 | 50% |
| Mixed | 2 | 25% |
| Neutral or Unclear | 0 | 0% |
| Total | 8 | 100% |

All category and sentiment totals reconciled
correctly to eight unique cases.

Three recurring operational problems were
identified: delivery delays, outer packaging
damage and customer communication delays.

Positive observations were preserved within
mixed feedback.

No reported food safety concerns requiring
urgent qualified review were identified.

This does not establish product safety.

### Test B — Complex Customer Complaints

| Evaluation Indicator | Result |
|---|---:|
| Submitted Feedback Records | 9 |
| Confirmed Duplicate Communications | 2 |
| Unique Complaint Cases | 7 |
| Cases Containing Complaints | 7 |
| Positive-only Cases | 0 |
| Urgent Qualified Review Cases | 4 |
| Standard Follow-up Cases | 3 |
| Recurring Primary Problem Categories | 1 |
| Unique Refund Requests | 3 |
| Requests with Known Amounts | 1 |
| Requests with Unknown Amounts | 2 |
| Known Requested Refund Subtotal | AUD 8.00 |
| Complete Requested Refund Total | Undetermined |
| Authorised Refunds | 0 |

#### Duplicate Reconciliation

| Complaint Ticket | Original Record | Duplicate Communication |
|---|---|---|
| COMP-26001 | CFA-B01 | CFA-B02 |
| COMP-26004 | CFA-B05 | CFA-B06 |

Nine submitted communications minus two
confirmed duplicates resulted in seven
unique complaint cases.

All original record IDs were preserved.

Duplicate communications were not counted
as separate incidents or refund requests.

#### Primary Issue Distribution

| Primary Category | Unique Cases | Percentage |
|---|---:|---:|
| Reported Illness | 1 | 14.29% |
| Possible Allergen Incident | 1 | 14.29% |
| Suspected Foreign Material | 1 | 14.29% |
| Delivery Delay | 2 | 28.57% |
| Allergen Information Concern | 1 | 14.29% |
| Other or Insufficient Information | 1 | 14.29% |
| Positive-only Feedback | 0 | 0.00% |
| Total | 7 | 100.00% |

Individual rounded percentages sum to
100.02% because of rounding.

#### Sentiment Distribution

| Sentiment | Unique Cases | Percentage |
|---|---:|---:|
| Positive | 0 | 0.00% |
| Negative | 6 | 85.71% |
| Mixed | 1 | 14.29% |
| Neutral or Unclear | 0 | 0.00% |
| Total | 7 | 100.00% |

#### Handling Priority

| Suggested Priority | Unique Cases | Percentage |
|---|---:|---:|
| Urgent Qualified Review | 4 | 57.14% |
| Standard Follow-up | 3 | 42.86% |
| Total | 7 | 100.00% |

Delivery delay was the only recurring
primary issue category.

Allergen-related concerns and reported
symptoms were identified as overlapping
broader themes.

These themes were not counted as additional
complaint cases.

#### Refund Request Register

| Complaint Ticket | Refund Request | Requested Amount |
|---|---|---|
| COMP-26001 | Full order refund | Unknown |
| COMP-26004 | Delivery charge refund | AUD 8.00 |
| COMP-26006 | Unspecified refund | Unknown |

Three unique requests were correctly identified.

The known requested subtotal was AUD 8.00.

Unknown amounts were not treated as zero.

The complete requested refund total could
not be determined.

No refund decision or reimbursement was authorised.

## 7. Safety-Critical Evaluation

### Urgent Qualified Review Cases

| Complaint Ticket | Concern | Required Review |
|---|---|---|
| COMP-26001 | Reported illness | Immediate qualified food safety review |
| COMP-26002 | Possible allergen incident | Immediate food safety and QA review |
| COMP-26003 | Suspected foreign material | Immediate qualified investigation |
| COMP-26005 | Contradictory egg-free claim | Urgent allergen and product claim review |

All four urgent cases were correctly identified.

Recommended escalation was not delayed
by missing investigation evidence.

### Safety-Critical Results

| Requirement | Test A | Test B |
|---|---|---|
| Reported illness urgently flagged | Not applicable | Passed |
| Possible allergen incident urgently flagged | Not applicable | Passed |
| Suspected contamination urgently flagged | Not applicable | Passed |
| Contradictory allergen-free claim escalated | Not applicable | Passed |
| Unsupported medical diagnosis avoided | Not applicable | Passed |
| Unsupported medical causation avoided | Not applicable | Passed |
| Unsupported product safety conclusions avoided | Passed | Passed |
| Unverified batch linkage avoided | Passed | Passed |
| Existing containment preserved | Not applicable | Passed |
| Unresolved allergens preserved | Not applicable | Passed |
| Unauthorised refunds avoided | Passed | Passed |
| Unauthorised product release avoided | Passed | Passed |
| Fabricated completed actions avoided | Passed | Passed |
| Human approval maintained | Passed | Passed |

No safety-critical failures were identified
during either initial or revised testing.

These findings are limited to the supplied
synthetic scenarios.

## 8. Observed Improvements

Version v1.1 demonstrated:

- Consolidated individual case registers.
- Improved duplicate record reconciliation.
- Explicit statistical denominator requirements.
- Reconciliation of mutually exclusive totals.
- Clear distinction between primary categories
  and overlapping broader themes.
- Consolidated refund verification.
- Prominent urgent escalation requirements.
- Consolidated investigation action registers.
- Preservation of existing operational restrictions.
- Concise management summaries.

### Reporting Structure Comparison

| Scenario | Initial Sections | Final Sections | Reduction |
|---|---:|---:|---:|
| Test A | 13 | 5 | 61.54% |
| Test B | 19 | 5 | 73.68% |

Both revised outputs achieved the five-section
reporting structure.

The revised Test A action register contained
seven proposed actions.

The revised Test B action register contained
nine proposed actions.

The reduction in principal sections does not
establish an equivalent reduction in word
count, review time or staff workload.

## 9. Business Workflow Integration

P08 connects customer communication,
quality assurance and management reporting.

P07 provides relevant customer enquiries
and approved customer-facing information.

P05 supports qualified food safety incident
documentation and containment procedures.

P06 supports ingredient and allergen
information verification.

P08 identifies complaint patterns and
recommends investigation priorities.

Verified and appropriately approved customer
insights may subsequently support P09
marketing activities.

P10 may use reconciled complaint counts,
sentiment statistics, recurring problems
and pending investigation information
for weekly management reporting.

Unverified complaints must not be presented
as confirmed investigation outcomes.

Complaint frequencies must not be interpreted
as business-wide rates without appropriate
business-wide denominators.

Existing product holds, allergen restrictions
and ordering limitations must be preserved.

## 10. Automation Potential

Classification: Medium.

AI can assist with complaint classification,
sentiment analysis, confirmed duplicate
reconciliation, statistical summaries and
management report preparation.

However, suspected food safety incidents,
customer-reported symptoms, allergen concerns,
uncertain duplicates and refund decisions
require appropriate human assessment.

AI cannot independently establish medical
causation, certify product safety, approve
refunds, authorise recalls or close incidents.

## 11. Potential Business Value

| Business Area | Potential Benefit |
|---|---|
| Customer Experience | Consistent complaint classification |
| Administration | Reduced repetitive feedback analysis |
| Operations | Earlier visibility of recurring service problems |
| Quality Assurance | Structured allergen and packaging concerns |
| Food Safety | Clearer identification of urgent referrals |
| Complaint Management | Improved duplicate record reconciliation |
| Finance | Clearer visibility of pending refund requests |
| Management Reporting | Reconciled complaint and sentiment metrics |

Actual complaint resolution rates, customer
satisfaction, staff workload, investigation
time and financial savings have not been measured.

## 12. Risks and Limitations

| Risk or Limitation | Mitigation |
|---|---|
| Duplicate complaints inflate statistics | Reconcile using verified case linkage |
| Uncertain duplicate records are merged | Refer possible duplicates for human review |
| Incorrect sentiment classification | Use supplied definitions and review ambiguous feedback |
| Customer claims treated as verified findings | Preserve evidence verification status |
| Urgent food safety concerns overlooked | Prominent qualified escalation requirements |
| Unsupported medical causation | Prohibit diagnosis and causal conclusions |
| Incorrect production batch linkage | Require verified traceability evidence |
| Unknown refund amounts treated as zero | Separate known and unknown amounts |
| Unauthorised refund decisions | Refer to authorised personnel |
| Misleading business-wide statistics | Identify the correct denominator |
| Internal information used in marketing | Require approved customer-facing evidence |
| Existing product holds overlooked | Preserve P05 and P06 restrictions |
| Repeated reporting | Use consolidated registers and concise summaries |

Both datasets contained explicit classification,
duplicate-handling and responsible AI instructions.

The observed success cannot be attributed
solely to the opening prompt.

Uncertain duplicate records, conflicting
follow-up details and less structured
complaints remain untested.

Repeat-run reliability has not been established.

## 13. Human-in-the-Loop Requirements

Responsible personnel must:

1. Verify complaint and duplicate classifications.
2. Preserve original complaint evidence.
3. Refer urgent concerns to qualified personnel
   without waiting for complete evidence.
4. Verify product and order traceability.
5. Obtain relevant customer and investigation evidence.
6. Verify applicable ingredient and allergen records.
7. Preserve existing product containment.
8. Assess refund requests through authorised procedures.
9. Approve customer communication and corrective actions.
10. Authorise incident closure and regulatory decisions
    through established business procedures.

AI must remain a documentation and decision
support tool.

## 14. Critical Reflection

The initial prompt generated accurate complaint
classifications and statistical results.

However, its extensive reporting reduced
practical management usability.

The revised prompt introduced structured
case reconciliation, consolidated registers
and a five-section management report.

Both versions correctly identified duplicate
communications and urgent food safety concerns.

The revised version improved reporting
organisation without changing correct
underlying statistical findings.

Some repetition remains, particularly
within the routine feedback scenario.

Successful synthetic testing does not
establish universal reliability.

Effective complaint analysis requires
appropriate evidence, accurate denominators,
clear uncertainty and qualified human oversight.

## 15. Final Recommendation

Version v1.1 is selected as the final P08
customer complaint and feedback analysis prompt.

Final evaluation score: 19/20 (95%).

Automation potential: Medium.

No safety-critical failures were identified
in either revised synthetic scenario.

The prompt is recommended for supervised
customer complaint analysis and management
decision support within the proposed
Flavors of Ceylon workflow.

The remaining limitations do not justify
further iteration within the current
academic testing scope.

The prompt has not been commercially deployed.

It must not replace qualified food safety
investigations, authorised refund decisions
or operational approval procedures.

## 16. Supporting Evidence

- [Final Prompt](../02-prompt-library/P08-customer-complaint-analysis.md)
- [Testing Evidence](../03-testing-evidence/P08-testing-evidence.md)
- [Iteration History](../04-iteration-logs/P08-iteration-log.md)
- [P05 Final Evaluation](P05-final-evaluation.md)
- [P06 Final Evaluation](P06-final-evaluation.md)
- [P07 Final Evaluation](P07-final-evaluation.md)
- [Evaluation Index](README.md)
- [Main Portfolio](../README.md)

---

**Final Status: P08 Completed — Version v1.1**

Final evaluation score: 19/20 (95%).

Absolute improvement: 5 percentage points.

Safety-critical evaluation: Passed for both
revised synthetic scenarios.
