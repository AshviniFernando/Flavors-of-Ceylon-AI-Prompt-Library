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

Testing date: 25 November 2026

AI tool and model: ChatGPT

#### Actual AI Output

# Flavors of Ceylon – Inventory Management Analysis

## 1. Inventory Review Overview

| Review Details | Information |
|---|---|
| Business | Flavors of Ceylon |
| Inventory Review Date | 1 December 2026 |
| Production Planning Period | 1–7 December 2026 |
| Objective | Identify ingredient shortages, excess stock and expiry risks to support production planning |

## 2. Inventory Assessment and Replenishment Recommendations

All existing ingredients have passed the stated storage and condition checks, and their planned usage dates fall within their respective usable-through dates.

| Ingredient | Current Usable Stock | Required Quantity | Stock Balance | Inventory Status | Recommended Replenishment |
|---|---:|---:|---:|---|---:|
| Wheat flour | 30 kg | 45 kg | -15 kg | Shortage | 15 kg |
| Rice | 40 kg | 25 kg | +15 kg | Excess stock | 0 kg |
| Chicken | 18 kg | 30 kg | -12 kg | Shortage and expiry attention | 12 kg |
| Grated coconut | 12 kg | 12 kg | 0 kg | Sufficient stock but expiry attention | 0 kg |
| Eggs | 100 units | 80 units | +20 units | Excess stock | 0 units |

## 3. Expiry Assessment and Stock Management Actions

| Ingredient | Usable-Through Date | Planned Usage Date | Expiry Attention | Recommended Action |
|---|---|---|---|---|
| Wheat flour | 31 Dec 2026 | 5 Dec 2026 | No | Purchase 15 kg before planned production. |
| Rice | 31 Dec 2026 | 5 Dec 2026 | No | Retain the remaining 15 kg for future production. Avoid unnecessary purchasing. |
| Chicken | 6 Dec 2026 | 5 Dec 2026 | Yes | Prioritise existing stock for production on 5 December. Purchase an additional 12 kg of verified suitable stock. |
| Grated coconut | 3 Dec 2026 | 2 Dec 2026 | Yes | Prioritise all 12 kg for production on 2 December. Monitor any changes to the production schedule. |
| Eggs | 12 Dec 2026 | 5 Dec 2026 | No – outside the planning period | Retain the remaining 20 eggs and monitor their usable-through date. |

## 4. Inventory Summary

| Performance Indicator | Result |
|---|---|
| Total ingredients reviewed | 5 |
| Ingredients with shortages | 2 |
| Ingredients with excess stock | 2 |
| Ingredients requiring expiry attention | 2 |
| Ingredients requiring replenishment | 2 |
| Total replenishment required | 27 kg |

### Stock Shortages

- Wheat flour: 15 kg
- Chicken: 12 kg

### Excess Stock

- Rice: 15 kg
- Eggs: 20 units

### Ingredients Requiring Expiry Attention

- Chicken – usable through 6 December 2026.
- Grated coconut – usable through 3 December 2026.

Both ingredients are scheduled for use before their respective usable-through dates. However, any production delays must trigger a reassessment of their suitability.

## 5. Replenishment Calculations

The following calculation is used:

**Stock balance = Current usable stock - Required quantity**

**Recommended replenishment = Maximum of zero or (Required quantity - Current usable stock)**

| Ingredient | Calculation | Recommended Replenishment |
|---|---|---:|
| Wheat flour | 45 - 30 | 15 kg |
| Rice | Maximum of zero or (25 - 40) | 0 kg |
| Chicken | 30 - 18 | 12 kg |
| Grated coconut | 12 - 12 | 0 kg |
| Eggs | Maximum of zero or (80 - 100) | 0 units |

**Total recommended replenishment: 15 kg + 12 kg = 27 kg**

## 6. Missing Information

The supplied information is sufficient to calculate replenishment quantities. However, the following additional information would support purchasing and operational decisions:

- Supplier availability and delivery lead times.
- Ingredient purchasing prices and procurement budget.
- Storage and condition verification for newly purchased ingredients.
- Usable-through dates of newly purchased ingredients.
- Future production requirements for remaining rice and eggs.
- Procedures for handling ingredients if planned production is delayed beyond their usable-through dates.

## 7. Assumptions and Limitations

- All existing inventory is considered usable for the stated planned usage dates based on the supplied scenario.
- Required quantities represent approved production requirements.
- No incoming purchase orders apply.
- No minimum order quantities apply.
- No additional safety stock requirements apply.
- Replenishment quantities cannot be negative.
- Excess stock represents quantities exceeding the approved requirements for the current planning period, rather than confirmed long-term overstocking.
- Ingredients with usable-through dates within the planning period require expiry-related attention.
- Newly purchased ingredients must undergo appropriate storage, condition and expiry verification before production.
- Expired or unverified ingredients must not be assumed suitable for production.
- All supplied dates and quantities are synthetic and do not constitute actual food safety determinations.
- Human verification is required before implementing AI-generated recommendations.

