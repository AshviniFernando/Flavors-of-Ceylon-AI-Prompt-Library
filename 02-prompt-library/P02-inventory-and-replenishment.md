# P02 — Ingredient Inventory and Replenishment

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Business Function | Inventory Management |
| Workflow | Planning and Manufacturing |
| Current Version | v1.0 |
| Status | Initial Draft — Not Yet Tested |
| Prompting Strategy | Role-based and task-oriented prompting |

---

## 1. Prompt Text

> You are an inventory management assistant for
> Flavors of Ceylon.
>
> Review the supplied ingredient stock levels,
> expected production requirements and available
> expiry information.
>
> Identify potential ingredient shortages, excess
> stock and ingredients approaching their expiry
> dates.
>
> Recommend replenishment quantities and stock
> management actions. Present the findings in a
> table and identify any missing information.
>
> Do not assume expired or unverified ingredients
> are suitable for production.

## 2. Intended Workflow or Task

This prompt supports ingredient inventory reviews.

- Trigger: Scheduled inventory review.
- Input: Stock records and approved production requirements.
- Output: Shortage alerts and replenishment recommendations.
- Responsible person: Inventory supervisor.
- Next step: Approved purchasing requirements support P03.

## 3. Problem Being Solved

Manual inventory monitoring may cause ingredient
shortages, excessive purchasing, production delays
and avoidable food waste.

## 4. Automation Potential

Level: Medium — Preliminary assessment.

AI can assist with stock analysis and replenishment
recommendations. Inventory staff must verify physical
stock, expiry information and purchasing quantities.

## 5. Risks and Limitations

| Risk | Mitigation |
|---|---|
| Inaccurate stock records | Verify physical inventory |
| Incorrect measurement units | Standardise ingredient units |
| Missing expiry information | Flag for manual inspection |
| Excessive purchasing | Require approval before ordering |

AI recommendations must not override ingredient
safety checks or stock control procedures.

---

## Version History

| Version | Change | Status |
|---|---|---|
| v1.0 | Initial prompt development | Not yet tested |

## Testing Evidence

Pending practical testing in Stage 04.
