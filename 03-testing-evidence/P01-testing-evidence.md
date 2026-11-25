# P01 — Product Demand Forecasting: Testing Evidence

## 1. Testing Information

| Detail | Information |
|---|---|
| Prompt ID | P01 |
| Business | Flavors of Ceylon |
| Business Function | Demand Planning |
| AI Tool | To be recorded during testing |
| AI Model | To be recorded if available |
| Data Type | Synthetic business data |
| Testing Status | Pending |

## 2. Testing Objective

Evaluate whether the AI prompt can analyse historical
food product sales, identify demand patterns and
produce useful demand estimates for production planning.

Testing also evaluates the handling of missing data,
stock shortages, uncertainty and unsupported assumptions.

---

## 3. Test Case A — Standard Scenario

The production manager requires Week 5 demand
estimates based on historical weekly sales.

### Test Input

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | 120 | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 80 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | 50 | 60 | 70 |

All figures represent units sold.

No stock shortages or unusual promotional events
are reported for this scenario.

### Expected Output

- Identify increasing sales patterns.
- Identify decreasing sales patterns.
- Identify stable sales patterns.
- Provide reasonable Week 5 demand estimates.
- Explain the forecasting method or assumptions.
- Present clear production recommendations.
- Avoid unsupported business information.

---

## 4. Test Case B — Challenging Scenario

The production manager requires Week 5 demand
estimates, but some sales records are incomplete.

### Test Input

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | Missing | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 25 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | Missing | 60 | Missing |

Additional information:

- Fish roti Week 3 sales are unavailable due to a
  reporting system error.
- Chicken kottu was out of stock for four days
  during Week 4.
- Some pol sambol sales records are unavailable.
- No promotional campaign information is supplied.

### Expected Output

- Identify all missing sales records.
- Do not interpret missing values as zero.
- Recognise that stock shortages can reduce
  recorded sales independently of customer demand.
- Avoid inventing missing sales information.
- Communicate forecasting uncertainty.
- Recommend appropriate human review.

---

## 5. Version v1.0 — Initial Prompt Testing

### Testing Date and AI Model

Pending actual testing.

### Test Case A — Actual AI Output

Pending actual testing.

### Test Case B — Actual AI Output

Pending actual testing.

### Observed Strengths

Pending evaluation.

### Observed Weaknesses

Pending evaluation.

---

## 6. Version v1.1 — Revised Prompt Testing

### Testing Date and AI Model

Pending.

### Test Case A — Actual AI Output

Pending.

### Test Case B — Actual AI Output

Pending.

### Observed Improvements

Pending.

### Remaining Limitations

Pending.

---

## 7. Version v1.2 — Further Refined Prompt Testing

### Testing Date and AI Model

Pending.

### Test Case A — Actual AI Output

Pending.

### Test Case B — Actual AI Output

Pending.

### Final Observations

Pending.

---

## 8. Testing Integrity

All sales figures are fictional and created for
academic testing purposes.

Actual AI outputs will be recorded without
retrospective modification.

The results do not demonstrate actual commercial
forecasting performance.

## Related Files

- [P01 Prompt](../02-prompt-library/P01-product-demand-forecasting.md)
- [Testing Evidence Index](README.md)
