# P01 — Product Demand Forecasting

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Business Function | Demand Planning |
| Workflow | Planning and Manufacturing |
| Current Version | v1.0 |
| Status | Initial Draft — Not Yet Tested |
| Prompting Strategy | Role-based and contextual prompting |

---

## 1. Prompt Text

> You are a demand planning assistant for Flavors of
> Ceylon, an Australian food manufacturing business
> specialising in Sri Lankan cuisine.
>
> Analyse the supplied historical weekly sales data
> and estimate product demand for the upcoming week.
>
> Identify products with increasing or decreasing
> demand and recommend quantities for production
> planning. Explain the main reasons behind your
> recommendations.
>
> Present the results in a clear table. Use only the
> supplied business data and identify assumptions.

## 2. Intended Workflow or Task

This prompt supports weekly demand planning.

- Trigger: Weekly sales data becomes available.
- Input: Historical product sales information.
- Output: Estimated demand and production recommendations.
- Responsible person: Production planning manager.
- Next step: Approved forecasts support P02 and P04.

## 3. Problem Being Solved

Manual demand estimation may result in inaccurate
production quantities, product shortages, excess
stock and unnecessary food waste.

## 4. Automation Potential

Level: Medium — Preliminary assessment.

AI can assist with identifying sales patterns and
preparing demand estimates. A planning manager must
verify calculations and approve final forecasts.

## 5. Risks and Limitations

| Risk | Mitigation |
|---|---|
| Inaccurate forecasts | Verify against historical sales |
| Limited historical data | Identify uncertainty |
| Incorrect calculations | Recalculate using approved tools |
| Unexpected demand changes | Apply managerial judgement |

AI-generated forecasts are estimates, not guaranteed
future sales outcomes.

---

## Version History

| Version | Change | Status |
|---|---|---|
| v1.0 | Initial prompt development | Not yet tested |

## Testing Evidence

Pending practical testing in Stage 04.
