# P02 — Ingredient Inventory and Replenishment: Testing Evidence

## 1. Testing Information

| Detail | Information |
|---|---|
| Prompt ID | P02 |
| Business | Flavors of Ceylon |
| Business Function | Inventory Management |
| Initial Version | v1.0 |
| Data Type | Synthetic business data |
| Testing Status | Completed — v1.1 Selected |

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

The v1.0 response correctly calculated replenishment
requirements of 15 kg of wheat flour and 12 kg of
chicken, resulting in a total of 27 kg.

It correctly identified surplus rice and eggs and
flagged chicken and grated coconut for expiry
attention.

All numerical calculations were correct.

However, the response used the terminology
"First Expired, First Out" instead of the preferred
"First Expiry, First Out" terminology.

The report also contained repeated calculations
and recommendations.

Evaluation score: 9/10 (90%).

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

The response correctly converted measurement units,
excluded expired ingredients and held unverified
stock pending verification.

All replenishment calculations were correct based
on confirmed eligible inventory.

The total indicative replenishment requirement
was 31 kg, including provisional rice and chicken
requirements.

However, the response inconsistently described
these shortages as confirmed while acknowledging
that purchasing quantities could change.

The response also used non-standardised risk
classifications and incorrect FEFO terminology.

The ten-section report contained repeated
information.

Evaluation score: 8/10 (80%).

---

## 6. Version v1.1 — Revised Testing

### Test Case A

Testing date: 25 November 2026

AI tool and model: ChatGPT

#### Actual AI Output


# Flavors of Ceylon – Ingredient Inventory and Replenishment Analysis

## Test Information

| Item | Details |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Australian Food Manufacturing |
| Prompt ID | P02 |
| Prompt Version | v1.1 |
| Test Scenario | Test A |
| Inventory Review Date | 1 December 2026 |
| Production Planning Period | 1–7 December 2026 |
| Data Type | Synthetic Business Data |

---

## 1. Data Validation

The supplied inventory records have been reviewed against the approved production requirements, measurement units, usable-through dates and planned usage dates.

| Validation Criteria | Findings | Status |
|---|---|---|
| Ingredient names | All five ingredients are clearly identified. | Valid |
| Inventory quantities | All quantities are provided and positive. | Valid |
| Measurement units | Stock and production requirement units are consistent. | Valid |
| Unit conversions | No conversions are required. | Valid |
| Usable-through dates | Dates are provided for all ingredients. | Valid |
| Planned usage dates | All usage dates fall within the planning period. | Valid |
| Storage and condition | All existing stock has passed the relevant internal checks. | Verified for this scenario |
| Production requirements | All required quantities are approved. | Valid |
| Batch records | Individual batch identification details are not supplied. | Limitation |
| Purchasing constraints | No incoming orders, minimum order quantities or additional safety stock requirements apply. | Confirmed |

**Validation Outcome:**

All supplied ingredient records are suitable for inventory planning calculations under the stated synthetic scenario. Missing batch identifiers represent a traceability limitation but do not prevent calculations at the supplied ingredient level.

---

## 2. Inventory Eligibility Assessment

| Ingredient | Current Stock | Usable-Through Date | Planned Usage Date | Eligibility Classification | Confirmed Eligible Stock |
|---|---:|---|---|---|---:|
| Wheat flour | 30 kg | 31 Dec 2026 | 5 Dec 2026 | Eligible | 30 kg |
| Rice | 40 kg | 31 Dec 2026 | 5 Dec 2026 | Eligible | 40 kg |
| Chicken | 18 kg | 6 Dec 2026 | 5 Dec 2026 | Eligible — Expiry Attention | 18 kg |
| Grated coconut | 12 kg | 3 Dec 2026 | 2 Dec 2026 | Eligible — Expiry Attention | 12 kg |
| Eggs | 100 units | 12 Dec 2026 | 5 Dec 2026 | Eligible | 100 units |

### Eligibility Findings

- **Eligible inventory:** All five ingredient records qualify for inclusion in the confirmed usable stock calculations under the supplied scenario.
- **Expiry attention:** Chicken and grated coconut have usable-through dates within the planning period.
- **Expired inventory:** None.
- **Inventory expiring before planned usage:** None.
- **Pending verification:** None, based on the supplied condition and storage verification.

These classifications support inventory planning and do not constitute independent food safety certification.

---

## 3. Replenishment Calculations

### 3.1 Calculation Formulas

**Stock Balance**

Stock Balance = Confirmed Eligible Stock − Approved Requirement

**Indicative Replenishment**

Indicative Replenishment = Max(0, Approved Requirement − Confirmed Eligible Stock)

