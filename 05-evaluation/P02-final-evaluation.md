# P02 — Ingredient Inventory and Replenishment: Final Evaluation

## 1. Evaluation Information

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Food Manufacturing and Hospitality |
| Prompt ID | P02 |
| Business Function | Inventory Management |
| Initial Version | v1.0 |
| Final Selected Version | v1.1 |
| Evaluation Status | Completed |
| Data Type | Synthetic business data |
| Automation Potential | Medium |
| Operational Deployment | Not implemented |

---

## 2. Evaluation Objective and Methodology

Evaluate the ability of generative AI to support
ingredient inventory assessment, expiry management,
stock validation and replenishment planning.

Two synthetic scenarios were used:

- Test A: Complete ingredient inventory records.
- Test B: Missing information, measurement unit
  differences, expired inventory and stock
  expiring before planned production.

Both prompt versions were tested using the same
original datasets.

Expected answers were not supplied during testing.

The evaluation considered accuracy, completeness,
consistency, business relevance and responsible AI
behaviour, using a zero-to-two scoring scale
for each criterion.

## 3. Prompting Strategies

- Role-based prompting.
- Contextual prompting.
- Constraint-based prompting.
- Rule-based classification.
- Explicit mathematical instructions.
- Structured-output prompting.
- Human-in-the-loop decision support.

## 4. Version Performance

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 8/10 | 17/20 (85%) |
| v1.1 | 10/10 | 9/10 | 19/20 (95%) |

Absolute improvement: 10 percentage points.

Relative improvement in evaluation score: 11.76%.

## 5. Final Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 1 |
| Business Relevance | 2 | 2 |
| Responsible AI | 2 | 2 |
| Total | 10/10 | 9/10 |

Final combined score: 19/20 (95%).

The score measures response quality under
selected synthetic business scenarios.

It does not represent guaranteed inventory
accuracy or actual commercial performance.

## 6. Key Testing Results

### Test A — Standard Inventory

| Ingredient | Eligible Stock | Replenishment | Classification |
|---|---:|---:|---|
| Wheat flour | 30 kg | 15 kg | Established |
| Rice | 40 kg | 0 kg | No replenishment |
| Chicken | 18 kg | 12 kg | Established |
| Grated coconut | 12 kg | 0 kg | No replenishment |
| Eggs | 100 units | 0 units | No replenishment |

Established replenishment: 27 kg.

Provisional replenishment: 0 kg.

Surplus stock: 15 kg of rice and 20 eggs.

Chicken and grated coconut were correctly
identified as requiring expiry attention.

### Test B — Challenging Inventory

| Ingredient | Eligible Stock | Replenishment | Classification |
|---|---:|---:|---|
| Wheat flour | 20 kg | 5 kg | Established |
| Rice | 15 kg | 5 kg | Provisional |
| Chicken | 10 kg | 15 kg | Provisional |
| Grated coconut | 4 kg | 6 kg | Established |
| Eggs | 60 units | 0 units | No replenishment |

| Indicator | Result |
|---|---|
| Established replenishment | 11 kg |
| Provisional replenishment | 20 kg |
| Total indicative replenishment | 31 kg |
| Eligible batches | 6 |
| Expired batches | 1 |
| Batches expiring before planned usage | 1 |
| Batches pending verification | 2 |
| Surplus eggs | 12 units |
| Eligible stock requiring expiry attention | 14 kg |

Provisional purchasing quantities must be
reassessed if held inventory is verified.

All purchasing quantities require approval.

## 7. Observed Improvements

Compared with v1.0, the final prompt demonstrated:

- Standardised inventory eligibility categories.
- Clearer measurement unit validation.
- Separate established and provisional
  replenishment requirements.
- Correct FEFO terminology.
- Appropriate expiry-related stock management.
- Explicit food safety decision boundaries.
- More structured management reporting.

All numerical replenishment calculations remained
correct across both prompt versions.

## 8. Automation Potential

Classification: Medium.

AI can assist with inventory record validation,
measurement conversions, replenishment calculations,
expiry alerts and draft purchasing recommendations.

However, inventory staff must verify physical
stock, ingredient condition, batch information
and purchasing requirements.

AI must not independently authorise ingredient
use, food safety decisions or supplier orders.

## 9. Potential Business Value

| Business Area | Potential Benefit |
|---|---|
| Inventory Management | Clearer understanding of eligible stock |
| Procurement | More transparent purchasing requirements |
| Food Waste | Reduced risk of unnecessary purchasing |
| Production Planning | Earlier identification of ingredient shortages |
| Quality Assurance | Improved visibility of expired and unverified batches |
| Management | More structured decision-support reports |

Actual cost savings, time savings, reductions
in food waste and commercial improvements
have not been measured.

## 10. Risks and Limitations

| Risk or Limitation | Mitigation |
|---|---|
| Incorrect inventory records | Verify physical stock |
| Missing measurement units | Hold stock records for verification |
| Expired ingredients | Exclude from production |
| Missing expiry information | Require appropriate human review |
| Changes to production dates | Reassess stock eligibility |
| Provisional purchasing needs | Recalculate after inventory verification |
| Subjective action priorities | Establish approved priority rules |
| Supplier uncertainty | Verify pricing, availability and lead times |
| AI over-reliance | Require human approval |

Some repeated information remains in the reports.

Additional purchasing constraints, invalid
numerical inputs and repeat-run reliability
have not been directly tested.

## 11. Human-in-the-Loop Requirements

Responsible inventory and procurement personnel must:

1. Verify physical inventory and batch records.
2. Confirm ingredient storage and condition.
3. Review expired and held inventory.
4. Verify replenishment calculations.
5. Confirm supplier availability and delivery.
6. Approve final purchasing requirements.

Disposal and ingredient suitability decisions
must follow approved food safety procedures.

## 12. Critical Reflection

The initial prompt generated correct numerical
inventory calculations but did not consistently
distinguish established replenishment requirements
from provisional purchasing quantities.

The revised prompt introduced explicit eligibility
and purchasing classification rules.

This improved management visibility without
changing the underlying replenishment calculations.

Minor subjective priority classifications remain,
demonstrating that AI-generated reports still
require appropriate human interpretation.

## 13. Final Recommendation

Version v1.1 is selected as the final P02 prompt.

It is recommended for supervised ingredient
inventory assessment and replenishment planning.

Automation potential remains Medium.

No further refinement is required within the
current academic testing scope.

The prompt has not been commercially deployed.

## 14. Supporting Evidence

- [Final Prompt](../02-prompt-library/P02-inventory-and-replenishment.md)
- [Testing Evidence](../03-testing-evidence/P02-testing-evidence.md)
- [Iteration History](../04-iteration-logs/P02-iteration-log.md)
- [Evaluation Index](README.md)
- [Main Portfolio](../README.md)

---

**Final Status: P02 Completed — Version v1.1**

Final evaluation score: 19/20 (95%).