## 8. Final Recommendation

Flavors of Ceylon should replenish **15 kg of wheat flour and 12 kg of chicken** before production on 5 December 2026.

The total recommended replenishment quantity is **27 kg**.

Chicken and grated coconut should receive expiry-related attention using the **First Expired, First Out (FEFO)** inventory management approach, which prioritises suitable ingredients with the earliest usable-through dates.

Additional purchases of rice, grated coconut and eggs are unnecessary for the current planning period.

The remaining 15 kg of rice and 20 eggs should be monitored and allocated to suitable future production requirements.

All recommendations should be reviewed and approved by the responsible inventory or production manager before purchasing or production activities proceed.

---

**Business:** Flavors of Ceylon

**Workflow:** Ingredient Inventory Management and Replenishment Planning

**Data Classification:** Synthetic Test Data

**Output Type:** AI-Generated Inventory Analysis

**Human Review Required:** Yes

#### Evaluation

Pending evaluation.

### Test Case B

Testing date: 25 November 2026

AI tool and model: ChatGPT

#### Actual AI Output

# Flavors of Ceylon – Ingredient Inventory Management Report

## 1. Inventory Review Overview

- **Inventory Review Date:** 1 December 2026
- **Production Planning Period:** 1–7 December 2026
- **Scheduled Production Date:** 5 December 2026
- **Business:** Flavors of Ceylon
- **Data Type:** Synthetic business data

The inventory assessment considers ingredient quantities, measurement unit consistency, usable-through dates and suitability for scheduled production.

Expired ingredients, ingredients with missing expiry information and quantities with unverified measurement units are excluded from confirmed usable inventory.

---

## 2. Batch-Level Inventory Assessment

| Ingredient | Batch | Recorded Stock | Usable-Through Date | Assessment | Recommended Action |
|---|---|---|---|---|---|
| Wheat flour | F01 | 12 kg | 31 Dec 2026 | Usable | Allocate to production. |
| Wheat flour | F02 | 8000 g | 31 Dec 2026 | Usable after unit conversion | Convert to 8 kg and allocate to production. |
| Rice | R01 | 15 kg | 31 Dec 2026 | Usable | Allocate to production. |
| Rice | R02 | 10 (unknown unit) | 31 Dec 2026 | Unverified quantity | Hold until the measurement unit is confirmed. |
| Chicken | C01 | 10 kg | 6 Dec 2026 | Usable but approaching expiry | Prioritise for production, subject to final checks. |
| Chicken | C02 | 8 kg | 30 Nov 2026 | Expired | Segregate and arrange safe disposal. |
| Chicken | C03 | 5 kg | Missing | Unverified expiry | Quarantine until expiry information is verified. |
| Grated coconut | G01 | 6 kg | 2 Dec 2026 | Expires before production | Exclude from scheduled production. Consider approved earlier use before expiry or safe disposal. |
| Grated coconut | G02 | 4 kg | 6 Dec 2026 | Usable but approaching expiry | Prioritise for production, subject to final checks. |
| Eggs | E01 | 60 units | 12 Dec 2026 | Usable with excess stock | Allocate 48 units and monitor the remaining 12 units. |

---

## 3. Ingredient Requirements and Replenishment Recommendations

Replenishment quantities are calculated using confirmed usable inventory rather than total recorded stock.

**Formula:**

Replenishment Quantity = Maximum of (0, Required Quantity − Confirmed Usable Stock)

| Ingredient | Required Quantity | Confirmed Usable Stock | Excluded or Unverified Stock | Shortage | Excess | Recommended Purchase |
|---|---:|---:|---|---:|---:|---:|
| Wheat flour | 25 kg | 20 kg | None | 5 kg | 0 kg | 5 kg |
| Rice | 20 kg | 15 kg | 10 (unknown unit) | 5 kg | 0 kg | 5 kg |
| Chicken | 25 kg | 10 kg | 13 kg | 15 kg | 0 kg | 15 kg |
| Grated coconut | 10 kg | 4 kg | 6 kg | 6 kg | 0 kg | 6 kg |
| Eggs | 48 units | 60 units | None | 0 units | 12 units | 0 units |

---

## 4. Inventory Availability Analysis

**Formula:**

Inventory Availability (%) = (Confirmed Usable Stock / Required Quantity) × 100

| Ingredient | Confirmed Usable Stock | Required Quantity | Availability | Status |
|---|---:|---:|---:|---|
| Wheat flour | 20 kg | 25 kg | 80% | Shortage |
| Rice | 15 kg | 20 kg | 75% | Shortage |
| Chicken | 10 kg | 25 kg | 40% | Significant shortage |
| Grated coconut | 4 kg | 10 kg | 40% | Significant shortage |
| Eggs | 60 units | 48 units | 125% | Excess stock |

