# P04 — Food Production and Batch Planning

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Business Function | Food Manufacturing |
| Workflow | Planning and Manufacturing |
| Current Version | v1.0 |
| Status | Initial Draft — Not Yet Tested |
| Prompting Strategy | Contextual and task-decomposition prompting |

---

## 1. Prompt Text

> You are a production planning assistant for
> Flavors of Ceylon.
>
> Develop a proposed weekly food production schedule
> using the supplied approved demand forecasts,
> available ingredients, staffing information and
> production capacity.
>
> Recommend production quantities, batch allocation
> and scheduling priorities for each food product.
>
> Identify potential production bottlenecks, ingredient
> shortages and resource limitations.
>
> Present the proposed schedule in a clear table.
> Flag missing information and do not override approved
> food safety procedures or production limits.

## 2. Intended Workflow or Task

This prompt supports weekly production scheduling.

- Trigger: Demand forecasts and supply information are approved.
- Input: Demand, inventory, staffing and capacity records.
- Output: Proposed production and batch schedule.
- Responsible person: Production manager.
- Next step: Human review before production begins.

## 3. Problem Being Solved

Manual production planning may create inefficient
batch allocation, excessive workloads, delayed
orders and unnecessary food waste.

## 4. Automation Potential

Level: Medium — Preliminary assessment.

AI can generate draft schedules and identify
resource constraints. Production managers must
confirm feasibility, staffing and safety requirements.

## 5. Risks and Limitations

| Risk | Mitigation |
|---|---|
| Unrealistic production quantities | Verify capacity limits |
| Incorrect ingredient allocation | Check approved stock |
| Inappropriate production sequence | Follow approved procedures |
| Staff workload conflicts | Review staffing availability |

AI must not independently approve manufacturing
schedules or bypass food safety procedures.

---

## Version History

| Version | Change | Status |
|---|---|---|
| v1.0 | Initial prompt development | Not yet tested |

## Testing Evidence

Pending practical testing in Stage 04.