**Surplus Stock**

Surplus Stock = Max(0, Confirmed Eligible Stock − Approved Requirement)

### 3.2 Ingredient Replenishment Table

| Ingredient | Eligible Stock | Approved Requirement | Stock Balance | Replenishment Calculation | Indicative Replenishment | Surplus Stock | Purchasing Classification |
|---|---:|---:|---:|---|---:|---:|---|
| Wheat flour | 30 kg | 45 kg | -15 kg | Max(0, 45 - 30) | 15 kg | 0 kg | Established requirement |
| Rice | 40 kg | 25 kg | +15 kg | Max(0, 25 - 40) | 0 kg | 15 kg | No replenishment required |
| Chicken | 18 kg | 30 kg | -12 kg | Max(0, 30 - 18) | 12 kg | 0 kg | Established requirement |
| Grated coconut | 12 kg | 12 kg | 0 kg | Max(0, 12 - 12) | 0 kg | 0 kg | No replenishment required |
| Eggs | 100 units | 80 units | +20 units | Max(0, 80 - 100) | 0 units | 20 units | No replenishment required |

### 3.3 Replenishment Subtotals

| Purchasing Classification | Kilograms (kg) | Individual Units |
|---|---:|---:|
| Established requirements | 27 kg | 0 units |
| Provisional requirements | 0 kg | 0 units |
| **Total indicative replenishment** | **27 kg** | **0 units** |

Kilograms and individual units are reported separately to avoid combining incompatible measurement units.

### 3.4 Surplus Stock Summary

| Ingredient | Surplus Quantity |
|---|---:|
| Rice | 15 kg |
| Eggs | 20 units |

The established replenishment requirements are not affected by unresolved inventory verification issues in this scenario. However, all purchasing quantities remain subject to inventory or procurement manager approval.

---

## 4. Stock Management Actions and Limitations

### 4.1 Recommended Stock Management Actions

| Ingredient | Inventory Issue | Recommended Stock Management Action |
|---|---|---|
| Wheat flour | Shortage | Submit the replenishment requirement for approval and ensure additional stock is verified before production. |
| Rice | Surplus stock | Retain the surplus under approved storage conditions and apply FEFO rotation for future production. |
| Chicken | Shortage and expiry attention | Prioritise existing eligible stock for production on 5 December and obtain approval for replenishment. |
| Grated coconut | Expiry attention and no stock buffer | Prioritise existing stock for production on 2 December. Monitor any production schedule changes. |
| Eggs | Surplus stock | Apply FEFO rotation and monitor remaining stock against its usable-through date. |

### 4.2 Operational Limitations and Controls

| Area | Limitation or Required Control |
|---|---|
| Batch traceability | Individual batch identifiers are unavailable. Obtain these records for operational traceability. |
| Supplier information | Supplier prices, delivery lead times and availability are not supplied. Purchasing feasibility cannot be confirmed. |
| Production schedule changes | Reassess inventory eligibility if planned usage dates change. |
| FEFO rotation | Apply First Expiry, First Out to verified and eligible inventory. |
| Expired inventory | Do not allocate expired ingredients to production. |
| Unverified inventory | Hold for appropriate inspection and authorisation. |
| Disposal or alternative use | Refer decisions to responsible personnel under approved food safety procedures. |
| Human oversight | Inventory suitability and purchasing decisions require authorised personnel. |

---

## 5. Management Summary and Priority Actions

### 5.1 Key Inventory Findings

| Performance Indicator | Result |
|---|---|
| Established replenishment | 27 kg |
| Provisional replenishment | 0 kg and 0 units |
| Ingredients with shortages | 2 — Wheat flour and chicken |
| Ingredients requiring expiry attention | 2 — Chicken and grated coconut |
| Ingredients with surplus stock | 2 — Rice and eggs |
| Expired ingredient records | 0 |
| Ingredient records pending verification | 0 |

### 5.2 Management Summary

The inventory analysis identifies two ingredient shortages, two surplus ingredients and two ingredients requiring expiry attention. All existing stock qualifies for planning calculations under the supplied scenario.

### 5.3 Priority Actions

1. Obtain procurement approval for 15 kg of wheat flour and 12 kg of chicken.
2. Prioritise chicken and grated coconut according to their scheduled usage dates.
3. Manage surplus rice and eggs through FEFO rotation.
4. Obtain batch traceability records and confirm supplier availability.
5. Reassess inventory eligibility if production dates or storage conditions change.

All recommendations require human approval.

---

### AI Governance and Human Oversight Disclaimer