Chicken and grated coconut have the most significant proportional shortages, with only 40% of their production requirements covered by confirmed usable inventory.

---

## 5. Recommended Purchasing Plan

| Ingredient | Recommended Purchase Quantity | Priority |
|---|---:|---|
| Chicken | 15 kg | High |
| Grated coconut | 6 kg | High |
| Wheat flour | 5 kg | Medium |
| Rice | 5 kg | Medium |
| Eggs | 0 units | No purchase required |
| **Total** | **31 kg** | **Human approval required** |

All proposed purchases should arrive before scheduled production on 5 December 2026 and have verified usable-through dates covering the production date.

The recommended rice and chicken purchase quantities should be recalculated if the unverified batches are successfully validated before purchasing approval.

No purchase orders should be placed without human approval.

---

## 6. Expiry Risk Assessment

| Batch | Ingredient | Usable-Through Date | Risk Level | Reason |
|---|---|---|---|---|
| C02 | Chicken | 30 Nov 2026 | Critical | Already expired on the review date. |
| C03 | Chicken | Missing | High | Expiry and production eligibility cannot be confirmed. |
| G01 | Grated coconut | 2 Dec 2026 | High | Expires before scheduled production. |
| C01 | Chicken | 6 Dec 2026 | Medium | Reaches usable-through date one day after production. |
| G02 | Grated coconut | 6 Dec 2026 | Medium | Reaches usable-through date one day after production. |
| E01 | Eggs | 12 Dec 2026 | Low | Suitable for scheduled production, but excess stock requires monitoring. |

The business should implement the **First Expired, First Out (FEFO)** inventory management method, prioritising verified and suitable ingredients with the earliest usable-through dates.

Expired ingredients must not be used under the FEFO method.

---

## 7. Missing Information and Data Limitations

| Missing Information | Affected Inventory | Required Action |
|---|---|---|
| Measurement unit | Rice – R02 | Confirm the recorded measurement unit and convert to kilograms if appropriate. |
| Usable-through date | Chicken – C03 | Obtain reliable batch expiry documentation before approving use. |
| Supplier lead times | All replenishment ingredients | Confirm delivery before scheduled production. |
| Supplier prices | All replenishment ingredients | Obtain quotations for purchasing approval. |
| Purchasing authorisation | Proposed purchase orders | Obtain approval from the responsible manager. |

---

## 8. Recommended Inventory Management Actions

- Immediately segregate the expired chicken batch C02 and arrange safe disposal.
- Quarantine chicken batch C03 until its expiry information is verified.
- Hold rice batch R02 until its measurement unit is confirmed.
- Exclude grated coconut batch G01 from the scheduled production requirements.
- Standardise ingredient measurement units in inventory records.
- Apply the FEFO method to verified and suitable inventory.
- Prioritise chicken batch C01 and grated coconut batch G02 for scheduled production, subject to final checks.
- Monitor the remaining 12 eggs to minimise future food waste.
- Recheck ingredient condition, storage compliance and expiry information before production.
- Confirm supplier delivery schedules.
- Obtain human approval before placing replenishment orders.

---

## 9. Assumptions and Limitations

- The assessment uses only the supplied synthetic business data.
- All ingredients are required for production on 5 December 2026.
- Wheat flour batch F02 is converted from 8000 g to 8 kg.
- No incoming purchase orders are scheduled.
- No additional safety stock requirements apply.
- No minimum order quantity requirements apply.
- Expired ingredients are excluded from confirmed usable inventory.
- Ingredients expiring before the scheduled production date are excluded.
- Ingredients with missing expiry information are excluded until verified.
- Ingredients with unverified measurement units are excluded until verified.
- Risk and purchasing priority classifications are qualitative planning assessments rather than formally defined business thresholds.
- Ingredients classified as usable remain subject to appropriate storage and final production checks.
- All purchasing recommendations require human approval.
- No missing measurement units or expiry dates have been invented.

---

## 10. Conclusion

Flavors of Ceylon faces confirmed shortages of wheat flour, rice, chicken and grated coconut, while eggs have an excess stock of 12 units.

A provisional replenishment of **31 kg of ingredients** is recommended to meet the scheduled production requirements on 5 December 2026.

The recommended replenishment quantities are:

- Wheat flour: 5 kg
- Rice: 5 kg
- Chicken: 15 kg
- Grated coconut: 6 kg
- Eggs: 0 units

Expired, unverified and unsuitable batches must remain excluded unless eligible unverified stock is subsequently validated.

All purchasing recommendations are subject to human review and approval to support food safety, production continuity, inventory accuracy and waste reduction.

---

**End of Report**

**Disclaimer:** This report is based entirely on synthetic business data and is prepared for academic AI prompt testing purposes.

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
