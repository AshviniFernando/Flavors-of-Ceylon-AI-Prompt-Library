# P01 — Product Demand Forecasting: Iteration Log

## 1. Prompt Development Objective

Improve the accuracy, consistency, transparency
and business suitability of AI-generated product
demand estimates for Flavors of Ceylon.

---

## 2. Version History

| Version | Change Made | Observed Effect | Lesson Learned |
|---|---|---|---|
| v1.0 | Initial role-based and contextual forecasting prompt | Correct basic forecasts but limitations in uncertainty and production planning; 80% evaluation score | Business context alone is insufficient for reliable decision support |
| v1.1 | Added data validation, standard forecasting formulas, reliability classifications and production safeguards | Original weaknesses addressed; 100% across three evaluated scenarios | Explicit rules improve transparency and responsible AI behaviour |
| v1.2 | Added standardised capacity calculations, shortfall analysis and a five-section reporting structure | Retained numerical accuracy and safeguards while improving output standardisation; 100% across three corrected scenarios | Prompt refinement can improve business usability without increasing numerical evaluation scores |

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

The revised prompt successfully addressed the
major limitations identified during v1.0 testing.

Test Case A produced accurate forecasts for all
five products, resulting in total estimated demand
of 470 units.

The response included complete data validation,
standardised reliability classifications and
transparent calculations for every product.

Test Case B correctly handled missing records
and excluded the stockout-affected chicken kottu
observation.

The pol sambol forecast was withheld because
only two usable historical observations were
available.

A partial subtotal of 390 units was correctly
reported for the four forecastable products.

Both responses withheld manufacturing quantities
because verified inventory, safety stock and
production capacity information was unavailable.

### Evaluation Results

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 2 |
| Business Relevance | 2 | 2 |
| Responsible AI | 2 | 2 |
| Total | 10/10 | 10/10 |

Combined score: 20/20 (100%).

The combined evaluation score improved by
20 percentage points compared with v1.0.

### Remaining Limitations

The generated reports contain lengthy explanations
and some repeated information.

The linear forecasting method has limited ability
to represent irregular or seasonal demand patterns.

The numerical production requirement calculation
and production capacity checks could not be
evaluated because neither test scenario supplied
the necessary operational information.

Further testing is required to assess these
production planning functions.

### Lesson Learned

Explicit forecasting rules and data validation
constraints can improve the consistency and
transparency of AI-generated business information.

Withholding unsupported recommendations is
sometimes more valuable than providing a complete
but unreliable numerical output.

A successful evaluation against selected test
criteria does not guarantee reliable performance
in every operational scenario.

AI prompt refinement should consider output
efficiency, practical business usability and
responsible decision-making alongside accuracy.

### Additional Production Planning Evaluation

Test Case C was conducted using complete historical
sales, finished-product inventory, target safety
stock and product-specific production capacity.

The v1.1 prompt correctly calculated estimated
demand of 470 units, required production of 345
units and capacity-limited production of 325 units.

It identified a 20-unit fish roti production
shortfall, consisting of 10 units of estimated
unmet customer demand and 10 units of safety
stock shortfall.

The additional test achieved 10/10.

The combined v1.1 evaluation across all three
scenarios was 30/30.

Although the numerical calculations were correct,
the response contained repeated information and
unrequested visualisations.

The v1.2 refinement therefore focuses on report
efficiency, standardised capacity calculations
and operational input validation rather than
correcting demonstrated numerical errors.

---

## 5. Version v1.2 — Further Refined Prompt

### Development Date

25 November 2026

### Changes Made

1. Introduced explicit capacity-limited production
   calculations.

2. Added production shortfall calculations.

3. Distinguished unmet customer demand from
   safety stock shortfalls.

4. Introduced validation of operational inputs.

5. Prevented unsupported assumptions about
   transferring production capacity between products.

6. Introduced a concise five-section report structure.

7. Removed unnecessary repetition and unsolicited
   charts.

8. Retained all successful v1.1 forecasting,
   validation and human oversight rules.

### Reason for Changes

Although v1.1 achieved the maximum score across
the two original scenarios, the generated reports
were lengthy and the production capacity function
required additional testing.

The refinement aims to improve practical management
usability and operational decision support.

### Expected Effect