This analysis uses only the supplied synthetic business data. It supports inventory management and production planning but does not independently certify food safety, approve ingredient suitability or authorise supplier orders.

All purchasing recommendations require inventory or procurement manager approval.

All supplied dates and quantities are synthetic and do not represent real food safety determinations.


#### Evaluation

The revised prompt correctly calculated all
ingredient replenishment and surplus quantities.

Established replenishment requirements totalled
27 kg, consisting of 15 kg of wheat flour and
12 kg of chicken.

No provisional replenishment was required.

The response correctly classified eligible
inventory, identified expiry attention requirements
and used First Expiry, First Out (FEFO) terminology.

Missing batch identifiers were recognised as a
traceability limitation.

The requested reporting structure and human
approval safeguards were maintained.

Evaluation score: 10/10 (100%).

Status: Passed.

### Test Case B

Testing date: 25 November 2026

AI tool and model: ChatGPT

#### Actual AI Output


# Flavors of Ceylon – Ingredient Inventory and Replenishment Report

## Report Overview

| Report Information | Details |
|---|---|
| Business | Flavors of Ceylon |
| Inventory Review Date | 1 December 2026 |
| Production Planning Period | 1–7 December 2026 |
| Scheduled Production Date | 5 December 2026 |
| Assessment Type | Ingredient Inventory and Replenishment Planning |
| Data Source | Supplied Synthetic Business Data |

---

## 1. Data Validation

The supplied inventory records and approved production requirements have been reviewed for ingredient names, batch identification, quantities, measurement units, usable-through dates and relevant storage and condition information.

| Validation Item | Finding | Status |
|---|---|---|
| Ingredient names | All five ingredients are consistently identified. | Valid |
| Batch identification | All 10 inventory records have unique batch identifiers. | Valid |
| Stock quantities | All recorded numerical quantities are positive. | Valid |
| Measurement conversion | Wheat flour F02: 8,000 g = 8 kg. | Valid |
| Measurement unit | Rice R02 has an unverified measurement unit. | Pending Verification |
| Usable-through dates | Chicken C03 has missing expiry information. | Pending Verification |
| Expired inventory | Chicken C02 expired on 30 November 2026. | Exclude |
| Planned usage eligibility | Grated coconut G01 expires before production. | Exclude |
| Storage and condition checks | Other batches have passed the relevant supplied internal checks. | Verified for this scenario |
| Production requirements | All five approved requirements have valid quantities and measurement units. | Valid |
| Planned usage date | All ingredients are required on 5 December 2026. | Valid |
| Purchasing constraints | No incoming orders, additional safety stock or minimum order quantities apply. | Confirmed |

### Data Validation Outcome

- Two batches require further verification.
- One batch has expired.
- One batch expires before the scheduled production date.
- All approved production requirements are valid.
- Compatible measurement units have been converted.

No missing measurement units, expiry dates or storage conditions have been assumed.

---

## 2. Inventory Eligibility Assessment

Each inventory batch is assessed against the inventory review date, scheduled production date and supplied internal storage and condition information.

| Ingredient | Batch | Stock Quantity | Usable-Through Date | Eligibility Classification | Confirmed Eligible Stock | Assessment Reason |
|---|---|---:|---|---|---:|---|
| Wheat flour | F01 | 12 kg | 31 Dec 2026 | Eligible | 12 kg | Covers planned usage date; condition checks passed. |
| Wheat flour | F02 | 8 kg | 31 Dec 2026 | Eligible | 8 kg | Converted from 8,000 g; condition checks passed. |
| Rice | R01 | 15 kg | 31 Dec 2026 | Eligible | 15 kg | Covers planned usage date; condition checks passed. |
| Rice | R02 | 10 (unit unknown) | 31 Dec 2026 | Pending Verification | Excluded | Measurement unit is unverified; relevant condition status must also be confirmed. |
| Chicken | C01 | 10 kg | 6 Dec 2026 | Eligible — Expiry Attention | 10 kg | Covers planned usage date but expires within the planning period; condition checks passed. |
| Chicken | C02 | 8 kg | 30 Nov 2026 | Expired | 0 kg | Expired before the inventory review date. |
| Chicken | C03 | 5 kg | Missing | Pending Verification | 0 kg | Missing expiry information; relevant condition status must also be confirmed. |
| Grated coconut | G01 | 6 kg | 2 Dec 2026 | Expires Before Planned Usage | 0 kg | Usable-through date precedes scheduled production. |
| Grated coconut | G02 | 4 kg | 6 Dec 2026 | Eligible — Expiry Attention | 4 kg | Covers planned usage date but expires within the planning period; condition checks passed. |
| Eggs | E01 | 60 units | 12 Dec 2026 | Eligible | 60 units | Covers planned usage date; condition checks passed. |

