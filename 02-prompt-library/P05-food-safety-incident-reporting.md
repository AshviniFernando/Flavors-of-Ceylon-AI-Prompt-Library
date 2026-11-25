# P05 — Food Safety and Quality Incident Reporting

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Business Function | Quality Assurance |
| Workflow | Food Safety and Product Quality |
| Current Version | v1.0 |
| Status | Initial Draft — Not Yet Tested |
| Prompting Strategy | Role-based and constraint-based prompting |

---

## 1. Prompt Text

> You are a food safety documentation assistant for
> Flavors of Ceylon.
>
> Convert the supplied production observations into
> a structured food safety or quality incident report.
>
> Include the incident date, affected product,
> batch identification, observed issue, recorded
> measurements, actions already taken and missing
> information.
>
> Identify matters requiring urgent review by the
> responsible food safety personnel.
>
> Clearly distinguish recorded facts from suggested
> follow-up actions.
>
> Do not invent measurements, certify food safety,
> determine product suitability or authorise the
> release of affected products.

## 2. Intended Workflow or Task

This prompt supports food safety documentation.

- Trigger: A production or quality incident is reported.
- Input: Staff observations and available incident records.
- Output: Structured draft incident report.
- Responsible person: Food safety or quality assurance officer.
- Next step: Qualified review and appropriate action.

## 3. Problem Being Solved

Unstructured incident notes may result in incomplete
documentation, inconsistent reporting and delayed
communication of potential safety concerns.

## 4. Automation Potential

Level: Medium — Preliminary assessment.

AI can organise recorded observations and identify
missing fields. Qualified personnel must investigate
incidents and make all food safety decisions.

## 5. Risks and Limitations

| Risk | Mitigation |
|---|---|
| Invented incident information | Use recorded facts only |
| Incorrect risk interpretation | Require qualified review |
| Missing critical measurements | Flag incomplete records |
| Delayed safety escalation | Follow approved incident procedures |

AI must not replace food safety investigations,
regulatory obligations or professional judgement.

---

## Version History

| Version | Change | Status |
|---|---|---|
| v1.0 | Initial prompt development | Not yet tested |

## Testing Evidence

Pending practical testing in Stage 04.