The revised prompt is expected to provide more
concise reports and clearer production capacity
calculations without reducing forecasting quality.

This expected effect has not yet been verified.

### Observed Effect — Initial Testing Attempt

The initial v1.2 testing attempt revealed a
testing procedure issue.

Expected numerical outcomes were supplied to the
AI, while complete original test inputs were not
consistently provided.

Consequently, the initial responses cannot be
used as independent evidence of forecasting or
production calculation performance.

The Test Case C response appropriately withheld
calculations when required information was missing.

### Corrective Action

Retest v1.2 using complete original input data
without providing expected answers.

The initial testing responses will be retained
for transparency and academic evidence.

### Remaining Limitations

Pending corrected retesting and final evaluation.

### Lesson Learned

Prompt performance must be evaluated using
appropriate and controlled test inputs.

Expected answers should be used by the evaluator
after testing rather than supplied to the AI
before it generates a response.

### Observed Effect — Corrected Retesting

All three corrected test scenarios satisfied
the selected evaluation criteria.

Test Case A produced a total estimated demand
of 470 units.

Test Case B correctly withheld an insufficient-data
forecast and reported a partial subtotal of
390 units across four products.

Test Case C produced 345 units of required
production and 325 units of capacity-limited
production.

The response correctly distinguished the
20-unit production shortfall into 10 units
of estimated unmet customer demand and
10 units of safety stock shortfall.

The final responses retained the required
forecasting calculations and human approval
safeguards.

The five-section report structure was followed,
with concise management summaries and no
unrequested charts.

### Evaluation Results

| Criterion | Test A | Test B | Test C |
|---|---:|---:|---:|
| Accuracy | 2 | 2 | 2 |
| Completeness | 2 | 2 | 2 |
| Consistency | 2 | 2 | 2 |
| Business Relevance | 2 | 2 | 2 |
| Responsible AI | 2 | 2 | 2 |
| Total | 10/10 | 10/10 | 10/10 |

Combined score: 30/30 (100%).

### Remaining Limitations

- Limited historical forecasting period.
- No modelling of seasonality or sudden changes.
- No validation against actual future sales.
- Some repetition remains in the generated reports.
- Invalid operational values and shared capacity
  conflicts have not been directly tested.
- Repeat-run reliability has not been established.
- Human verification remains necessary.

### Final Lesson Learned

Effective prompt engineering requires both
accurate task instructions and a controlled
testing methodology.

Providing expected answers during testing can
reduce evaluation validity.

Explicit formulas, structured reporting and
responsible decision boundaries can improve
business usability even when evaluation scores
remain unchanged.

The final prompt should be selected based on
observed performance and suitability for the
intended business workflow rather than version
number alone.

### Final Version Selection

Version v1.2 is selected as the final P01 prompt
because it retains the successful v1.1 safeguards
and introduces more standardised operational
calculations and management reporting.

No further prompt refinement is required within
the current academic testing scope.

---

## 6. Version Comparison

### Original Comparable Scenarios

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 7/10 | 16/20 (80%) |
| v1.1 | 10/10 | 10/10 | 20/20 (100%) |
| v1.2 | 10/10 | 10/10 | 20/20 (100%) |

Absolute improvement: 20 percentage points.

Relative improvement in evaluation score: 25%.

### Additional Production Planning Scenario

| Version | Test C | Status |
|---|---:|---|
| v1.0 | Not tested | Outside initial scope |
| v1.1 | 10/10 | Evaluated |
| v1.2 | 10/10 | Evaluated |

The final v1.2 prompt achieved 30/30 across
all three corrected test scenarios.

The initial v1.2 testing attempts are excluded
from formal evaluation due to input limitations.

## 7. Current Development Status

P01 development, testing, iterative improvement
and final evaluation are complete.

Final selected version: v1.2.

Automation potential: Medium.

Operational deployment: Not implemented.

All outputs require production manager review
and approval.

## 8. Related Evidence

- [Final P01 Prompt](../02-prompt-library/P01-product-demand-forecasting.md)
- [P01 Testing Evidence](../03-testing-evidence/P01-testing-evidence.md)
- [P01 Final Evaluation](../05-evaluation/P01-final-evaluation.md)
- [Iteration Log Index](README.md)