### Eligibility Assessment Summary

| Eligibility Classification | Number of Batches |
|---|---:|
| Eligible | 4 |
| Eligible — Expiry Attention | 2 |
| Expired | 1 |
| Expires Before Planned Usage | 1 |
| Pending Verification | 2 |
| **Total** | **10** |

Only the six eligible batches are included in confirmed usable stock calculations.

Eligibility is based on the supplied scenario information and does not constitute independent food safety certification.

---

## 3. Replenishment Calculations

### Calculation Methodology

The following formulas are applied because no incoming purchase orders, additional safety stock or minimum order quantity requirements are specified.

**Stock Balance**

    Stock Balance = Confirmed Eligible Stock - Approved Requirement

**Indicative Replenishment**

    Indicative Replenishment = Max(0, Approved Requirement - Confirmed Eligible Stock)

**Surplus Stock**

    Surplus Stock = Max(0, Confirmed Eligible Stock - Approved Requirement)

### Ingredient Replenishment Analysis

| Ingredient | Approved Requirement | Confirmed Eligible Stock | Stock Balance | Replenishment Calculation | Indicative Replenishment | Surplus Stock | Purchasing Classification |
|---|---:|---:|---:|---|---:|---:|---|
| Wheat flour | 25 kg | 20 kg | -5 kg | Max(0, 25 - 20) | 5 kg | 0 kg | Established Requirement |
| Rice | 20 kg | 15 kg | -5 kg | Max(0, 20 - 15) | 5 kg | 0 kg | Provisional Requirement |
| Chicken | 25 kg | 10 kg | -15 kg | Max(0, 25 - 10) | 15 kg | 0 kg | Provisional Requirement |
| Grated coconut | 10 kg | 4 kg | -6 kg | Max(0, 10 - 4) | 6 kg | 0 kg | Established Requirement |
| Eggs | 48 units | 60 units | +12 units | Max(0, 48 - 60) | 0 units | 12 units | No Replenishment Required |

### Purchasing Requirement Subtotals

| Purchasing Classification | Ingredients | Subtotal |
|---|---|---:|
| Established Requirement | Wheat flour (5 kg) + Grated coconut (6 kg) | **11 kg** |
| Provisional Requirement | Rice (5 kg) + Chicken (15 kg) | **20 kg** |
| No Replenishment Required | Eggs | **0 units** |
| Pending Calculation | None | Not applicable |

### Inventory Findings Summary

| Indicator | Result |
|---|---|
| Ingredients with shortages | 4 |
| Ingredients with surplus stock | 1 |
| Established replenishment requirement | 11 kg |
| Provisional replenishment requirement | 20 kg |
| Surplus stock | 12 egg units |
| Eligible stock requiring expiry attention | 14 kg |
| Batches requiring verification | 2 |

### Impact of Unresolved Inventory Verification

| Ingredient | Outstanding Issue | Potential Impact |
|---|---|---|
| Rice | Batch R02 has an unverified measurement unit. | The provisional shortage of 5 kg may change after the measurement unit and eligibility are verified. |
| Chicken | Batch C03 contains 5 kg with missing expiry information. | If the entire batch is subsequently verified and authorised as eligible, the provisional shortage could decrease from 15 kg to 10 kg. |

The provisional replenishment quantities are indicative only and must not be treated as final or approved purchasing quantities.

Kilograms and individual units have been reported separately and have not been combined into a single numerical total.

---

## 4. Stock Management Actions and Limitations

### Recommended Stock Management Actions

| Ingredient or Batch | Identified Issue | Recommended Action | Priority |
|---|---|---|---|
| Wheat flour F01 and F02 | Established shortage | Request procurement manager approval for replenishment. Apply FEFO; either batch may be used first because their usable-through dates are identical. | High |
| Rice R02 | Unverified measurement unit | Hold the batch and verify its measurement unit, quantity and relevant condition information before recalculating the shortage. | High |
| Chicken C01 | Approaching expiry | Prioritise allocation to production on 5 December using FEFO, subject to continued suitability and human authorisation. | High |
| Chicken C02 | Expired inventory | Segregate from usable inventory, prevent production allocation and refer disposal decisions to responsible personnel. | Critical |
| Chicken C03 | Missing expiry information | Hold the batch, verify expiry and relevant condition records, and obtain appropriate authorisation before use. | High |
| Grated coconut G01 | Expires before production | Exclude from scheduled production and refer alternative-use or disposal decisions to responsible personnel. | High |
| Grated coconut G02 | Approaching expiry | Prioritise allocation to scheduled production using FEFO, subject to continued suitability and human authorisation. | High |
| Grated coconut | Established shortage | Request procurement manager approval for replenishment. | High |
| Eggs E01 | Surplus inventory | Retain surplus stock under approved storage conditions and monitor its usable-through date for future production planning. | Medium |

