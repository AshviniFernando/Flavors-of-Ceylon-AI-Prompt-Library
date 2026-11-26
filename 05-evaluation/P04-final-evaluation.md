# P04 — Food Production and Batch Planning: Final Evaluation

## 1. Evaluation Information

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Food Manufacturing and Hospitality |
| Prompt ID | P04 |
| Business Function | Production Management |
| Initial Version | v1.0 |
| Final Selected Version | v1.1 |
| Evaluation Status | Completed |
| Data Type | Synthetic business data |
| Automation Potential | Medium |
| Operational Deployment | Not implemented |

## 2. Evaluation Objective and Methodology

Evaluate the ability of generative AI to develop
feasible production schedules using approved
production targets, verified ingredient inventory,
batch capacities, staffing and shared resources.

Two synthetic scenarios were used:

- Test A: Complete production information with
  sufficient ingredients, staffing and capacity.
- Test B: Ingredient shortages, unconfirmed supplier
  deliveries and restricted staffing and capacity.

Both prompt versions were tested using the same
original datasets without supplying expected answers.

Actual responses were compared with independently
established numerical benchmarks.

The evaluation considered accuracy, completeness,
consistency, business relevance and responsible AI,
using a zero-to-two scoring scale for each criterion.

## 3. Prompting Strategies

- Role-based prompting.
- Contextual prompting.
- Constraint-based prompting.
- Task decomposition.
- Explicit mathematical instructions.
- Priority-based resource allocation.
- Structured-output prompting.
- Human-in-the-loop decision support.

## 4. Version Performance

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 9/10 | 18/20 (90%) |
| v1.1 | 9/10 | 10/10 | 19/20 (95%) |

Absolute improvement: 5 percentage points.

Relative improvement in evaluation score: 5.56%.

## 5. Final Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 2 |
| Business Relevance | 1 | 2 |
| Responsible AI | 2 | 2 |
| Total | 9/10 | 10/10 |

Final combined score: 19/20 (95%).

The Test A business relevance deduction reflects
remaining repetition in the standard scenario.

The score represents response quality under
selected synthetic scenarios rather than
actual commercial manufacturing performance.

## 6. Key Testing Results

### Test A — Standard Production Scenario

| Product | Approved Target | Proposed Quantity | Batch Allocation | Minutes |
|---|---:|---:|---|---:|
| Fish roti | 120 | 120 | 6 x 20 | 240 |
| Chicken kottu | 85 | 85 | 4 x 20 + 1 x 5 | 225 |
| Rice and curry packs | 50 | 50 | 2 x 25 | 100 |
| Pol sambol sachets | 70 | 70 | 2 x 35 | 60 |
| Vegetable rolls | 0 | 0 | None | 0 |
| Total | 325 | 325 | 15 batches | 625 |

| Performance Indicator | Result |
|---|---|
| Approved production target | 325 units |
| Feasible production | 325 units |
| Unmet production target | 0 units |
| Target achievement | 100% |
| Scheduled production time | 625 minutes |
| Feasible available time | 1,080 minutes |
| Remaining capacity | 455 minutes |
| Capacity utilisation | 57.87% |
| Scheduled staff requirement | 1,250 staff-minutes |

All approved production targets were achieved
within the proposed synthetic schedule.

No ingredient shortages, overlapping batches,
additional staff or overtime were required.

### Test B — Constrained Production Scenario

| Product | Approved Target | Proposed Quantity | Shortfall | Binding Constraint |
|---|---:|---:|---:|---|
| Fish roti | 120 | 100 | 20 | Fish availability |
| Chicken kottu | 85 | 40 | 45 | Remaining wheat flour |
| Rice and curry packs | 50 | 10 | 40 | Chicken availability and batch increments |
| Pol sambol sachets | 70 | 35 | 35 | Remaining production time |
| Vegetable rolls | 0 | 0 | 0 | Zero approved target |
| Total | 325 | 185 | 140 | |

| Performance Indicator | Result |
|---|---|
| Approved production target | 325 units |
| Feasible production | 185 units |
| Unmet production target | 140 units |
| Target achievement | 56.92% |
| Production batches | 9 |
| Full-target minimum production time | 625 minutes |
| Feasible available production time | 375 minutes |
| Scheduled production time | 370 minutes |
| Remaining feasible time | 5 minutes |
| Capacity utilisation | 98.67% |
| Minimum full-target capacity deficit | 250 minutes |
| Unconfirmed deliveries included | None |

Production was scheduled only on 5 December
because the remaining dates could not satisfy
the concurrent staffing requirements.

The 140-unit shortfall represents unmet approved
production targets, not confirmed unmet customer
demand.

### Ingredient Reconciliation

| Ingredient | Test A Consumption | Test A Remaining | Test B Consumption | Test B Remaining |
|---|---:|---:|---:|---:|
| Wheat flour | 31.4 kg | 13.6 kg | 20 kg | 0 kg |
| Rice | 7.5 kg | 32.5 kg | 1.5 kg | 13.5 kg |
| Chicken | 25.3 kg | 4.7 kg | 9.2 kg | 0.8 kg |
| Grated coconut | 5 kg | 7 kg | 2.05 kg | 1.95 kg |
| Fish | 9.6 kg | 2.4 kg | 8 kg | 0 kg |
| Vegetables | 0 kg | 10 kg | 0 kg | 10 kg |
| Eggs | 85 units | 15 units | 40 units | 20 units |

