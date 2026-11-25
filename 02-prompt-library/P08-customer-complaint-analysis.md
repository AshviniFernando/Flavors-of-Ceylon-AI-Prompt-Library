# P08 — Customer Complaint and Feedback Analysis

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Business Function | Customer Experience |
| Workflow | Customer Experience and Marketing |
| Current Version | v1.0 |
| Status | Initial Draft — Not Yet Tested |
| Prompting Strategy | Classification and structured-output prompting |

---

## 1. Prompt Text

> You are a customer experience analyst for Flavors
> of Ceylon.
>
> Analyse the supplied customer complaints and
> feedback concerning the company's food products
> and services.
>
> Classify feedback by issue category, customer
> sentiment and suggested priority.
>
> Identify recurring problems and recommend
> appropriate follow-up actions.
>
> Present individual findings in a table followed
> by a short management summary.
>
> Immediately flag reported illness, possible
> contamination or allergen incidents for qualified
> food safety review.
>
> Do not invent complaint details, determine medical
> causes or authorise refunds.

## 2. Intended Workflow or Task

This prompt supports customer feedback management.

- Trigger: New complaints or feedback become available.
- Input: Anonymised customer feedback records.
- Output: Categorised complaints and suggested actions.
- Responsible person: Customer experience manager.
- Next step: Human review and relevant escalation.

## 3. Problem Being SolVED

Manual complaint analysis may delay issue
identification, reduce response consistency and
make recurring product problems difficult to detect.

## 4. Automation Potential

Level: Medium — Preliminary assessment.

AI can support complaint categorisation and identify
common themes. Staff must verify priorities and
manage sensitive or safety-related complaints.

## 5. Risks and Limitations

| Risk | Mitigation |
|---|---|
| Incorrect sentiment classification | Review original feedback |
| Underestimated safety concerns | Prioritise safety escalation |
| Customer privacy exposure | Anonymise personal information |
| Unsupported compensation decisions | Require management approval |

AI must not independently dismiss serious complaints
or determine whether food caused a reported illness.

---

## Version History

| Version | Change | Status |
|---|---|---|
| v1.0 | Initial prompt development | Not yet tested |

## Testing Evidence

Pending practical testing in Stage 04.
