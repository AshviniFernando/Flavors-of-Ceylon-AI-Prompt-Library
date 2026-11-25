# P01 — Product Demand Forecasting: Final Evaluation

## 1. Evaluation Information

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Food Manufacturing and Hospitality |
| Prompt ID | P01 |
| Business Function | Demand Planning |
| Workflow | Planning and Manufacturing |
| Initial Version | v1.0 |
| Final Selected Version | v1.2 |
| Evaluation Status | Completed |
| Data Type | Synthetic business data |
| Automation Potential | Medium |
| Operational Deployment | Not implemented |

---

## 2. Evaluation Objective

Evaluate the ability of generative AI to support
product demand forecasting, historical sales
analysis and indicative production planning
at Flavors of Ceylon.

The evaluation considers accuracy, completeness,
consistency, business relevance and responsible
AI behaviour.

## 3. Evaluation Methodology

The prompt was developed through an iterative
testing and refinement process.

Three synthetic scenarios were used:

- Test A: Complete historical sales records.
- Test B: Missing sales data and stockout conditions.
- Test C: Inventory and production capacity constraints.

Versions v1.0 and v1.1 were compared using the
original scenarios.

Test C was introduced during v1.1 development
to evaluate numerical production planning.

Initial v1.2 testing attempts contained input
limitations and expected-answer leakage.

These attempts were retained for transparency
but excluded from formal evaluation.

Corrected tests used the complete original
datasets without supplying expected answers.

Each evaluation criterion was scored from
zero to two, with a maximum of ten points
per scenario.

## 4. Prompting Strategies

The final prompt incorporates:

- Role-based prompting
- Contextual prompting
- Constraint-based prompting
- Task decomposition
- Structured-output prompting
- Rule-based data classification
- Explicit mathematical instructions
- Human-in-the-loop decision support

## 5. Version Performance

### Comparable Evaluation — Tests A and B

| Version | Test A | Test B | Combined | Percentage |
|---|---:|---:|---:|---:|
| v1.0 | 9/10 | 7/10 | 16/20 | 80% |
| v1.1 | 10/10 | 10/10 | 20/20 | 100% |
| v1.2 | 10/10 | 10/10 | 20/20 | 100% |

Absolute improvement: 20 percentage points.

Relative improvement in evaluation score: 25%.

### Additional Scenario — Test C

| Version | Score |
|---|---:|
| v1.0 | Not tested |
| v1.1 | 10/10 |
| v1.2 | 10/10 |

## 6. Final Evaluation Scores

| Criterion | Test A | Test B | Test C |
|---|---:|---:|---:|
| Accuracy | 2 | 2 | 2 |
| Completeness | 2 | 2 | 2 |
| Consistency | 2 | 2 | 2 |
| Business Relevance | 2 | 2 | 2 |
| Responsible AI | 2 | 2 | 2 |
| Total | 10/10 | 10/10 | 10/10 |

Final combined score: 30/30 (100%).

The score reflects performance against the
selected synthetic scenarios and evaluation
criteria.

It does not represent actual commercial
forecasting accuracy or guaranteed AI reliability.

## 7. Key Testing Results

### Test A — Complete Historical Sales

| Indicator | Result |
|---|---|
| Historical records | 20 |
| Forecasted products | 5 |
| Week 4 recorded sales | 440 units |
| Week 5 estimated demand | 470 units |
| Estimated demand increase | 6.82% |
| Production quantities | Pending verification |

### Test B — Incomplete Data and Stockouts

| Indicator | Result |
|---|---|
| Missing records | 3 |
| Stockout-affected records | 1 |
| Usable observations | 16 |
| Forecasted products | 4 |
| Forecast withheld | Pol sambol sachets |
| Partial estimated demand | 390 units |
| Production quantities | Pending verification |

The partial subtotal excludes one product and
must not be interpreted as total business demand.

### Test C — Production Planning

| Indicator | Result |
|---|---:|
| Estimated customer demand | 470 |
| Required production | 345 |
| Capacity-limited production | 325 |
| Production shortfall | 20 |
| Estimated unmet demand | 10 |
| Safety stock shortfall | 10 |
| Projected closing inventory | 30 |
| Estimated demand fulfilled | 460 |