All ingredient balances matched the expected
results and remained non-negative.

## 7. Observed Improvements

Compared with v1.0, the revised prompt demonstrated:

- More structured production reporting.
- Explicit priority-based resource allocation.
- Consolidated ingredient reconciliation.
- Clearer daily staffing and capacity validation.
- Evidence-based bottleneck descriptions.
- Removal of unsupported risk classifications.
- Removal of unnecessary visualisations.
- Retention of correct numerical calculations.

### Reporting Structure Improvement

| Scenario | v1.0 Principal Sections | v1.1 Principal Sections | Reduction |
|---|---:|---:|---:|
| Test A | 13 | 5 | 61.54% |
| Test B | 18 | 5 | 72.22% |

These percentages measure principal report section
counts rather than document word counts or
administrative time savings.

Some repeated information remains.

## 8. Business Workflow Integration

P04 connects the preceding planning and
procurement prompts:

- P01 provides demand estimates and indicative
  production quantities.
- P02 assesses eligible ingredient inventory
  and replenishment requirements.
- P03 prepares draft procurement documents.
- Human personnel approve purchasing, verify
  received ingredients and approve production targets.
- P04 develops a proposed production schedule
  using verified available resources.

Draft purchase orders and unconfirmed supplier
deliveries must not be treated as available stock.

The proposed schedules may subsequently support
production monitoring and P05 food safety and
quality incident documentation.

## 9. Automation Potential

Classification: Medium.

AI can assist with production calculations,
batch allocation, ingredient reconciliation,
capacity assessment and draft scheduling.

However, real manufacturing operations require
verified inventory, staff qualifications,
equipment readiness, approved production
procedures and management authorisation.

AI should support planning rather than
independently control manufacturing operations.

## 10. Potential Business Value

| Business Area | Potential Benefit |
|---|---|
| Production Planning | More structured production schedules |
| Inventory Management | Reduced risk of duplicate ingredient allocation |
| Staffing | Earlier identification of staffing limitations |
| Capacity Management | Better visibility of available production time |
| Procurement | Identification of ingredient shortages |
| Food Waste | Improved allocation of verified ingredients |
| Management | Clearer production shortfall reporting |

Actual reductions in production costs, food waste,
administrative time and production delays have
not been measured.

## 11. Risks and Limitations

| Risk or Limitation | Mitigation |
|---|---|
| Incorrect ingredient records | Verify available inventory |
| Unconfirmed supplier deliveries | Exclude until received and verified |
| Incorrect recipe calculations | Use approved recipes and independent checks |
| Insufficient staffing | Verify concurrent staffing requirements |
| Overlapping batches | Validate shared resource schedules |
| Equipment failure | Confirm readiness and reassess affected schedules |
| Missing production information | Withhold affected allocations |
| Repeated reporting information | Use approved management templates |
| Food safety concerns | Follow approved procedures |
| Unauthorised production | Require production manager approval |

Multiple production stations, invalid recipes,
complex staffing restrictions and dynamic
rescheduling have not been directly tested.

Repeat-run reliability remains unverified.

## 12. Human-in-the-Loop Requirements

Responsible production personnel must:

1. Verify approved production targets.
2. Confirm physical ingredient availability.
3. Verify ingredient condition and eligibility.
4. Confirm staffing and equipment readiness.
5. Independently review batch allocations,
   calculations and scheduling constraints.
6. Confirm applicable food safety, storage
   and quality requirements.
7. Approve the production schedule before
   implementation.

AI must not independently approve ingredient
suitability, certify food safety or authorise
manufacturing activities.

## 13. Critical Reflection

The initial prompt generated correct numerical
production allocations but produced lengthy
reports containing repeated information.

The revised prompt introduced explicit allocation,
reconciliation and scheduling validation rules.

Both versions achieved the same numerical
production outputs under the tested conditions.

The improvement therefore relates primarily to
reporting structure, allocation transparency
and operational decision support.

The remaining repetition demonstrates that
structured-output instructions do not necessarily
eliminate all unnecessary content.

## 14. Final Recommendation

Version v1.1 is selected as the final P04 prompt.

It is recommended for supervised food production
planning, batch allocation and resource assessment.

Automation potential remains Medium.

The remaining minor limitations do not justify
further refinement within the current
academic testing scope.

The prompt has not been commercially deployed.

## 15. Supporting Evidence

- [Final Prompt](../02-prompt-library/P04-production-and-batch-planning.md)
- [Testing Evidence](../03-testing-evidence/P04-testing-evidence.md)
- [Iteration History](../04-iteration-logs/P04-iteration-log.md)
- [P01 Final Evaluation](P01-final-evaluation.md)
- [P02 Final Evaluation](P02-final-evaluation.md)
- [P03 Final Evaluation](P03-final-evaluation.md)
- [Evaluation Index](README.md)
- [Main Portfolio](../README.md)

---

**Final Status: P04 Completed — Version v1.1**

Final evaluation score: 19/20 (95%).
