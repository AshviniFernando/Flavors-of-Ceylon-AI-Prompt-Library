# P02 — Ingredient Inventory and Replenishment: Testing Evidence

## 1. Testing Information

| Detail | Information |
|---|---|
| Prompt ID | P02 |
| Business | Flavors of Ceylon |
| Business Function | Inventory Management |
| Initial Version | v1.0 |
| Data Type | Synthetic business data |
| Testing Status | In Progress |

## 2. Testing Objective

Evaluate whether the AI can identify ingredient
shortages, excess inventory, expiry-related risks
and appropriate replenishment quantities.

Testing also evaluates missing information,
measurement unit consistency and responsible
inventory management recommendations.

---

## 3. Test Case A — Standard Inventory Scenario

### Test Input

Inventory review date: 1 December 2026.

Production planning period: 1–7 December 2026.

| Ingredient | Current Stock | Required Quantity | Usable-Through Date | Planned Usage Date |
|---|---:|---:|---|---|
| Wheat flour | 30 kg | 45 kg | 31 Dec 2026 | 5 Dec 2026 |
| Rice | 40 kg | 25 kg | 31 Dec 2026 | 5 Dec 2026 |
| Chicken | 18 kg | 30 kg | 6 Dec 2026 | 5 Dec 2026 |
| Grated coconut | 12 kg | 12 kg | 3 Dec 2026 | 2 Dec 2026 |
| Eggs | 100 units | 80 units | 12 Dec 2026 | 5 Dec 2026 |

All existing stock has passed the relevant internal
storage and condition checks for this scenario.

Required quantities are approved production requirements.

No incoming purchase orders, minimum order quantities
or additional safety stock requirements apply.

Ingredients with usable-through dates within the
planning period require expiry-related attention.

All dates and quantities are synthetic and are
not real food safety determinations.

### Expected Output

- Identify ingredient shortages correctly.
- Calculate replenishment quantities.
- Identify stock exceeding production requirements.
- Flag ingredients approaching their usable-through dates.
- Recommend appropriate stock management actions.
- Avoid unsupported food safety guarantees.

---

## 4. Test Case B — Challenging Inventory Scenario

### Test Input

Inventory review date: 1 December 2026.

Production planning period: 1–7 December 2026.

All ingredients are required for production
on 5 December 2026.

### Approved Production Requirements

| Ingredient | Required Quantity |
|---|---:|
| Wheat flour | 25 kg |
| Rice | 20 kg |
| Chicken | 25 kg |
| Grated coconut | 10 kg |
| Eggs | 48 units |

### Current Inventory Records

| Ingredient | Batch | Stock Quantity | Usable-Through Date |
|---|---|---|---|
| Wheat flour | F01 | 12 kg | 31 Dec 2026 |
| Wheat flour | F02 | 8000 g | 31 Dec 2026 |
| Rice | R01 | 15 kg | 31 Dec 2026 |
| Rice | R02 | 10 (unit missing) | 31 Dec 2026 |
| Chicken | C01 | 10 kg | 6 Dec 2026 |
| Chicken | C02 | 8 kg | 30 Nov 2026 |
| Chicken | C03 | 5 kg | Missing |
| Grated coconut | G01 | 6 kg | 2 Dec 2026 |
| Grated coconut | G02 | 4 kg | 6 Dec 2026 |
| Eggs | E01 | 60 units | 12 Dec 2026 |

Additional information:

- Batch C02 has passed its usable-through date.
- Batch C03 has missing expiry information.
- Batch R02 has an unverified measurement unit.
- Batch G01 reaches its usable-through date before
  the scheduled production date.
- Other batches have passed the relevant internal
  storage and condition checks for this scenario.
- No incoming purchase orders are scheduled.
- No additional safety stock or minimum order
  quantity requirements apply.
- Purchasing decisions require human approval.

All information is synthetic.

### Expected Output

- Correctly convert compatible measurement units.
- Identify expired stock and missing expiry information.
- Identify stock unavailable for the planned usage date.
- Exclude unverified stock from confirmed usable inventory.
- Do not assume missing measurement units.
- Calculate replenishment requirements using verified
  eligible stock.
- Clearly distinguish provisional purchasing needs.
- Recommend human review of food safety concerns.

---

## 5. Version v1.0 — Initial Testing

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

## 6. Version v1.1 — Revised Testing

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

## 7. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---|---|---|
| v1.0 | Pending | Pending | Pending |
| v1.1 | Pending | Pending | Pending |

## 8. Testing Integrity

All inventory records, dates and production
requirements are fictional and created for
academic testing.

Expected answers must not be supplied to the AI
when conducting tests.

Actual responses must be retained without
retrospective modification.

Food safety decisions and supplier purchasing
commitments require appropriate human approval.

## Related Evidence

- [P02 Prompt](../02-prompt-library/P02-inventory-and-replenishment.md)
- [Testing Evidence Index](README.md)