### Expiry Attention

| Ingredient | Batch | Eligible Quantity | Usable-Through Date | Planned Usage Date |
|---|---|---:|---|---|
| Chicken | C01 | 10 kg | 6 Dec 2026 | 5 Dec 2026 |
| Grated coconut | G02 | 4 kg | 6 Dec 2026 | 5 Dec 2026 |
| **Total** | | **14 kg** | | |

First Expiry, First Out (FEFO) stock rotation should be applied to verified and eligible inventory.

### Missing Information Requiring Human Review

| Batch | Missing or Unverified Information | Required Action |
|---|---|---|
| R02 | Measurement unit and relevant condition verification | Confirm measurement unit and eligibility before including stock in calculations. |
| C03 | Usable-through date and relevant condition verification | Verify expiry information and obtain appropriate authorisation before use. |

### Limitations and Operational Safeguards

- Missing measurement units, expiry dates and relevant condition information must be verified by responsible personnel.
- An unexpired usable-through date alone does not establish food safety or ingredient suitability.
- Inventory eligibility must be reassessed if scheduled production dates change.
- Supplier prices, delivery dates and stock availability have not been provided and are not assumed.
- Expired and unverified inventory must not be allocated to production.
- Disposal and alternative-use decisions must follow approved food safety procedures.
- All purchasing recommendations require inventory or procurement manager approval.
- AI cannot independently certify food safety, approve ingredient suitability or authorise supplier orders.

---

## 5. Management Summary and Priority Actions

The inventory assessment identifies four ingredient shortages and an egg surplus of 12 units. Established replenishment requirements total 11 kg, while provisional requirements total 20 kg. Two batches require verification, and 14 kg of eligible stock requires expiry attention.

### Priority Actions

1. Request approval for established replenishment of 5 kg wheat flour and 6 kg grated coconut.
2. Verify rice R02 and chicken C03 before finalising provisional purchasing quantities.
3. Segregate expired chicken C02 and exclude grated coconut G01 from scheduled production.
4. Prioritise chicken C01 and grated coconut G02 using FEFO.
5. Monitor surplus eggs and obtain human approval before purchasing or releasing held inventory.

**Final Assessment:** Confirmed eligible inventory cannot fully satisfy scheduled production requirements. Replenishment and inventory verification are required before production on 5 December 2026.

---

*Disclaimer: This report uses synthetic business data for testing purposes. All recommendations are subject to human review, approved food safety procedures and management authorisation.*

#### Evaluation

The revised prompt correctly assessed all ten
inventory batches and calculated eligible stock.

All replenishment calculations were correct.

Established replenishment requirements:

- Wheat flour: 5 kg.
- Grated coconut: 6 kg.
- Subtotal: 11 kg.

Provisional replenishment requirements:

- Rice: 5 kg.
- Chicken: 15 kg.
- Subtotal: 20 kg.

Total indicative replenishment: 31 kg.

The response correctly identified 12 surplus eggs
and 14 kg of eligible stock requiring expiry
attention.

Expired and unverified inventory remained excluded
from eligible stock calculations.

The response introduced qualitative action
priorities without defined classification
thresholds. Some repeated information also remained.

Evaluation score: 9/10 (90%).

Status: Passed with minor reporting limitations.

---

## 7. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 8/10 | 17/20 (85%) |
| v1.1 | 10/10 | 9/10 | 19/20 (95%) |

### Final Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 1 |
| Business Relevance | 2 | 2 |
| Responsible AI | 2 | 2 |
| Total | 10/10 | 9/10 |

Absolute improvement: 10 percentage points.

Relative improvement in evaluation score: 11.76%.

### Final Observations

The revised prompt retained correct numerical
calculations while improving inventory eligibility
classification, purchasing transparency and
responsible inventory management.

Established and provisional replenishment
requirements were clearly separated.

Correct FEFO terminology and appropriate human
approval requirements were maintained.

Minor limitations remain in subjective action
priority classifications and repeated information.

Final selected version: v1.1.

No further refinement is required within the
current academic testing scope.

The results measure response quality against
selected synthetic scenarios, not actual
commercial inventory management performance.

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

- [P02 Iteration Log](../04-iteration-logs/P02-iteration-log.md)
- [P02 Final Evaluation](../05-evaluation/P02-final-evaluation.md)
