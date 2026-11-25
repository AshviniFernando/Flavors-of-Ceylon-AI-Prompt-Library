# P01 — Product Demand Forecasting: Iteration Log

## 1. Prompt Development Objective

Improve the accuracy, consistency, transparency
and business suitability of AI-generated product
demand estimates for Flavors of Ceylon.

---

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial role-based and contextual forecasting prompt | Accurate forecasts for complete data, but limitations in handling uncertainty and production requirements | Clear business context is useful, but additional constraints are required for reliable decision support |
| v1.1 | Introduced data validation, standard calculations, minimum data requirements, reliability classification and production planning safeguards | Awaiting retesting | Pending evaluation |
| v1.2 | Pending further refinement if required | Pending | Pending |

---

## 3. Version v1.0 — Initial Prompt

### Development and Testing Date

25 November 2026

### Prompting Strategies

- Role-based prompting
- Contextual prompting
- Structured-output prompting

### Test Case A — Observations

The AI correctly identified all product sales
trends and selected a linear trend forecasting
method.

The resulting Week 5 forecast was 470 units,
representing an estimated increase of 6.82%
compared with Week 4 sales.

The response was mathematically correct for
the selected forecasting method.

However, production recommendations were equal
to forecast demand despite missing finished-product
inventory, safety stock and capacity information.

### Test Case B — Observations

The AI correctly recognised missing sales records
and the impact of a four-day chicken kottu stockout.

It avoided treating missing records as zero and
introduced qualitative forecast confidence ratings.

However, a missing fish roti record was estimated,
and a pol sambol forecast was generated from only
two available historical observations.

The response also provided a combined production
recommendation of 470 units despite differing
levels of uncertainty.

### Evaluation Scores

| Evaluation Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 1 |
| Business Relevance | 1 | 1 |
| Responsible AI | 2 | 1 |
| Total | 9/10 | 7/10 |

Combined score: 16/20 (80%).

### Identified Improvement Opportunities

- Introduce a standard forecasting formula.
- Require transparent calculation steps.
- Preserve missing records without filling them.
- Exclude stockout-affected observations.
- Introduce minimum usable data requirements.
- Standardise data reliability classifications.
- Distinguish full forecasts from partial subtotals.
- Separate forecast demand from production quantities.

### Lesson Learned

A prompt can generate mathematically correct and
professionally presented forecasts while still
providing recommendations that require further
business information.

Explicit data validation and decision boundaries
are important when using AI for operational
planning.

---

## 4. Version v1.1 — Revised Prompt

### Development Date

25 November 2026

### Prompting Strategies

- Role-based prompting
- Contextual prompting
- Task decomposition
- Constraint-based prompting
- Structured-output prompting
- Rule-based classification

### Changes Made

1. Introduced explicit missing-data validation.

2. Required stockout-affected sales observations
   to be excluded from baseline calculations.

3. Defined a standard linear trend formula using
   elapsed week intervals.

4. Required at least three usable historical
   observations before producing a forecast.

5. Introduced rule-based data reliability
   classifications.

6. Required calculation transparency for each
   forecasted product.

7. Required partial subtotals when forecasts
   cannot be generated for every product.

8. Separated demand forecasts from production
   requirements.

9. Strengthened management approval requirements.

### Reason for Changes

The changes address observed weaknesses in the
initial test responses, particularly the handling
of incomplete sales records, forecast transparency
and production recommendations without sufficient
operational information.

### Expected Effect

The revised prompt is expected to produce more
consistent calculations, clearer data quality
assessments and more responsible production
planning recommendations.

This expected effect has not yet been verified.

### Observed Effect

Pending actual v1.1 testing.

### Remaining Limitations

Pending actual v1.1 evaluation.

### Lesson Learned

Pending actual v1.1 evaluation.

---

## 5. Version v1.2 — Further Refined Prompt

### Development Date

Pending.

### Changes Made

Pending further testing.

### Reason for Changes

Pending v1.1 evaluation.

### Observed Effect

Pending testing.

### Lesson Learned

Pending.

---

## 6. Version Comparison

| Version | Test A Score | Test B Score | Combined Score | Status |
|---|---:|---:|---:|---|
| v1.0 | 9/10 | 7/10 | 16/20 (80%) | Evaluated |
| v1.1 | Pending | Pending | Pending | Awaiting retesting |
| v1.2 | Pending | Pending | Pending | Not developed |

## 7. Current Development Status

Initial v1.0 testing and evaluation are complete.

The v1.1 prompt has been developed based on the
observed limitations of the original responses.

The next stage is to repeat both original test
scenarios using the revised prompt.

The evaluation measures AI response quality and
does not establish actual commercial forecasting
accuracy.

## 8. Related Evidence

- [P01 Current Prompt](../02-prompt-library/P01-product-demand-forecasting.md)
- [P01 Testing Evidence](../03-testing-evidence/P01-testing-evidence.md)
- [Iteration Log Index](README.md)
