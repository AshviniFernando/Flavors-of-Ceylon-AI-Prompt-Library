# P04 — Food Production and Batch Planning: Testing Evidence

## 1. Testing Information

| Detail | Information |
|---|---|
| Prompt ID | P04 |
| Business | Flavors of Ceylon |
| Business Function | Production Management |
| Initial Version | v1.0 |
| Data Type | Synthetic business data |
| Testing Status | In Progress |

## 2. Testing Objective

Evaluate whether AI can develop feasible production
schedules using approved production targets,
available ingredients, batch capacities, staffing
and shared production resources.

Testing evaluates numerical accuracy, batch
allocation, resource limitations, production
priorities and responsible manufacturing decisions.

## 3. Business Workflow Connection

Production targets are based on P01 Test C.

Ingredient availability and purchasing information
are connected to the P02 and P03 workflows.

Only verified and available ingredients may be
allocated to production.

Draft purchase orders and unconfirmed deliveries
must not be treated as available inventory.

---

## 4. Test Case A — Standard Production Scenario

### Test Input

[Paste the complete original Test A dataset.]

### Expected Output

- Achieve the approved production targets.
- Calculate feasible batch allocations.
- Respect ingredient availability.
- Respect staffing and production time limits.
- Avoid unnecessary vegetable roll production.
- Present a feasible production schedule.
- Maintain human approval requirements.

## 5. Test Case B — Constrained Production Scenario

### Test Input

[Paste the complete original Test B dataset.]

### Expected Output

- Exclude unconfirmed supplier deliveries.
- Identify ingredient and staffing constraints.
- Respect the approved production priority order.
- Calculate feasible production quantities.
- Identify unmet production targets.
- Prevent overlapping resource allocations.
- Maintain food safety and approval safeguards.

---

## 6. Version v1.0 — Initial Testing

### Test Case A

Testing date: Pending.

AI tool and model: Pending.

#### Actual AI Output

Pending testing.

#### Evaluation

Pending evaluation.

### Test Case B

Testing date: Pending.

AI tool and model: Pending.

#### Actual AI Output

Pending testing.

#### Evaluation

Pending evaluation.

---

## 7. Version v1.1 — Revised Testing

### Test Case A

Testing date: Pending.

AI tool and model: Pending.

#### Actual AI Output

Pending testing.

#### Evaluation

Pending evaluation.

### Test Case B

Testing date: Pending.

AI tool and model: Pending.

#### Actual AI Output

Pending testing.

#### Evaluation

Pending evaluation.

---

## 8. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---|---|---|
| v1.0 | Pending | Pending | Pending |
| v1.1 | Pending | Pending | Pending |

## 9. Testing Integrity

All production quantities, ingredient consumption
rates, batch capacities, staffing records and
operational restrictions are synthetic.

Expected answers must not be supplied to the AI
during testing.

Actual AI responses must be retained without
retrospective modification.

Production schedules remain subject to management
approval and approved food safety procedures.

## Related Evidence

- [P04 Prompt](../02-prompt-library/P04-production-and-batch-planning.md)
- [P01 Final Evaluation](../05-evaluation/P01-final-evaluation.md)
- [P02 Final Evaluation](../05-evaluation/P02-final-evaluation.md)
- [P03 Final Evaluation](../05-evaluation/P03-final-evaluation.md)
- [Testing Evidence Index](README.md)