All quantities are expressed in units.

Fish roti was the only product with an identified
production capacity shortfall.

Vegetable rolls required no additional production
because existing inventory could satisfy forecast
demand and target safety stock.

## 8. Observed Improvements

Compared with v1.0, the final prompt demonstrates:

- More explicit data validation.
- Transparent forecasting calculations.
- Standardised reliability classifications.
- Appropriate handling of missing observations.
- Exclusion of stockout-affected records.
- Responsible withholding of insufficient-data forecasts.
- Clear separation of demand and production.
- Standardised capacity and shortfall calculations.
- More structured management reporting.
- Stronger operational decision boundaries.

Version v1.2 retained the evaluation performance
of v1.1 while improving the standardisation of
operational calculations and reporting.

## 9. Automation Potential

Classification: Medium.

AI can assist with historical sales analysis,
forecast preparation, data validation, production
requirement calculations and management reporting.

However, forecast reliability, inventory usability,
capacity constraints and manufacturing decisions
require human verification.

The prompt supports decision-making rather than
autonomous production management.

## 10. Potential Business Value

| Business Area | Potential Benefit |
|---|---|
| Demand Planning | More consistent forecasting calculations |
| Inventory Management | Earlier identification of possible excess stock |
| Food Waste | Reduced risk of unnecessary production |
| Manufacturing | Earlier identification of capacity constraints |
| Management | More transparent decision-support reports |
| Risk Management | Reduced reliance on unsupported numerical estimates |

These are potential business benefits.

Actual cost savings, time savings, food waste
reductions and commercial performance improvements
have not been measured.

## 11. Risks and Limitations

| Risk or Limitation | Mitigation |
|---|---|
| Limited historical data | Collect additional verified sales records |
| Missing data | Flag missing records and withhold forecasts where required |
| Incorrect calculations | Independently verify calculations |
| Seasonal demand changes | Use additional data and appropriate forecasting methods |
| Unexpected market conditions | Apply management judgement |
| Capacity constraints | Verify available product-specific and shared resources |
| Inventory uncertainty | Confirm usable stock before production planning |
| AI over-reliance | Require production manager approval |

The simple endpoint trend method may overlook
irregular intermediate sales patterns.

Data reliability classifications do not represent
statistical forecast confidence.

Invalid operational values, shared capacity
conflicts and repeat-run reliability require
further testing.

## 12. Human-in-the-Loop Requirements

The production planning manager must:

1. Verify historical sales and stockout records.
2. Review forecast calculations.
3. Confirm usable finished-product inventory.
4. Verify target safety stock and production capacity.
5. Assess additional operational and safety constraints.
6. Approve final manufacturing decisions.

AI must not independently authorise manufacturing.

## 13. Critical Reflection

The initial prompt successfully produced basic
demand estimates but generated production
recommendations without sufficient operational
information.

Iterative refinement introduced explicit
forecasting formulas, data validation and
responsible decision boundaries.

The testing process also demonstrated the
importance of separating expected answers
from actual AI inputs.

The final version achieved the maximum score
under the selected evaluation criteria.

However, further testing and business validation
would be necessary before real-world deployment.

## 14. Final Recommendation

Version v1.2 is selected as the final P01 prompt.

The prompt is recommended for supervised demand
planning and indicative production analysis
within the proposed Flavors of Ceylon workflow.

Automation potential remains Medium.

The prompt is evaluated for academic purposes
and has not been operationally deployed.

## 15. Supporting Evidence

- [Final Prompt](../02-prompt-library/P01-product-demand-forecasting.md)
- [Testing Evidence](../03-testing-evidence/P01-testing-evidence.md)
- [Iteration History](../04-iteration-logs/P01-iteration-log.md)
- [Evaluation Index](README.md)
- [Main Portfolio](../README.md)

---

**Final Status: P01 Completed — Version v1.2**

All evaluation scores are based on the project
evaluation rubric and selected synthetic scenarios.
