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

PRODUCTION PLANNING INFORMATION

Business: Flavors of Ceylon.
Planning date: 4 December 2026.
Planning period: 1–7 December 2026.
Available production dates: 5–7 December 2026.

Related assessments:
- P01 Test C: Demand and production planning.
- P02 Test A: Inventory and replenishment.
- P03 Test A: Supplier purchase order preparation.

APPROVED PRODUCTION TARGETS

Product | Forecast Demand | Approved Production Target
Fish roti | 160 | 120
Vegetable rolls | 80 | 0
Chicken kottu | 90 | 85
Rice and curry packs | 60 | 50
Pol sambol sachets | 80 | 70

All product quantities represent individual units.

The production targets already account for
finished-product inventory, safety stock and
previous production capacity assessment.

Use the approved production targets rather than
the full demand forecasts when allocating batches.

INGREDIENT CONSUMPTION REQUIREMENTS

The following quantities are required to produce
10 units of each product.

Product | Wheat Flour (kg) | Rice (kg) | Chicken (kg) | Grated Coconut (kg) | Fish (kg) | Vegetables (kg) | Eggs (units)
Fish roti | 1.2 | 0 | 0 | 0 | 0.8 | 0 | 0
Vegetable rolls | 1.2 | 0 | 0 | 0 | 0 | 1.0 | 0
Chicken kottu | 2.0 | 0 | 1.8 | 0 | 0 | 0 | 10
Rice and curry packs | 0 | 1.5 | 2.0 | 0.3 | 0 | 0 | 0
Pol sambol sachets | 0 | 0 | 0 | 0.5 | 0 | 0 | 0

Ingredient consumption scales proportionally
with the number of units produced.

All other necessary ingredients and packaging
materials are verified as sufficient for the
approved production targets.

AVAILABLE INGREDIENT INVENTORY

Ingredient | Confirmed Available Stock
Wheat flour | 45 kg
Rice | 40 kg
Chicken | 30 kg
Grated coconut | 12 kg
Fish | 12 kg
Vegetables | 10 kg
Eggs | 100 units

This is an updated inventory snapshot for
production planning.

All listed stock has passed the relevant
internal storage and condition checks and is
eligible for the available production dates
under this synthetic scenario.

The P03 Test A purchases of 15 kg wheat flour
and 12 kg chicken have subsequently been
approved, received and inspected.

These received quantities are already included
in the available stock figures above.

Do not count these received quantities twice.

Do not assume that earlier inventory records
or previously expiring batches remain available.

BATCH AND PRODUCTION CAPACITY

Product | Maximum Units per Batch | Fixed Minutes per Batch | Staff Required per Batch | Weekly Production Limit
Fish roti | 20 | 40 | 2 | 120
Vegetable rolls | 20 | 35 | 2 | 60
Chicken kottu | 20 | 45 | 2 | 100
Rice and curry packs | 25 | 50 | 2 | 60
Pol sambol sachets | 35 | 30 | 2 | 70

Partial batches are permitted in multiples
of 5 units.

Every batch, including a partial batch,
requires its full stated production duration.

STAFFING AND SHARED RESOURCE AVAILABILITY

Date | Available Staff | Available Production Minutes
5 December 2026 | 2 | 360
6 December 2026 | 2 | 360
7 December 2026 | 2 | 360

All products use one shared production station.

Only one batch may operate at a time.

Both required staff members must be available
for the entire duration of each batch.

The supplied production durations include
the required setup and cleaning allowances.

The available production minutes represent
net scheduling time after other approved
workplace allowances.

PRODUCTION PRIORITIES

Allocate production in the following priority order:

1. Fish roti.
2. Chicken kottu.
3. Rice and curry packs.
4. Pol sambol sachets.
5. Vegetable rolls.

Prioritise achieving higher-priority approved
targets before allocating remaining resources
to lower-priority products.

ADDITIONAL CONDITIONS

- Do not exceed approved production targets.
- Do not exceed product-specific weekly limits.
- Do not exceed available ingredient quantities.
- Do not assume additional staff or overtime.
- Do not overlap production batches.
- Do not assume ingredient substitutions.
- All proposed quantities and schedules require
  production manager approval.

All recipes, quantities, capacities, durations,
staffing records and dates are synthetic and
created solely for academic testing.

The scheduling exercise does not establish
actual food processing or food safety standards.

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

PRODUCTION PLANNING INFORMATION

Business: Flavors of Ceylon.
Planning date: 4 December 2026.
Planning period: 1–7 December 2026.
Available production dates: 5–7 December 2026.

Related assessments:
- P01 Test C: Demand and production planning.
- P02 Test B: Challenging inventory assessment.
- P03 Test B: Incomplete procurement information.

APPROVED PRODUCTION TARGETS

Product | Forecast Demand | Approved Production Target
Fish roti | 160 | 120
Vegetable rolls | 80 | 0
Chicken kottu | 90 | 85
Rice and curry packs | 60 | 50
Pol sambol sachets | 80 | 70

All product quantities represent individual units.

The production targets already account for
finished-product inventory, safety stock and
previous production capacity assessment.

Use these approved production targets rather than
the full demand forecasts when allocating batches.

INGREDIENT CONSUMPTION REQUIREMENTS

The following quantities are required to produce
10 units of each product.

Product | Wheat Flour (kg) | Rice (kg) | Chicken (kg) | Grated Coconut (kg) | Fish (kg) | Vegetables (kg) | Eggs (units)
Fish roti | 1.2 | 0 | 0 | 0 | 0.8 | 0 | 0
Vegetable rolls | 1.2 | 0 | 0 | 0 | 0 | 1.0 | 0
Chicken kottu | 2.0 | 0 | 1.8 | 0 | 0 | 0 | 10
Rice and curry packs | 0 | 1.5 | 2.0 | 0.3 | 0 | 0 | 0
Pol sambol sachets | 0 | 0 | 0 | 0.5 | 0 | 0 | 0

Ingredient consumption scales proportionally
with the number of units produced.

All other necessary ingredients and packaging
materials are verified as sufficient for the
approved production targets.

CONFIRMED AVAILABLE INGREDIENT INVENTORY

Ingredient | Confirmed Available Stock
Wheat flour | 20 kg
Rice | 15 kg
Chicken | 10 kg
Grated coconut | 4 kg
Fish | 8 kg
Vegetables | 10 kg
Eggs | 60 units

This is an updated verified inventory snapshot.

All listed stock has passed the relevant internal
storage and condition checks and is eligible for
production on 5 and 6 December 2026 under this
synthetic scenario.

Expired and unverified batches identified during
P02 have already been excluded.

Do not include previously excluded inventory.

PENDING SUPPLIER DELIVERIES

Ingredient | Quantity | Status
Wheat flour | 5 kg | Draft order only; delivery unconfirmed
Grated coconut | 6 kg | Draft order only; price and delivery unconfirmed

These ingredients are associated with P03 Test B.

Neither delivery has been confirmed or received.

Rice and chicken purchasing requirements from
P02 Test B remain provisional and unapproved.

Do not count pending supplier deliveries or
provisional purchases as available inventory.

BATCH AND PRODUCTION CAPACITY

Product | Maximum Units per Batch | Fixed Minutes per Batch | Staff Required per Batch | Weekly Production Limit
Fish roti | 20 | 40 | 2 | 120
Vegetable rolls | 20 | 35 | 2 | 60
Chicken kottu | 20 | 45 | 2 | 100
Rice and curry packs | 25 | 50 | 2 | 60
Pol sambol sachets | 35 | 30 | 2 | 70

Partial batches are permitted in multiples
of 5 units.

Every batch, including a partial batch,
requires its full stated production duration.

STAFFING AND SHARED RESOURCE AVAILABILITY

Date | Available Staff | Available Production Minutes
5 December 2026 | 2 | 375
6 December 2026 | 1 | 360
7 December 2026 | 0 | 0

Only one employee is available on 6 December
because of a staffing shortage.

All products use one shared production station.

Only one batch may operate at a time.

Both required staff members must be available
for the entire duration of each batch.

The supplied production durations include
the required setup and cleaning allowances.

The available production minutes represent
net scheduling time after other approved
workplace allowances.

PRODUCTION PRIORITIES

Allocate production in the following priority order:

1. Fish roti.
2. Chicken kottu.
3. Rice and curry packs.
4. Pol sambol sachets.
5. Vegetable rolls.

For each product, allocate the maximum feasible
quantity up to its approved production target
before allocating remaining ingredients and
production time to the next product.

Do not reduce higher-priority allocations solely
to increase lower-priority production.

ADDITIONAL CONDITIONS

- Do not exceed approved production targets.
- Do not exceed product-specific weekly limits.
- Do not exceed available ingredient quantities.
- Do not assume additional staff or overtime.
- Do not overlap production batches.
- Do not assume ingredient substitutions.
- Do not assume unconfirmed deliveries will arrive.
- Identify unmet production targets and their causes.
- All proposed quantities and schedules require
  production manager approval.

All recipes, quantities, capacities, durations,
staffing records and dates are synthetic and
created solely for academic testing.

The scheduling exercise does not establish
actual food processing or food safety standards.

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

Testing date: 26 November 2026

AI tool and model: ChatGPT

#### Actual AI Output

# Flavors of Ceylon – Proposed Weekly Production Schedule

## 1. Production Planning Overview

| Planning Information | Details |
|---|---|
| Business Name | Flavors of Ceylon |
| Planning Date | 4 December 2026 |
| Planning Period | 1–7 December 2026 |
| Available Production Dates | 5–7 December 2026 |
| Available Staff per Day | 2 |
| Available Production Time per Day | 360 minutes |
| Total Available Production Time | 1,080 minutes |
| Production Stations | 1 shared production station |
| Schedule Status | Draft – Pending Production Manager Approval |

### Related Assessments

- P01 Test C – Demand and production planning.
- P02 Test A – Inventory and replenishment.
- P03 Test A – Supplier purchase order preparation.

The proposed production schedule uses the approved production
targets rather than the full demand forecasts.

Production quantities are allocated according to the specified
product priorities, confirmed ingredient availability, staffing
requirements, batch sizes and production capacity.

The updated inventory figures already include the received
quantities of 15 kg of wheat flour and 12 kg of chicken.
These quantities have not been counted twice.

---

## 2. Approved Production Target Assessment

| Product | Forecast Demand (Units) | Approved Target (Units) | Weekly Limit (Units) | Proposed Production (Units) | Unfulfilled Target |
|---|---:|---:|---:|---:|---:|
| Fish roti | 160 | 120 | 120 | 120 | 0 |
| Vegetable rolls | 80 | 0 | 60 | 0 | 0 |
| Chicken kottu | 90 | 85 | 100 | 85 | 0 |
| Rice and curry packs | 60 | 50 | 60 | 50 | 0 |
| Pol sambol sachets | 80 | 70 | 70 | 70 | 0 |
| **Total** | **470** | **325** | **410** | **325** | **0** |

### Assessment

All approved production targets can be achieved using the
confirmed ingredients and available production resources.

Vegetable rolls are excluded from the production schedule
because the approved production target is zero, despite the
forecast demand of 80 units.

The difference between the total forecast demand and approved
production target does not represent an additional production
requirement because the approved targets already account for
finished-product inventory, safety stock and previous
production capacity assessments.

---

## 3. Ingredient Requirements and Availability Assessment

### 3.1 Ingredient Consumption Calculation

The required ingredient quantities are calculated using
the following formula:

**Required ingredient quantity = (Proposed production units / 10)
× Ingredient requirement per 10 units**

### 3.2 Ingredient Consumption by Product

| Product | Wheat Flour (kg) | Rice (kg) | Chicken (kg) | Grated Coconut (kg) | Fish (kg) | Vegetables (kg) | Eggs (Units) |
|---|---:|---:|---:|---:|---:|---:|---:|
| Fish roti | 14.4 | 0 | 0 | 0 | 9.6 | 0 | 0 |
| Vegetable rolls | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| Chicken kottu | 17.0 | 0 | 15.3 | 0 | 0 | 0 | 85 |
| Rice and curry packs | 0 | 7.5 | 10.0 | 1.5 | 0 | 0 | 0 |
| Pol sambol sachets | 0 | 0 | 0 | 3.5 | 0 | 0 | 0 |
| **Total Requirements** | **31.4** | **7.5** | **25.3** | **5.0** | **9.6** | **0** | **85** |

### 3.3 Inventory Sufficiency Assessment

| Ingredient | Available Stock | Required Quantity | Remaining Stock | Shortage | Status |
|---|---:|---:|---:|---:|---|
| Wheat flour | 45 kg | 31.4 kg | 13.6 kg | 0 kg | Sufficient |
| Rice | 40 kg | 7.5 kg | 32.5 kg | 0 kg | Sufficient |
| Chicken | 30 kg | 25.3 kg | 4.7 kg | 0 kg | Sufficient |
| Grated coconut | 12 kg | 5.0 kg | 7.0 kg | 0 kg | Sufficient |
| Fish | 12 kg | 9.6 kg | 2.4 kg | 0 kg | Sufficient |
| Vegetables | 10 kg | 0 kg | 10 kg | 0 kg | Not required |
| Eggs | 100 units | 85 units | 15 units | 0 units | Sufficient |

### 3.4 Ingredient Inventory Utilisation

**Inventory utilisation (%) =
(Required quantity / Available stock) × 100**

| Ingredient | Inventory Utilisation | Management Attention |
|---|---:|---|
| Wheat flour | 69.78% | Standard monitoring |
| Rice | 18.75% | Standard monitoring |
| Chicken | 84.33% | Increased monitoring |
| Grated coconut | 41.67% | Standard monitoring |
| Fish | 80.00% | Increased monitoring |
| Vegetables | 0.00% | Not required |
| Eggs | 85.00% | Increased monitoring |

An illustrative inventory utilisation threshold of 80%
is used to identify ingredients requiring increased
management attention. This is not an approved operational
or food safety threshold.

### Assessment

- No ingredient shortages have been identified.
- No additional ingredient purchases are required.
- Eggs, chicken and fish have relatively high inventory
  utilisation and require additional monitoring.
- All other ingredients and packaging materials are
  verified as sufficient under the supplied scenario.
- Received purchase quantities have not been double-counted.
- Earlier inventory records and previously expiring
  batches have not been assumed to remain available.

---

## 4. Production Batch Allocation

Production batches are allocated according to the specified
priority order.

Partial batches are permitted in multiples of five units
and require the full stated production duration.

| Priority | Product | Proposed Units | Full Batches | Partial Batches | Total Batches | Total Minutes |
|---:|---|---:|---|---|---:|---:|
| 1 | Fish roti | 120 | 6 × 20 | None | 6 | 240 |
| 2 | Chicken kottu | 85 | 4 × 20 | 1 × 5 | 5 | 225 |
| 3 | Rice and curry packs | 50 | 2 × 25 | None | 2 | 100 |
| 4 | Pol sambol sachets | 70 | 2 × 35 | None | 2 | 60 |
| 5 | Vegetable rolls | 0 | None | None | 0 | 0 |
| **Total** | | **325** | **14** | **1** | **15** | **625** |

### Production Time Calculations

| Product | Calculation | Required Time |
|---|---|---:|
| Fish roti | 6 × 40 minutes | 240 minutes |
| Chicken kottu | 5 × 45 minutes | 225 minutes |
| Rice and curry packs | 2 × 50 minutes | 100 minutes |
| Pol sambol sachets | 2 × 30 minutes | 60 minutes |
| Vegetable rolls | 0 × 35 minutes | 0 minutes |
| **Total** | | **625 minutes** |

The five-unit chicken kottu partial batch is allocated
the full 45-minute production duration.

No batch exceeds its product-specific maximum batch size.

---

## 5. Proposed Weekly Production Schedule

The proposed schedule uses elapsed production minutes
rather than specific clock times because daily shift
starting times have not been supplied.

All batches operate sequentially using one shared
production station and two staff members.

### 5.1 Saturday, 5 December 2026

| Batch ID | Product | Quantity (Units) | Start Minute | End Minute | Duration | Staff |
|---|---|---:|---:|---:|---:|---:|
| FR-01 | Fish roti | 20 | 0 | 40 | 40 min | 2 |
| FR-02 | Fish roti | 20 | 40 | 80 | 40 min | 2 |
| FR-03 | Fish roti | 20 | 80 | 120 | 40 min | 2 |
| FR-04 | Fish roti | 20 | 120 | 160 | 40 min | 2 |
| FR-05 | Fish roti | 20 | 160 | 200 | 40 min | 2 |
| FR-06 | Fish roti | 20 | 200 | 240 | 40 min | 2 |
| CK-01 | Chicken kottu | 20 | 240 | 285 | 45 min | 2 |
| CK-02 | Chicken kottu | 20 | 285 | 330 | 45 min | 2 |
| **Daily Total** | | **160** | | | **330 min** | |

#### Daily Capacity Summary

- Available production time: 360 minutes.
- Scheduled production time: 330 minutes.
- Remaining production time: 30 minutes.
- Total production batches: 8.
- Total proposed production: 160 units.
- Required concurrent staff: 2.
- Capacity utilisation: 91.67%.

#### Scheduling Explanation

Fish roti production is completed first because it has
the highest production priority.

Two chicken kottu batches are then scheduled within
the remaining available production time.

The remaining 30 minutes are insufficient to accommodate
another chicken kottu batch requiring 45 minutes.

This time is left unallocated to maintain the selected
strict priority-based scheduling approach.

---

### 5.2 Sunday, 6 December 2026

| Batch ID | Product | Quantity (Units) | Start Minute | End Minute | Duration | Staff |
|---|---|---:|---:|---:|---:|---:|
| CK-03 | Chicken kottu | 20 | 0 | 45 | 45 min | 2 |
| CK-04 | Chicken kottu | 20 | 45 | 90 | 45 min | 2 |
| CK-05 | Chicken kottu – Partial batch | 5 | 90 | 135 | 45 min | 2 |
| RC-01 | Rice and curry packs | 25 | 135 | 185 | 50 min | 2 |
| RC-02 | Rice and curry packs | 25 | 185 | 235 | 50 min | 2 |
| PS-01 | Pol sambol sachets | 35 | 235 | 265 | 30 min | 2 |
| PS-02 | Pol sambol sachets | 35 | 265 | 295 | 30 min | 2 |
| **Daily Total** | | **165** | | | **295 min** | |

#### Daily Capacity Summary

- Available production time: 360 minutes.
- Scheduled production time: 295 minutes.
- Remaining production time: 65 minutes.
- Total production batches: 7.
- Total proposed production: 165 units.
- Required concurrent staff: 2.
- Capacity utilisation: 81.94%.

#### Scheduling Explanation

The remaining chicken kottu batches are completed first,
including the five-unit partial batch.

Rice and curry packs and pol sambol sachets are then
produced according to their respective production priorities.

All approved production targets are scheduled for
completion by the end of the second production day.

---

### 5.3 Monday, 7 December 2026

| Activity | Proposed Quantity | Allocated Production Time | Status |
|---|---:|---:|---|
| Additional production | 0 units | 0 minutes | Not required |
| Contingency capacity | Not applicable | 360 minutes available | Unallocated reserve |

#### Daily Capacity Summary

- Available production time: 360 minutes.
- Scheduled production time: 0 minutes.
- Remaining production time: 360 minutes.
- Total production batches: 0.
- Total proposed production: 0 units.
- Capacity utilisation: 0.00%.

#### Scheduling Explanation

The third production day remains available for approved
contingency scheduling if unexpected disruptions occur.

Any rescheduling must remain within the approved production
targets, ingredient availability, staffing requirements
and product-specific production limits.

Remaining capacity does not authorise additional production.

---

## 6. Weekly Production Summary

| Product | 5 December | 6 December | 7 December | Total Production | Approved Target |
|---|---:|---:|---:|---:|---:|
| Fish roti | 120 | 0 | 0 | 120 | 120 |
| Vegetable rolls | 0 | 0 | 0 | 0 | 0 |
| Chicken kottu | 40 | 45 | 0 | 85 | 85 |
| Rice and curry packs | 0 | 50 | 0 | 50 | 50 |
| Pol sambol sachets | 0 | 70 | 0 | 70 | 70 |
| **Total** | **160** | **165** | **0** | **325** | **325** |

### Production Target Achievement

**Target achievement (%) =
(Proposed production / Approved production target) × 100**

| Product | Target Achievement |
|---|---:|
| Fish roti | 100% |
| Vegetable rolls | Not applicable – Zero approved target |
| Chicken kottu | 100% |
| Rice and curry packs | 100% |
| Pol sambol sachets | 100% |
| **Overall Achievement** | **100%** |

---

## 7. Production Capacity and Staffing Assessment

### 7.1 Production Capacity Utilisation

**Capacity utilisation (%) =
(Scheduled production minutes / Available production minutes)
× 100**

| Production Date | Available Minutes | Scheduled Minutes | Remaining Minutes | Utilisation |
|---|---:|---:|---:|---:|
| 5 December 2026 | 360 | 330 | 30 | 91.67% |
| 6 December 2026 | 360 | 295 | 65 | 81.94% |
| 7 December 2026 | 360 | 0 | 360 | 0.00% |
| **Total** | **1,080** | **625** | **455** | **57.87%** |

### 7.2 Weekly Capacity Summary

| Performance Indicator | Result |
|---|---|
| Total Approved Production Target | 325 units |
| Total Proposed Production | 325 units |
| Production Target Achievement | 100% |
| Total Production Batches | 15 |
| Full Batches | 14 |
| Partial Batches | 1 |
| Available Production Time | 1,080 minutes |
| Required Production Time | 625 minutes |
| Remaining Production Time | 455 minutes |
| Weekly Capacity Utilisation | 57.87% |
| Unallocated Capacity | 42.13% |
| Additional Staff Required | None |
| Overtime Required | None |
| Ingredient Shortages | None identified |

The proposed production requires 10 hours and 25 minutes
of shared production station time.

The remaining weekly production capacity is 7 hours
and 35 minutes.

### 7.3 Staffing Requirements

| Date | Available Staff | Required Concurrent Staff | Available Staff-Minutes | Required Staff-Minutes |
|---|---:|---:|---:|---:|
| 5 December 2026 | 2 | 2 | 720 | 660 |
| 6 December 2026 | 2 | 2 | 720 | 590 |
| 7 December 2026 | 2 | 0 | 720 | 0 |
| **Total** | | | **2,160** | **1,250** |

**Required staff-minutes =
Scheduled production minutes × Required staff members**

**Remaining staff-minutes = 2,160 - 1,250 = 910 minutes**

Staffing is sufficient to complete the proposed production
schedule. No additional staffing or overtime is required
under the supplied conditions.

However, both staff members are required throughout every
scheduled batch. Staff absence could therefore prevent
production from proceeding as planned.

---

## 8. Production Bottlenecks and Resource Limitations

| Identified Issue | Risk Level | Potential Impact | Recommended Management Action |
|---|---|---|---|
| Single shared production station | Medium | Equipment failure could interrupt the entire production schedule. | Confirm equipment readiness and retain contingency capacity. |
| Dependence on two staff members | Medium | Absence of either staff member could prevent batch completion. | Confirm staff availability before commencing production. |
| High egg utilisation | Medium | Only 15 eggs remain after planned production. | Monitor consumption and prevent unapproved stock allocation. |
| High chicken utilisation | Medium | Only 4.7 kg remains after planned production. | Monitor ingredient usage against approved recipes. |
| High fish utilisation | Medium | Only 2.4 kg remains after planned production. | Confirm stock availability before production. |
| Fish roti weekly production limit | Medium | Production reaches the weekly maximum of 120 units. | Do not allocate additional production without authorised reassessment. |
| Pol sambol weekly production limit | Medium | Production reaches the weekly maximum of 70 units. | Maintain the approved production limit. |
| Partial chicken kottu batch | Low | Five units require the full 45-minute batch duration. | Retain the partial batch to achieve the approved target. |
| Vegetable rolls excluded | Low | No new production despite forecast demand. | Maintain the approved zero-production target unless formally revised. |
| Ingredient shortages | None identified | All approved production requirements are covered. | Continue monitoring stock availability. |

The risk levels are illustrative qualitative management
assessments for this synthetic scenario.

They do not represent formally approved operational
or food safety risk classifications.

### Bottleneck Assessment

No binding resource shortage prevents the achievement
of the approved weekly production targets.

However, the single shared production station and
dependence on two staff members represent potential
operational bottlenecks.

The remaining capacity provides flexibility to manage
unexpected production disruptions, subject to continued
resource availability and management approval.

---

## 9. Missing Information and Verification Requirements

| Information Requiring Confirmation | Status | Required Action |
|---|---|---|
| Exact daily shift starting and finishing times | Not supplied | Confirm clock-based production schedule. |
| Individual staff assignments | Not supplied | Confirm staff roster and responsibilities. |
| Equipment operational readiness | Pending verification | Complete approved pre-production checks. |
| Product-specific food safety procedures | Not supplied | Follow existing approved food safety procedures. |
| Finished-product storage capacity | Not supplied | Confirm sufficient storage before production. |
| Product shelf-life and dispatch arrangements | Not supplied | Confirm approved storage and distribution arrangements. |
| Production manager authorisation | Pending approval | Obtain formal approval before implementation. |

No missing ingredient quantities, recipe consumption rates,
batch capacities or production durations prevent the
preparation of this draft schedule.

However, operational verification and management approval
remain necessary before actual implementation.

---

## 10. Production Scheduling Compliance Assessment

### Production Target Compliance

- [x] Uses approved production targets instead of full
  demand forecasts.
- [x] Achieves all approved production targets.
- [x] Follows the specified production priority order.
- [x] Does not exceed product-specific weekly limits.
- [x] Excludes vegetable rolls because the approved
  production target is zero.

### Ingredient Availability Compliance

- [x] Does not exceed confirmed ingredient availability.
- [x] Does not double-count received purchase quantities.
- [x] Does not assume earlier inventory records remain
  available.
- [x] Does not assume ingredient substitutions.
- [x] Identifies remaining ingredient quantities.
- [x] Identifies potential ingredient-related limitations.

### Batch and Capacity Compliance

- [x] Respects maximum batch sizes.
- [x] Uses permitted five-unit partial batch increments.
- [x] Allocates the full production duration to every batch.
- [x] Does not exceed daily production capacity.
- [x] Does not overlap production batches.
- [x] Uses only one shared production station.
- [x] Includes the supplied setup and cleaning allowances
  within stated production durations.

### Staffing Compliance

- [x] Maintains two staff members per scheduled batch.
- [x] Does not assume additional staffing.
- [x] Does not assume overtime.
- [x] Remains within available staff-minutes.

### Approval and Operational Requirements

- [x] Identifies missing operational information.
- [x] Identifies potential production bottlenecks.
- [x] Does not override approved food safety procedures.
- [ ] Production manager approval obtained.
- [ ] Equipment readiness confirmed.
- [ ] Individual staff assignments confirmed.
- [ ] Operational and food safety requirements verified.

**Overall Status: Planning requirements satisfied –
Operational verification and production manager approval pending.**

---

## 11. Management Recommendations

1. Approve the proposed production quantity of 325 units
   across the four products with positive approved
   production targets.

2. Prioritise fish roti and chicken kottu before commencing
   lower-priority products.

3. Complete the planned production activities on
   5 and 6 December 2026.

4. Retain 7 December 2026 as a contingency production day.

5. Closely monitor eggs, chicken and fish consumption
   during production.

6. Confirm staffing availability and equipment readiness
   before commencing production.

7. Confirm sufficient finished-product storage capacity
   and approved dispatch arrangements.

8. Do not use remaining production capacity to manufacture
   additional unapproved quantities.

9. Maintain the approved zero-production target for
   vegetable rolls unless formally revised.

10. Follow all existing approved food safety, hygiene,
    cleaning, storage and quality control procedures.

11. Obtain production manager approval before implementing
    the proposed production schedule.

---

## 12. Conclusion

The proposed weekly production schedule for Flavors of Ceylon
is feasible under the supplied synthetic planning conditions.

A total of 325 product units can be manufactured through
15 production batches using 625 minutes of the available
1,080 production minutes.

This represents a weekly production capacity utilisation
rate of 57.87%, leaving 455 minutes of unallocated capacity.

All approved production targets can be achieved without
ingredient shortages, additional staff, overtime,
ingredient substitutions or overlapping production
activities.

The proposed schedule supports efficient resource allocation
while maintaining the specified production priorities and
operational limitations.

All approved production targets are scheduled for completion
by 6 December 2026, with 7 December 2026 retained as a
contingency production day.

The schedule remains a draft and must not be implemented
without operational verification and production manager
approval.

---

## 13. Production Approval

| Approval Information | Details |
|---|---|
| Prepared By | AI Production Planning Assistant |
| Prepared For | Flavors of Ceylon |
| Planning Date | 4 December 2026 |
| Planning Period | 1–7 December 2026 |
| Proposed Production Quantity | 325 units |
| Proposed Production Batches | 15 |
| Proposed Production Duration | 625 minutes |
| Production Manager | Pending confirmation |
| Approval Date | Pending |
| Final Status | Draft – Pending Production Manager Approval |

---

## Disclaimer

> All recipes, quantities, capacities, durations, staffing
> records and dates are synthetic and provided solely for
> academic testing.
>
> This production schedule does not establish actual food
> processing or food safety standards, override approved
> procedures or authorise production.
>
> All proposed production quantities, batch allocations
> and schedules require human verification and production
> manager approval.

#### Evaluation

The response correctly achieved all approved
production targets of 325 units using 15 batches
and 625 production minutes.

All ingredient consumption, remaining inventory,
batch allocation and staffing calculations matched
the independently established benchmarks.

The response correctly avoided double-counting
received ingredients and respected all production
limits.

However, the 13-section report contained repeated
calculations, summaries and compliance checks.

An illustrative inventory utilisation threshold
and qualitative risk classifications were also
introduced without approved business thresholds.

Evaluation score: 9/10 (90%).

### Test Case B

Testing date: 26 November 2026

AI tool and model: ChatGPT

#### Actual AI Output

# Flavors of Ceylon – Weekly Production Planning and Scheduling Report

## P04 v1.0 – Test B

| Document Information | Details |
|---|---|
| Business | Flavors of Ceylon |
| Prompt Reference | P04 v1.0 |
| Test Reference | Test B |
| Planning Date | 4 December 2026 |
| Planning Period | 1–7 December 2026 |
| Available Production Dates | 5–7 December 2026 |
| Prepared By | AI Production Planning Assistant |
| Approval Status | Draft – Pending Production Manager Approval |
| Intended Use | Academic Testing |

### Related Assessments

- P01 Test C: Demand and production planning.
- P02 Test B: Challenging inventory assessment.
- P03 Test B: Incomplete procurement information.

---

## 1. Executive Summary

The proposed weekly production schedule has been developed using approved production targets, confirmed ingredient inventory, batch capacities, staffing availability, shared production resources and established production priorities.

The assessment identifies significant ingredient shortages and staffing limitations that prevent the business from achieving its approved weekly production targets.

Although production time is available on 6 December 2026, only one employee is available. All production batches require two employees. Therefore, production can only be scheduled on 5 December 2026.

### Key Production Indicators

| Performance Indicator | Result |
|---|---:|
| Total Forecast Demand | 470 units |
| Approved Production Target | 325 units |
| Proposed Production | 185 units |
| Production Shortfall | 140 units |
| Target Achievement | 56.92% |
| Feasible Production Time | 375 minutes |
| Scheduled Production Time | 370 minutes |
| Production Time Utilisation | 98.67% |
| Total Production Batches | 9 |

No unconfirmed supplier deliveries, provisional purchases, additional staffing or overtime have been included in the proposed schedule.

> **Approval Notice:** This production schedule is a draft and must not be implemented without production manager approval.

---

## 2. Production Data Validation

| Validation Area | Assessment |
|---|---|
| Approved production targets | Supplied and used |
| Demand forecasts | Supplied for reference |
| Ingredient consumption requirements | Supplied |
| Confirmed ingredient inventory | Available and verified |
| Pending supplier deliveries | Excluded |
| Provisional purchasing requirements | Excluded |
| Previously expired or unverified inventory | Excluded |
| Batch capacity and duration | Supplied |
| Partial batch requirements | Multiples of 5 units |
| Staffing availability | Insufficient on 6 and 7 December |
| Shared production station | One batch at a time |
| Production priorities | Supplied and followed |
| Production manager approval | Pending |

The approved production targets already account for finished-product inventory, safety stock and previous production capacity assessments.

Therefore, no additional adjustments have been applied.

---

## 3. Ingredient Requirements for Approved Production Targets

The following table identifies the total ingredients required to achieve all approved production targets before applying scheduling constraints.

| Ingredient | Required Quantity | Confirmed Stock | Shortage | Surplus |
|---|---:|---:|---:|---:|
| Wheat flour (kg) | 31.40 | 20.00 | 11.40 | 0.00 |
| Rice (kg) | 7.50 | 15.00 | 0.00 | 7.50 |
| Chicken (kg) | 25.30 | 10.00 | 15.30 | 0.00 |
| Grated coconut (kg) | 5.00 | 4.00 | 1.00 | 0.00 |
| Fish (kg) | 9.60 | 8.00 | 1.60 | 0.00 |
| Vegetables (kg) | 0.00 | 10.00 | 0.00 | 10.00 |
| Eggs (units) | 85 | 60 | 25 | 0 |

### Identified Ingredient Shortages

- Wheat flour: 11.40 kg.
- Chicken: 15.30 kg.
- Grated coconut: 1.00 kg.
- Fish: 1.60 kg.
- Eggs: 25 units.

These shortages relate to the full approved production targets, not solely to the proposed reduced production schedule.

---

## 4. Staffing and Production Capacity Assessment

| Date | Available Staff | Available Station Minutes | Feasible Production Minutes | Status |
|---|---:|---:|---:|---|
| 5 December 2026 | 2 | 375 | 375 | Production permitted |
| 6 December 2026 | 1 | 360 | 0 | Insufficient staff |
| 7 December 2026 | 0 | 0 | 0 | No production |
| **Total** | — | **735** | **375** | **Limited capacity** |

All products require two employees throughout each production batch.

Consequently, the 360 minutes available on 6 December cannot be used for production under the supplied staffing requirements.

The production schedule must therefore be restricted to 5 December 2026.

No additional staffing or overtime has been assumed.

---

## 5. Production Priority and Quantity Allocation

Production quantities have been allocated in the specified priority order.

Higher-priority production quantities have not been reduced solely to increase lower-priority production.

### 5.1 Priority 1 – Fish Roti

- Forecast demand: 160 units.
- Approved production target: 120 units.
- Weekly production limit: 120 units.
- Available fish: 8 kg.
- Fish requirement per unit: 0.08 kg.
- Wheat flour requirement per unit: 0.12 kg.

#### Maximum Feasible Quantity

Fish-supported production:

`8 / 0.08 = 100 units`

Wheat flour-supported production before batch rounding:

`20 / 0.12 = 166.67 units`

Fish inventory is the primary limiting factor.

| Allocation Indicator | Result |
|---|---:|
| Proposed Production | 100 units |
| Batch Allocation | 5 × 20 units |
| Required Production Time | 200 minutes |
| Wheat Flour Consumption | 12.00 kg |
| Fish Consumption | 8.00 kg |
| Unmet Production Target | 20 units |
| Remaining Production Time | 175 minutes |

**Decision:** Allocate 100 fish roti units across five full batches.

---

### 5.2 Priority 2 – Chicken Kottu

Following fish roti production, 8 kg of wheat flour remains available.

- Forecast demand: 90 units.
- Approved production target: 85 units.
- Weekly production limit: 100 units.
- Remaining wheat flour: 8 kg.
- Available chicken: 10 kg.
- Available eggs: 60 units.
- Wheat flour requirement per unit: 0.20 kg.
- Chicken requirement per unit: 0.18 kg.
- Egg requirement per unit: 1 unit.

#### Maximum Feasible Quantity

Wheat flour-supported production:

`8 / 0.20 = 40 units`

Chicken-supported production before batch rounding:

`10 / 0.18 = 55.56 units`

Egg-supported production:

`60 / 1 = 60 units`

The remaining wheat flour inventory is the primary limiting factor.

| Allocation Indicator | Result |
|---|---:|
| Proposed Production | 40 units |
| Batch Allocation | 2 × 20 units |
| Required Production Time | 90 minutes |
| Wheat Flour Consumption | 8.00 kg |
| Chicken Consumption | 7.20 kg |
| Egg Consumption | 40 units |
| Unmet Production Target | 45 units |
| Remaining Production Time | 85 minutes |

**Decision:** Allocate 40 chicken kottu units across two full batches.

---

### 5.3 Priority 3 – Rice and Curry Packs

Following chicken kottu production, 2.80 kg of chicken remains available.

- Forecast demand: 60 units.
- Approved production target: 50 units.
- Weekly production limit: 60 units.
- Remaining chicken: 2.80 kg.
- Available rice: 15 kg.
- Available grated coconut: 4 kg.
- Chicken requirement per unit: 0.20 kg.
- Rice requirement per unit: 0.15 kg.
- Grated coconut requirement per unit: 0.03 kg.

#### Maximum Feasible Quantity

Chicken-supported production:

`2.80 / 0.20 = 14 units`

Partial batches must be produced in multiples of five units.

Therefore, the maximum permitted production quantity is 10 units.

| Allocation Indicator | Result |
|---|---:|
| Proposed Production | 10 units |
| Batch Allocation | 1 × 10 units |
| Batch Type | Partial batch |
| Required Production Time | 50 minutes |
| Rice Consumption | 1.50 kg |
| Chicken Consumption | 2.00 kg |
| Grated Coconut Consumption | 0.30 kg |
| Unmet Production Target | 40 units |
| Remaining Production Time | 35 minutes |

**Decision:** Allocate 10 rice and curry packs in one partial batch.

The partial batch requires its full stated production duration of 50 minutes.

---

### 5.4 Priority 4 – Pol Sambol Sachets

Following rice and curry pack production, 35 production minutes and 3.70 kg of grated coconut remain available.

- Forecast demand: 80 units.
- Approved production target: 70 units.
- Weekly production limit: 70 units.
- Remaining grated coconut: 3.70 kg.
- Grated coconut requirement per unit: 0.05 kg.
- Maximum units per batch: 35 units.
- Required production duration per batch: 30 minutes.

#### Maximum Feasible Quantity

Coconut-supported production:

`3.70 / 0.05 = 74 units`

Maximum feasible batches within remaining production time:

`35 / 30 = 1 complete batch`

Available production time is the primary limiting factor.

| Allocation Indicator | Result |
|---|---:|
| Proposed Production | 35 units |
| Batch Allocation | 1 × 35 units |
| Required Production Time | 30 minutes |
| Grated Coconut Consumption | 1.75 kg |
| Unmet Production Target | 35 units |
| Remaining Production Time | 5 minutes |

**Decision:** Allocate 35 pol sambol sachets in one full batch.

---

### 5.5 Priority 5 – Vegetable Rolls

- Forecast demand: 80 units.
- Approved production target: 0 units.
- Weekly production limit: 60 units.
- Available vegetables: 10 kg.

Although vegetable inventory is available, production must not exceed the approved production target.

| Allocation Indicator | Result |
|---|---:|
| Proposed Production | 0 units |
| Batch Allocation | 0 batches |
| Required Production Time | 0 minutes |
| Ingredient Consumption | 0 |
| Unmet Production Target | 0 units |

**Decision:** Do not schedule vegetable roll production.

---

## 6. Proposed Weekly Production Allocation

| Priority | Product | Forecast Demand | Approved Target | Proposed Quantity | Batches | Shortfall |
|---:|---|---:|---:|---:|---:|---:|
| 1 | Fish roti | 160 | 120 | 100 | 5 | 20 |
| 2 | Chicken kottu | 90 | 85 | 40 | 2 | 45 |
| 3 | Rice and curry packs | 60 | 50 | 10 | 1 | 40 |
| 4 | Pol sambol sachets | 80 | 70 | 35 | 1 | 35 |
| 5 | Vegetable rolls | 80 | 0 | 0 | 0 | 0 |
| **Total** | | **470** | **325** | **185** | **9** | **140** |

### Production Target Achievement by Product

| Product | Approved Target | Proposed Production | Achievement |
|---|---:|---:|---:|
| Fish roti | 120 | 100 | 83.33% |
| Chicken kottu | 85 | 40 | 47.06% |
| Rice and curry packs | 50 | 10 | 20.00% |
| Pol sambol sachets | 70 | 35 | 50.00% |
| Vegetable rolls | 0 | 0 | Not applicable |
| **Total** | **325** | **185** | **56.92%** |

### Production Achievement Visualisation

```text
Fish roti          [█████████████████░░░] 83.33%
Chicken kottu      [█████████░░░░░░░░░░░] 47.06%
Rice & curry packs [████░░░░░░░░░░░░░░░░] 20.00%
Pol sambol sachets [██████████░░░░░░░░░░] 50.00%
Vegetable rolls    No approved production target

Overall            [███████████░░░░░░░░░] 56.92%
```

Legend:

- Filled blocks represent achieved production.
- Empty blocks represent unmet approved production.
- Bars are approximate visual representations of the stated percentages.

---

## 7. Detailed Proposed Production Schedule

### 7.1 Saturday, 5 December 2026

Actual shift commencement times have not been supplied.

Therefore, the schedule uses elapsed production minutes rather than assumed clock times.

| Batch Reference | Product | Units | Start Minute | End Minute | Duration | Staff |
|---|---|---:|---:|---:|---:|---:|
| FR-01 | Fish roti | 20 | 0 | 40 | 40 min | 2 |
| FR-02 | Fish roti | 20 | 40 | 80 | 40 min | 2 |
| FR-03 | Fish roti | 20 | 80 | 120 | 40 min | 2 |
| FR-04 | Fish roti | 20 | 120 | 160 | 40 min | 2 |
| FR-05 | Fish roti | 20 | 160 | 200 | 40 min | 2 |
| CK-01 | Chicken kottu | 20 | 200 | 245 | 45 min | 2 |
| CK-02 | Chicken kottu | 20 | 245 | 290 | 45 min | 2 |
| RC-01 | Rice and curry packs | 10 | 290 | 340 | 50 min | 2 |
| PS-01 | Pol sambol sachets | 35 | 340 | 370 | 30 min | 2 |
| — | Unallocated capacity | 0 | 370 | 375 | 5 min | — |

### Daily Production Summary

| Indicator | Result |
|---|---:|
| Total Proposed Production | 185 units |
| Total Scheduled Batches | 9 |
| Full Batches | 8 |
| Partial Batches | 1 |
| Available Production Time | 375 minutes |
| Scheduled Production Time | 370 minutes |
| Remaining Production Time | 5 minutes |
| Required Staff | 2 |
| Scheduled Labour Consumption | 740 staff-minutes |

### Production Timeline

```text
5 December 2026 – Shared Production Station

Minute 0
    |
    | Fish roti – Batch FR-01
    | 20 units / 40 minutes
    |
Minute 40
    |
    | Fish roti – Batch FR-02
    | 20 units / 40 minutes
    |
Minute 80
    |
    | Fish roti – Batch FR-03
    | 20 units / 40 minutes
    |
Minute 120
    |
    | Fish roti – Batch FR-04
    | 20 units / 40 minutes
    |
Minute 160
    |
    | Fish roti – Batch FR-05
    | 20 units / 40 minutes
    |
Minute 200
    |
    | Chicken kottu – Batch CK-01
    | 20 units / 45 minutes
    |
Minute 245
    |
    | Chicken kottu – Batch CK-02
    | 20 units / 45 minutes
    |
Minute 290
    |
    | Rice and curry packs – Batch RC-01
    | 10 units / 50 minutes
    |
Minute 340
    |
    | Pol sambol sachets – Batch PS-01
    | 35 units / 30 minutes
    |
Minute 370
    |
    | Unallocated capacity – 5 minutes
    |
Minute 375 – End of available production time
```

### Production Time Utilisation

```text
Fish roti          200 minutes
Chicken kottu       90 minutes
Rice & curry packs  50 minutes
Pol sambol sachets  30 minutes
Unallocated time     5 minutes
--------------------------------
Total              375 minutes
```

Production time utilisation:

`(370 / 375) × 100 = 98.67%`

All batches are scheduled sequentially without overlapping.

### 7.2 Sunday, 6 December 2026

| Indicator | Result |
|---|---|
| Available Staff | 1 |
| Available Station Time | 360 minutes |
| Feasible Production Time | 0 minutes |
| Proposed Production | 0 units |
| Reason | Insufficient staffing |

No production is scheduled because every batch requires two employees.

### 7.3 Monday, 7 December 2026

| Indicator | Result |
|---|---|
| Available Staff | 0 |
| Available Production Time | 0 minutes |
| Proposed Production | 0 units |
| Reason | No staffing or production capacity |

### Weekly Production Schedule Summary

| Production Date | Fish Roti | Chicken Kottu | Rice and Curry Packs | Pol Sambol Sachets | Vegetable Rolls | Total Units |
|---|---:|---:|---:|---:|---:|---:|
| 5 December 2026 | 100 | 40 | 10 | 35 | 0 | 185 |
| 6 December 2026 | 0 | 0 | 0 | 0 | 0 | 0 |
| 7 December 2026 | 0 | 0 | 0 | 0 | 0 | 0 |
| **Total** | **100** | **40** | **10** | **35** | **0** | **185** |

---

## 8. Ingredient Consumption by Product

| Product | Flour (kg) | Rice (kg) | Chicken (kg) | Coconut (kg) | Fish (kg) | Vegetables (kg) | Eggs (units) |
|---|---:|---:|---:|---:|---:|---:|---:|
| Fish roti | 12.00 | 0.00 | 0.00 | 0.00 | 8.00 | 0.00 | 0 |
| Chicken kottu | 8.00 | 0.00 | 7.20 | 0.00 | 0.00 | 0.00 | 40 |
| Rice and curry packs | 0.00 | 1.50 | 2.00 | 0.30 | 0.00 | 0.00 | 0 |
| Pol sambol sachets | 0.00 | 0.00 | 0.00 | 1.75 | 0.00 | 0.00 | 0 |
| Vegetable rolls | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0 |
| **Total** | **20.00** | **1.50** | **9.20** | **2.05** | **8.00** | **0.00** | **40** |

Ingredient consumption has been calculated proportionally using the supplied ingredient requirements per 10 product units.

All other necessary ingredients and packaging materials are verified as sufficient under the supplied synthetic scenario.

---

## 9. Projected Remaining Ingredient Inventory

| Ingredient | Confirmed Stock | Proposed Consumption | Remaining Stock | Status |
|---|---:|---:|---:|---|
| Wheat flour (kg) | 20.00 | 20.00 | 0.00 | Fully allocated |
| Rice (kg) | 15.00 | 1.50 | 13.50 | Remaining stock |
| Chicken (kg) | 10.00 | 9.20 | 0.80 | Limited stock |
| Grated coconut (kg) | 4.00 | 2.05 | 1.95 | Remaining stock |
| Fish (kg) | 8.00 | 8.00 | 0.00 | Fully allocated |
| Vegetables (kg) | 10.00 | 0.00 | 10.00 | Unused |
| Eggs (units) | 60 | 40 | 20 | Remaining stock |

### Inventory Calculation

`Remaining Stock = Confirmed Available Stock - Proposed Consumption`

All proposed ingredient consumption quantities remain within confirmed available inventory.

Wheat flour and fish inventory will be fully allocated under the proposed schedule.

Remaining stock must be reassessed for expiry, storage conditions and production eligibility before use in future planning periods.

No previously expired or unverified ingredient inventory has been included.

---

## 10. Unmet Production Targets and Causes

| Product | Unmet Target | Primary Cause | Recommended Action |
|---|---:|---|---|
| Fish roti | 20 units | Insufficient fish inventory | Review additional fish purchasing requirements |
| Chicken kottu | 45 units | Wheat flour shortage following higher-priority allocation | Confirm replenishment and review chicken and egg requirements |
| Rice and curry packs | 40 units | Insufficient remaining chicken and batch increment restrictions | Review chicken procurement requirements |
| Pol sambol sachets | 35 units | Insufficient remaining production time | Review staffing and production capacity |
| Vegetable rolls | 0 units | Approved production target is zero | Maintain zero production |
| **Total** | **140 units** | | |

### Production Shortfall Calculation

`Unmet Production Target = Approved Production Target - Proposed Production`

`325 - 185 = 140 units`

### Overall Target Achievement

`(185 / 325) × 100 = 56.92%`

### Overall Production Shortfall Percentage

`(140 / 325) × 100 = 43.08%`

The difference between forecast demand and proposed production is not automatically equivalent to unmet customer demand because the approved production targets already incorporate finished-product inventory and safety stock considerations.

---

## 11. Production Bottlenecks and Resource Limitations

| Bottleneck | Impact | Severity |
|---|---|---|
| Staffing shortage | Prevents production on 6 December | Critical |
| Wheat flour shortage | Limits chicken kottu production | High |
| Fish shortage | Prevents completion of the highest-priority target | High |
| Chicken shortage | Restricts chicken kottu and rice and curry production | High |
| Shared production station | Prevents simultaneous batch production | High |
| Limited production time | Prevents the second pol sambol batch | High |
| Unconfirmed supplier deliveries | Cannot support current production allocations | High |
| Fixed batch durations | Partial batches require full production time | Medium |
| Unused vegetable inventory | Potential future inventory management concern | Medium |

Severity ratings are qualitative management assessments based on the supplied production constraints.

### Full Approved Target Capacity Assessment

| Product | Approved Target | Required Batches | Minutes per Batch | Total Required Minutes |
|---|---:|---:|---:|---:|
| Fish roti | 120 | 6 | 40 | 240 |
| Chicken kottu | 85 | 5 | 45 | 225 |
| Rice and curry packs | 50 | 2 | 50 | 100 |
| Pol sambol sachets | 70 | 2 | 30 | 60 |
| Vegetable rolls | 0 | 0 | 35 | 0 |
| **Total** | **325** | **15** | — | **625** |

Achieving all approved production targets would require 625 production minutes, assuming sufficient ingredients and staffing.

Only 375 feasible production minutes are available.

### Minimum Production Capacity Deficit

`625 - 375 = 250 minutes`

The minimum production capacity deficit is 250 minutes.

This deficit relates to achieving the full approved production targets under the supplied batch capacities and fixed batch durations.

Additional production capacity alone would not resolve the confirmed ingredient shortages.

---

## 12. Pending Procurement Assessment

| Ingredient | Pending Quantity | Procurement Status | Included in Schedule |
|---|---|---|---|
| Wheat flour | 5 kg | Draft order only; delivery unconfirmed | No |
| Grated coconut | 6 kg | Draft order only; price and delivery unconfirmed | No |
| Rice | Not confirmed | Provisional and unapproved | No |
| Chicken | Not confirmed | Provisional and unapproved | No |

The pending supplier deliveries associated with P03 Test B have been excluded from all production calculations.

No draft purchase order has been treated as a confirmed purchasing or delivery commitment.

The rice and chicken purchasing requirements associated with P02 Test B remain provisional and unapproved.

The proposed schedule should only be revised following:

1. Appropriate procurement approval.
2. Confirmed delivery arrangements.
3. Verified receipt of ingredients.
4. Ingredient storage and condition checks.
5. Confirmation of production eligibility.
6. Reassessment of staffing and production capacity.
7. Production manager approval.

---

## 13. Missing Information and Required Verification

| Missing Information or Verification | Required Action |
|---|---|
| Actual shift commencement time | Confirm before assigning clock-based batch times |
| Employee identities and task qualifications | Verify appropriate staffing assignments |
| Supplier delivery confirmation | Obtain verified delivery commitments and receipt records |
| Grated coconut purchase price | Verify supplier quotation |
| Procurement approval status | Obtain approval before issuing outstanding purchase orders |
| Additional staffing availability | Review without assuming additional staff |
| Ingredient batch identification and expiry details | Verify traceability and future-use eligibility |
| Product shelf life and dispatch requirements | Confirm suitability of production timing |
| Finished-product storage capacity | Confirm sufficient approved storage |
| Production manager approval | Obtain before implementing the schedule |

The missing information does not prevent preparation of a proposed schedule under the supplied synthetic constraints.

However, operational implementation requires further verification and approval.

The supplied inventory has already passed the relevant internal storage and condition checks for 5 and 6 December 2026. Missing detailed batch records must not be interpreted as invalidating that supplied confirmation.

---

## 14. Management Recommendations

### 14.1 Production Management

- Prioritise the proposed production of 100 fish roti units using confirmed available fish inventory.
- Allocate remaining wheat flour to 40 chicken kottu units.
- Produce 10 rice and curry packs using the remaining eligible chicken inventory.
- Allocate the remaining feasible production time to 35 pol sambol sachets.
- Maintain zero production for vegetable rolls in accordance with the approved production target.
- Maintain sequential batch scheduling without overlapping production activities.

### 14.2 Procurement Management

- Review identified wheat flour, chicken, fish, grated coconut and egg shortages.
- Obtain appropriate procurement approval before issuing purchase orders.
- Confirm pending supplier deliveries before including them in revised production calculations.
- Verify the missing grated coconut purchase price.
- Do not treat provisional purchasing requirements as approved purchases.
- Reassess purchasing requirements using updated inventory and approved production targets.

### 14.3 Staffing and Capacity Management

- Review the staffing shortage affecting 6 December 2026.
- Confirm that two appropriately qualified employees are available throughout each scheduled batch.
- Assess opportunities to improve future production capacity without exceeding approved limits.
- Do not assume additional employees, overtime or simultaneous production.

### 14.4 Inventory and Food Safety Management

- Reassess unused ingredient inventory for expiry, storage conditions and future production eligibility.
- Maintain appropriate ingredient and production batch traceability.
- Follow all approved food safety and quality management procedures.
- Do not introduce unapproved ingredient substitutions.
- Verify finished-product storage and dispatch arrangements.

### 14.5 Management Approval

- Obtain production manager approval before implementing the proposed production schedule.
- Recalculate the schedule if confirmed ingredient availability, staffing or production capacity changes.
- Document and approve any revised production allocations.

---

## 15. Final Production Performance Summary

| Performance Indicator | Result |
|---|---:|
| Total Forecast Demand | 470 units |
| Total Approved Production Target | 325 units |
| Total Proposed Production | 185 units |
| Total Unmet Production Target | 140 units |
| Approved Target Achievement | 56.92% |
| Approved Target Shortfall | 43.08% |
| Total Production Batches | 9 |
| Full Batches | 8 |
| Partial Batches | 1 |
| Full Target Production Time Requirement | 625 minutes |
| Feasible Production Time | 375 minutes |
| Allocated Production Time | 370 minutes |
| Remaining Production Time | 5 minutes |
| Minimum Full Target Capacity Deficit | 250 minutes |
| Production Time Utilisation | 98.67% |
| Scheduled Labour Consumption | 740 staff-minutes |
| Active Production Dates | 1 day |
| Unconfirmed Deliveries Included | None |
| Provisional Purchases Included | None |
| Production Limits Exceeded | None |
| Overlapping Batches | None |
| Unauthorised Overtime | None |
| Ingredient Substitutions | None |
| Production Manager Approval | Pending |

---

## 16. Production Compliance Validation

| Compliance Requirement | Validation Result |
|---|---|
| Approved production targets respected | Pass |
| Product-specific weekly limits respected | Pass |
| Maximum batch quantities respected | Pass |
| Partial batch quantities are valid multiples of five | Pass |
| Full production duration allocated to partial batches | Pass |
| Confirmed ingredient inventory limits respected | Pass |
| Required staffing levels maintained | Pass |
| Shared production station constraints respected | Pass |
| No overlapping production batches | Pass |
| Production priority order maintained | Pass |
| Maximum feasible higher-priority quantities allocated | Pass |
| Unconfirmed supplier deliveries excluded | Pass |
| Provisional purchasing requirements excluded | Pass |
| Previously excluded inventory not reused | Pass |
| No additional staffing assumed | Pass |
| No overtime assumed | Pass |
| No ingredient substitutions assumed | Pass |
| Missing information identified | Pass |
| Production bottlenecks identified | Pass |
| Unmet production targets identified | Pass |
| Approved food safety procedures not overridden | Pass – Planning constraint only |
| Production manager approval obtained | Pending |

### Compliance Checklist

- [x] Approved production targets respected.
- [x] Product-specific weekly production limits respected.
- [x] Maximum batch capacities respected.
- [x] Partial batch increments respected.
- [x] Fixed batch durations respected.
- [x] Confirmed ingredient inventory limits respected.
- [x] Staffing constraints respected.
- [x] Shared production station constraints respected.
- [x] Production priorities followed.
- [x] No overlapping production batches.
- [x] Unconfirmed deliveries excluded.
- [x] Provisional purchases excluded.
- [x] Previously excluded inventory not reused.
- [x] No additional staff or overtime assumed.
- [x] No ingredient substitutions assumed.
- [x] Production shortages and bottlenecks identified.
- [x] Missing information flagged.
- [ ] Operational verification completed.
- [ ] Production manager approval obtained.
- [ ] Production schedule authorised for implementation.

> The validation results confirm consistency with the supplied synthetic planning constraints only. They do not constitute operational food safety certification or production authorisation.

---

## 17. Conclusion

The proposed weekly production schedule enables Flavors of Ceylon to manufacture 185 food product units across nine production batches on 5 December 2026, subject to management approval.

The proposed schedule achieves 56.92% of the approved weekly production target while utilising 98.67% of feasible production time.

Ingredient shortages, staffing limitations and shared production station constraints prevent the completion of the remaining 140 approved production units.

The proposed schedule respects all supplied production priorities, ingredient availability, staffing requirements, batch durations and weekly production limits.

No unconfirmed supplier deliveries, provisional purchasing quantities, additional employees, overtime or ingredient substitutions have been included.

The schedule provides a structured basis for production manager review, procurement planning, inventory management and future production capacity assessment.

All proposed production quantities and scheduling arrangements remain subject to production manager review and approval.

---

## 18. Approval and Disclaimer

| Approval Field | Details |
|---|---|
| Prepared By | AI Production Planning Assistant |
| Business | Flavors of Ceylon |
| Prompt Reference | P04 v1.0 |
| Test Reference | Test B |
| Planning Date | 4 December 2026 |
| Reviewed By | Pending |
| Approved By | Production Manager – Pending |
| Approval Date | Pending |
| Document Status | Draft |
| Production Authorisation | Not granted |
| Intended Use | Academic Testing |

### Disclaimer

All recipes, quantities, capacities, durations, staffing records and dates are synthetic and created solely for academic testing.

This proposed production schedule does not establish actual food processing or food safety standards.

The AI-generated recommendations must not override approved food safety procedures, quality management requirements, staffing requirements or production limits.

All proposed production quantities, batch allocations and scheduling arrangements require production manager review and approval before implementation.

---

**End of Report**

**Flavors of Ceylon | P04 v1.0 | Test B | AI-Generated Output**

#### Evaluation

The response correctly allocated 185 production
units across nine batches using 370 of the
375 feasible production minutes.

The approved production target shortfall was
140 units, with target achievement of 56.92%.

All ingredient consumption and remaining-stock
calculations matched the expected results.

The response followed the production priority
order and excluded unconfirmed supplier deliveries,
provisional purchases and insufficiently staffed
production dates.

However, the 18-section report contained repeated
information, unrequested visualisations, subjective
severity ratings and AI-generated self-assessment.

Evaluation score: 9/10 (90%).

---

## 7. Version v1.1 — Revised Testing

### Test Case A

Testing date: 26 November 2026

AI tool and model: ChatGPT

#### Actual AI Output


# Flavors of Ceylon – P04 v1.1 – Test A

## Proposed Weekly Production Schedule

**Document Status:** Draft – Pending Production Manager Approval

| Planning Information | Details |
|---|---|
| Business | Flavors of Ceylon |
| Planning date | 4 December 2026 |
| Planning period | 1–7 December 2026 |
| Available production dates | 5–7 December 2026 |
| Related demand assessment | P01 Test C |
| Related inventory assessment | P02 Test A |
| Related procurement assessment | P03 Test A |
| Planning purpose | Academic testing and production planning |

---

## 1. Data Validation and Operational Constraints

### 1.1 Production Information Validation

| Validation Area | Findings |
|---|---|
| Approved production targets | Supplied for all five products. |
| Demand forecasts | Supplied but not used as direct production targets. |
| Ingredient consumption rates | Complete and supplied per 10 product units. |
| Ingredient measurement units | Consistent and suitable for calculations. |
| Available inventory | Confirmed and eligible for all available production dates under the synthetic scenario. |
| Received purchases | Already included in the updated inventory snapshot. |
| Batch sizes | Supplied for all products. |
| Partial batches | Permitted in multiples of five units. |
| Batch durations | Fixed, including partial batches. |
| Weekly production limits | Supplied for all products. |
| Staffing availability | Two staff members available on each production date. |
| Shared production station | One station available; simultaneous batches prohibited. |
| Shift starting times | Not supplied. Elapsed production minutes will be used. |
| Other ingredients and packaging | Verified as sufficient for approved targets. |
| Production approval | Pending Production Manager approval. |

### 1.2 Operational Constraints

- Production must not exceed approved targets or product-specific weekly limits.
- Each batch requires two staff members throughout its full duration.
- Only one batch may operate at a time.
- Each production date provides 360 net production minutes.
- Partial batches require the same production duration as full batches.
- No overtime, additional staff, ingredient substitutions or additional equipment are assumed.
- Received purchases of 15 kg of wheat flour and 12 kg of chicken must not be added again.
- Vegetable rolls must not be produced because their approved production target is zero.

No essential production information is missing that prevents the preparation of a proposed schedule. Actual shift starting times remain subject to confirmation.

---

## 2. Production Allocation and Batch Requirements

### 2.1 Proposed Production Allocation

Production is allocated according to the supplied priority order. All approved production targets can be achieved within the available ingredient, staffing and production capacity constraints.

| Priority | Product | Approved Target | Weekly Limit | Proposed Quantity | Unmet Target | Target Achievement |
|---:|---|---:|---:|---:|---:|---:|
| 1 | Fish roti | 120 | 120 | 120 | 0 | 100% |
| 2 | Chicken kottu | 85 | 100 | 85 | 0 | 100% |
| 3 | Rice and curry packs | 50 | 60 | 50 | 0 | 100% |
| 4 | Pol sambol sachets | 70 | 70 | 70 | 0 | 100% |
| 5 | Vegetable rolls | 0 | 60 | 0 | 0 | N/A |
| **Total** | | **325** | **410** | **325** | **0** | **100%** |

### 2.2 Batch Allocation and Production Time

| Product | Maximum Batch Size | Full-Target Minimum Batches | Proposed Batch Allocation | Minutes per Batch | Scheduled Minutes |
|---|---:|---:|---|---:|---:|
| Fish roti | 20 | 6 | 6 × 20 | 40 | 240 |
| Chicken kottu | 20 | 5 | (4 × 20) + (1 × 5) | 45 | 225 |
| Rice and curry packs | 25 | 2 | 2 × 25 | 50 | 100 |
| Pol sambol sachets | 35 | 2 | 2 × 35 | 30 | 60 |
| Vegetable rolls | 20 | 0 | No production | 35 | 0 |
| **Total** | | **15** | **325 units** | | **625** |

### 2.3 Essential Batch Calculations

#### Fish Roti

- Minimum batches = 120 / 20 = 6 batches.
- Production time = 6 × 40 = 240 minutes.

#### Chicken Kottu

- Minimum batches = 85 / 20, rounded upwards = 5 batches.
- Batch allocation = 20 + 20 + 20 + 20 + 5 = 85 units.
- Production time = 5 × 45 = 225 minutes.
- The partial batch of five units requires the full 45-minute duration.

#### Rice and Curry Packs

- Minimum batches = 50 / 25 = 2 batches.
- Production time = 2 × 50 = 100 minutes.

#### Pol Sambol Sachets

- Minimum batches = 70 / 35 = 2 batches.
- Production time = 2 × 30 = 60 minutes.

#### Vegetable Rolls

- Approved production target = 0 units.
- Required batches = 0.
- Production time = 0 minutes.

### 2.4 Binding Constraint Assessment

| Product | Allocation Constraint | Explanation |
|---|---|---|
| Fish roti | Approved target and weekly production limit | Both limits are reached at 120 units. |
| Chicken kottu | Approved production target | Production is restricted to 85 units despite a weekly limit of 100 units. |
| Rice and curry packs | Approved production target | Production is restricted to 50 units despite a weekly limit of 60 units. |
| Pol sambol sachets | Approved target and weekly production limit | Both limits are reached at 70 units. |
| Vegetable rolls | Zero approved production target | No additional production is allocated under the supplied target. |

There are no unmet approved production targets.

Differences between forecast demand and approved production targets must not be interpreted as confirmed unmet customer demand because the targets already incorporate finished-product inventory, safety stock and previous capacity assessments.

---

## 3. Ingredient Requirements and Reconciliation

### 3.1 Ingredient Requirement Calculation Method

The following formula is applied using the supplied recipe consumption rates:

**Ingredient requirement = (Production quantity / 10) × Ingredient quantity required per 10 units**

| Product | Calculated Ingredient Requirements |
|---|---|
| Fish roti | Wheat flour: 12 × 1.2 = 14.40 kg; Fish: 12 × 0.8 = 9.60 kg |
| Chicken kottu | Wheat flour: 8.5 × 2.0 = 17.00 kg; Chicken: 8.5 × 1.8 = 15.30 kg; Eggs: 8.5 × 10 = 85 units |
| Rice and curry packs | Rice: 5 × 1.5 = 7.50 kg; Chicken: 5 × 2.0 = 10.00 kg; Grated coconut: 5 × 0.3 = 1.50 kg |
| Pol sambol sachets | Grated coconut: 7 × 0.5 = 3.50 kg |
| Vegetable rolls | No ingredient consumption |

### 3.2 Consolidated Ingredient Reconciliation

| Ingredient | Unit | Confirmed Eligible Stock | Full-Target Requirement | Full-Target Shortage | Scheduled Consumption | Projected Remaining Stock |
|---|---|---:|---:|---:|---:|---:|
| Wheat flour | kg | 45.00 | 31.40 | 0.00 | 31.40 | 13.60 |
| Rice | kg | 40.00 | 7.50 | 0.00 | 7.50 | 32.50 |
| Chicken | kg | 30.00 | 25.30 | 0.00 | 25.30 | 4.70 |
| Grated coconut | kg | 12.00 | 5.00 | 0.00 | 5.00 | 7.00 |
| Fish | kg | 12.00 | 9.60 | 0.00 | 9.60 | 2.40 |
| Vegetables | kg | 10.00 | 0.00 | 0.00 | 0.00 | 10.00 |
| Eggs | units | 100 | 85 | 0 | 85 | 15 |

### 3.3 Sequential Inventory Allocation

Ingredient stock is allocated and deducted in production priority order.

#### Priority 1 – Fish Roti

Allocating 120 units leaves:

- Wheat flour: 30.60 kg.
- Fish: 2.40 kg.

#### Priority 2 – Chicken Kottu

Allocating 85 units leaves:

- Wheat flour: 13.60 kg.
- Chicken: 14.70 kg.
- Eggs: 15 units.

#### Priority 3 – Rice and Curry Packs

Allocating 50 units leaves:

- Rice: 32.50 kg.
- Chicken: 4.70 kg.
- Grated coconut: 10.50 kg.

#### Priority 4 – Pol Sambol Sachets

Allocating 70 units leaves:

- Grated coconut: 7.00 kg.

#### Priority 5 – Vegetable Rolls

- No ingredients are allocated.
- All 10.00 kg of vegetables remain in inventory.

### 3.4 Ingredient Shortage and Inventory Findings

**Full-target ingredient shortage:**

`Shortage = MAX(0, Full-target requirement - Confirmed eligible stock)`

**Projected remaining inventory:**

`Remaining stock = Confirmed eligible stock - Scheduled consumption`

All ingredient balances remain non-negative.

No ingredient shortages are identified, and no additional ingredient purchases are required to achieve the approved production targets under the supplied conditions.

The received wheat flour and chicken purchases have not been double-counted. No earlier inventory records or unconfirmed supplier deliveries have been incorporated.

---

## 4. Daily Production Schedule and Capacity

### 4.1 Proposed Daily Batch Schedule

Actual shift starting times have not been provided. Therefore, start and end times are expressed as elapsed production minutes from the beginning of each production day.

The proposed scheduling approach completes production over the first two available days while retaining 7 December as unused capacity. This is a proposed scheduling decision rather than a supplied operational requirement.

| Production Date | Batch Reference | Product | Batch Quantity | Start Minute | End Minute | Duration (min) | Staff Required |
|---|---|---|---:|---:|---:|---:|---:|
| 5 Dec 2026 | FR-01 | Fish roti | 20 | 0 | 40 | 40 | 2 |
| 5 Dec 2026 | FR-02 | Fish roti | 20 | 40 | 80 | 40 | 2 |
| 5 Dec 2026 | FR-03 | Fish roti | 20 | 80 | 120 | 40 | 2 |
| 5 Dec 2026 | FR-04 | Fish roti | 20 | 120 | 160 | 40 | 2 |
| 5 Dec 2026 | FR-05 | Fish roti | 20 | 160 | 200 | 40 | 2 |
| 5 Dec 2026 | FR-06 | Fish roti | 20 | 200 | 240 | 40 | 2 |
| 5 Dec 2026 | CK-01 | Chicken kottu | 20 | 240 | 285 | 45 | 2 |
| 5 Dec 2026 | CK-02 | Chicken kottu | 20 | 285 | 330 | 45 | 2 |
| 6 Dec 2026 | CK-03 | Chicken kottu | 20 | 0 | 45 | 45 | 2 |
| 6 Dec 2026 | CK-04 | Chicken kottu | 20 | 45 | 90 | 45 | 2 |
| 6 Dec 2026 | CK-05 | Chicken kottu | 5 | 90 | 135 | 45 | 2 |
| 6 Dec 2026 | RC-01 | Rice and curry packs | 25 | 135 | 185 | 50 | 2 |
| 6 Dec 2026 | RC-02 | Rice and curry packs | 25 | 185 | 235 | 50 | 2 |
| 6 Dec 2026 | PS-01 | Pol sambol sachets | 35 | 235 | 265 | 30 | 2 |
| 6 Dec 2026 | PS-02 | Pol sambol sachets | 35 | 265 | 295 | 30 | 2 |
| 7 Dec 2026 | N/A | No scheduled production | 0 | N/A | N/A | 0 | 0 |
| **Total** | **15 batches** | | **325** | | | **625** | |

Batch references are proposed identifiers created for this draft schedule.

### 4.2 Daily Capacity Summary

| Production Date | Available Staff | Feasible Available Minutes | Scheduled Minutes | Remaining Minutes | Capacity Utilisation | Staffing Restrictions |
|---|---:|---:|---:|---:|---:|---|
| 5 Dec 2026 | 2 | 360 | 330 | 30 | 91.67% | Both staff required throughout each batch. |
| 6 Dec 2026 | 2 | 360 | 295 | 65 | 81.94% | Both staff required throughout each batch. |
| 7 Dec 2026 | 2 | 360 | 0 | 360 | 0.00% | Both staff required if production is subsequently approved. |
| **Total** | | **1,080** | **625** | **455** | **57.87%** | |

### 4.3 Production Capacity Calculations

#### Total Feasible Available Production Time

`3 × 360 = 1,080 minutes`

#### Theoretical Full-Target Production Time

`240 + 225 + 100 + 60 = 625 minutes`

#### Feasible Scheduled Production Time

`330 + 295 + 0 = 625 minutes`

#### Remaining Production Time

`1,080 - 625 = 455 minutes`

#### Weekly Capacity Utilisation

**Formula:**

`Capacity utilisation = (Scheduled production minutes / Feasible available production minutes) × 100`

**Calculation:**

`(625 / 1,080) × 100 = 57.87%`

#### Overall Approved Target Achievement

**Formula:**

`Target achievement = (Proposed production / Approved production target) × 100`

**Calculation:**

`(325 / 325) × 100 = 100%`

#### Total Scheduled Staff Requirement

`625 × 2 = 1,250 staff-minutes`

The theoretical full-target production requirement equals the feasible scheduled production time because all approved targets can be accommodated within the individual daily production limits.

### 4.4 Schedule Validation

| Validation Requirement | Result |
|---|---|
| Approved production targets | All approved targets achieved without exceeding supplied quantities. |
| Product-specific weekly limits | All limits respected. |
| Ingredient availability | Scheduled consumption remains within eligible inventory. |
| Maximum batch sizes | All batches comply with product-specific maximum sizes. |
| Partial batch increments | Five-unit chicken kottu batch complies with permitted increments. |
| Fixed batch durations | Applied to every scheduled batch. |
| Daily production capacity | Neither scheduled production day exceeds 360 minutes. |
| Concurrent staffing | Two staff members required and available for each scheduled batch under the supplied scenario. |
| Shared production station | All batches scheduled sequentially without overlap. |
| Batch splitting | No individual batch is split across production dates. |
| Production priority | Supplied priority order maintained. |
| Zero-target products | No vegetable rolls scheduled. |
| Overtime and additional resources | None assumed. |
| Schedule reconciliation | Batch quantities and durations reconcile with ingredient consumption and production allocations. |

### 4.5 Potential Production Bottlenecks

| Bottleneck or Limitation | Supporting Evidence | Recommended Management Response |
|---|---|---|
| Shared production station | All products depend on one station. | Maintain sequential batch scheduling and approved cleaning procedures. |
| Staffing dependency | Two available staff members are required for every batch. | Confirm both staff members are available throughout scheduled production. |
| Chicken availability | 25.30 kg of the available 30 kg is allocated. | Monitor actual consumption against approved recipes. |
| Egg availability | 85 of the available 100 eggs are allocated. | Monitor consumption and maintain inventory records. |
| Fixed partial batch duration | Five units of chicken kottu require a full 45-minute batch. | Retain the full duration to achieve the approved target. |
| Product-specific weekly limits | Fish roti and pol sambol sachets reach their weekly limits. | Do not allocate additional quantities without an approved capacity and target revision. |
| Unused production capacity | 455 production minutes remain available. | Retain unused capacity without automatically increasing production quantities. |
| Missing shift starting times | Actual clock-based production times are not supplied. | Confirm shift starting times before issuing the operational schedule. |

---

## 5. Management Summary and Priority Actions

### 5.1 Key Production Indicators

| Performance Indicator | Calculated Result |
|---|---:|
| Total approved production target | 325 units |
| Total proposed production | 325 units |
| Total unmet production target | 0 units |
| Approved target achievement | 100% |
| Total production batches | 15 |
| Theoretical full-target production time | 625 minutes |
| Scheduled production time | 625 minutes |
| Feasible available production time | 1,080 minutes |
| Remaining production capacity | 455 minutes |
| Weekly capacity utilisation | 57.87% |
| Scheduled staff requirement | 1,250 staff-minutes |
| Ingredients with identified shortages | 0 |
| Additional ingredient purchases required | None under supplied conditions |
| Scheduled production days | 2 |
| Unused available production days | 1 |

### 5.2 Management Summary

The proposed schedule achieves all 325 approved production units through 15 batches completed on 5 and 6 December 2026. All verified ingredient quantities, staffing requirements, batch restrictions and weekly production limits are satisfied. No ingredient shortages or unmet production targets are identified. Production requires 625 of the available 1,080 minutes, resulting in 57.87% capacity utilisation. The remaining 455 minutes provide scheduling flexibility without authorising additional production. Key operational dependencies include the shared production station, continuous availability of two staff members and controlled ingredient consumption. Vegetable rolls remain excluded due to their zero approved target. Implementation remains subject to production manager approval and established food safety procedures.

### 5.3 Priority Management Actions

1. Obtain Production Manager approval before implementing the proposed schedule.
2. Confirm actual shift starting times and continuous availability of both staff members.
3. Verify ingredient eligibility and stock availability before scheduled production.
4. Monitor actual batch quantities, ingredient consumption and production durations against the approved plan.
5. Retain unused capacity for approved operational requirements without exceeding production targets or weekly limits.

---

**Final Production Planning Status:** Draft – Pending Production Manager Approval.

**Production Feasibility Conclusion:** All approved production targets are achievable under the supplied synthetic conditions without additional ingredients, staffing, equipment or overtime.

**Food Safety and Authorisation Disclaimer:** This production schedule has been prepared solely for academic testing using supplied synthetic business information. It does not independently certify ingredient suitability, establish food safety standards, authorise production or override approved food safety and operational procedures.

#### Evaluation

Pending evaluation.

### Test Case B

Testing date: 26 November 2026

AI tool and model: ChatGPT

#### Actual AI Output


# Flavors of Ceylon – Proposed Weekly Production Schedule

## P04 v1.1 – Test B

| Planning Information | Details |
| --- | --- |
| Business | Flavors of Ceylon |
| Planning Date | 4 December 2026 |
| Planning Period | 1–7 December 2026 |
| Available Production Dates | 5–7 December 2026 |
| Related Assessments | P01 Test C, P02 Test B and P03 Test B |
| Schedule Status | Draft – Pending Production Manager Approval |
| Assessment Purpose | Synthetic Academic Testing |

---

## 1. Data Validation and Operational Constraints

### 1.1 Production Information Validation

The supplied production targets, ingredient consumption rates, verified inventory, batch requirements and staffing information have been reviewed to determine feasible production quantities.

Approved production targets are used instead of forecast demand because finished-product inventory, safety stock and previous capacity adjustments have already been incorporated.

| Validation Area | Findings |
| --- | --- |
| Approved production targets | Supplied for all five products |
| Demand forecasts | Available for reference only |
| Ingredient consumption rates | Complete and specified per 10 product units |
| Measurement units | Consistent and compatible |
| Confirmed ingredient inventory | Verified under the supplied synthetic scenario |
| Batch sizes and durations | Supplied for all products |
| Partial batch restrictions | Permitted in multiples of 5 units |
| Weekly production limits | All approved targets are within product-specific limits |
| Staffing requirements | Two concurrent employees required per batch |
| Shared production resources | One production station; simultaneous batches prohibited |
| Other ingredients and packaging | Confirmed sufficient for approved targets |
| Actual shift starting times | Not supplied; elapsed production minutes will be used |
| Setup and cleaning | Already included in fixed batch durations |

No essential numerical production information is missing. No negative ingredient quantities or invalid production targets have been identified.

### 1.2 Excluded Purchasing Requirements

The following purchasing requirements must not be included in available production inventory.

| Ingredient | Quantity | Exclusion Reason |
| --- | ---: | --- |
| Wheat flour | 5 kg | Draft purchase order; delivery unconfirmed |
| Grated coconut | 6 kg | Price and delivery unconfirmed |
| Rice | Not supplied | Provisional and unapproved purchase |
| Chicken | Not supplied | Provisional and unapproved purchase |

Previously expired and unverified inventory identified in P02 remains excluded.

Only the updated verified inventory snapshot is used. No pending purchases or unconfirmed supplier deliveries are counted as available inventory.

### 1.3 Staffing and Operational Constraints

- **5 December 2026:** Two employees available for 375 production minutes. Eligible for production scheduling.
- **6 December 2026:** Only one employee available. Production cannot be scheduled because every batch requires two concurrent employees.
- **7 December 2026:** No employees or production minutes available.
- All products use one shared production station.
- Only one production batch may operate at a time.
- Both required employees must be available throughout each batch.
- Fixed production durations include setup and cleaning allowances.
- No overtime, additional employees or ingredient substitutions are assumed.

Although 735 net production minutes are listed across the planning dates, only **375 minutes are feasible for production** under the supplied staffing and shared-resource constraints.

---

## 2. Production Allocation and Batch Requirements

### 2.1 Full-Target Batch Requirements

The following calculations represent the theoretical resources required to achieve all approved production targets before applying ingredient and staffing constraints.

**Calculation formulas:**

- Minimum batches required = Approved production target / Maximum batch size, rounded upwards.
- Required production minutes = Minimum batches required × Fixed batch duration.

Full fixed batch durations apply to both full and partial batches.

| Product (Priority Order) | Forecast Demand | Approved Target | Required Batch Allocation | Minimum Batches | Required Minutes |
| --- | ---: | ---: | --- | ---: | ---: |
| Fish roti | 160 | 120 | 6 × 20 | 6 | 240 |
| Chicken kottu | 90 | 85 | 4 × 20 + 1 × 5 | 5 | 225 |
| Rice and curry packs | 60 | 50 | 2 × 25 | 2 | 100 |
| Pol sambol sachets | 80 | 70 | 2 × 35 | 2 | 60 |
| Vegetable rolls | 80 | 0 | None | 0 | 0 |
| **Total** | **470** | **325** | — | **15** | **625** |

The full approved production targets require 625 production minutes.

**Theoretical capacity shortfall:**

    625 - 375 = 250 minutes

This represents a theoretical capacity shortfall of 250 minutes before considering ingredient shortages.

### 2.2 Feasible Production Allocation Calculations

#### Priority 1 – Fish Roti

Fish availability limits production to:

    Maximum fish-supported production
    = (8 / 0.8) × 10
    = 100 units

Proposed allocation:

- Approved production target: 120 units.
- Feasible production: 100 units.
- Batch allocation: 5 batches of 20 units.
- Production time: 5 × 40 = 200 minutes.
- Wheat flour consumed: (100 / 10) × 1.2 = 12 kg.
- Fish consumed: (100 / 10) × 0.8 = 8 kg.
- Remaining wheat flour: 20 - 12 = 8 kg.
- Remaining fish: 8 - 8 = 0 kg.
- Remaining production time: 375 - 200 = 175 minutes.
- Unmet production target: 120 - 100 = 20 units.

**Binding constraint:** Insufficient fish inventory.

#### Priority 2 – Chicken Kottu

After allocating fish roti production, 8 kg of wheat flour remains.

    Maximum flour-supported production
    = (8 / 2.0) × 10
    = 40 units

Proposed allocation:

- Approved production target: 85 units.
- Feasible production: 40 units.
- Batch allocation: 2 batches of 20 units.
- Production time: 2 × 45 = 90 minutes.
- Wheat flour consumed: (40 / 10) × 2.0 = 8 kg.
- Chicken consumed: (40 / 10) × 1.8 = 7.2 kg.
- Eggs consumed: (40 / 10) × 10 = 40 units.
- Remaining wheat flour: 8 - 8 = 0 kg.
- Remaining chicken: 10 - 7.2 = 2.8 kg.
- Remaining eggs: 60 - 40 = 20 units.
- Remaining production time: 175 - 90 = 85 minutes.
- Unmet production target: 85 - 40 = 45 units.

**Binding constraint:** Remaining wheat flour inventory.

#### Priority 3 – Rice and Curry Packs

Remaining chicken inventory after chicken kottu production:

    10 - 7.2 = 2.8 kg

Maximum ingredient-supported production:

    (2.8 / 2.0) × 10 = 14 units

As partial batches must be produced in multiples of five, feasible production is reduced to 10 units.

Proposed allocation:

- Approved production target: 50 units.
- Feasible production: 10 units.
- Batch allocation: 1 partial batch of 10 units.
- Production time: 1 × 50 = 50 minutes.
- Rice consumed: (10 / 10) × 1.5 = 1.5 kg.
- Chicken consumed: (10 / 10) × 2.0 = 2 kg.
- Grated coconut consumed: (10 / 10) × 0.3 = 0.3 kg.
- Remaining rice: 15 - 1.5 = 13.5 kg.
- Remaining chicken: 2.8 - 2 = 0.8 kg.
- Remaining grated coconut: 4 - 0.3 = 3.7 kg.
- Remaining production time: 85 - 50 = 35 minutes.
- Unmet production target: 50 - 10 = 40 units.

**Binding constraints:** Remaining chicken inventory and permitted partial batch increments.

#### Priority 4 – Pol Sambol Sachets

There are 35 production minutes remaining.

Each batch requires 30 minutes and accommodates a maximum of 35 units.

The remaining grated coconut inventory of 3.7 kg is sufficient for the proposed batch.

    Maximum batches supported by remaining time
    = 35 / 30, rounded down
    = 1 batch

Proposed allocation:

- Approved production target: 70 units.
- Feasible production: 35 units.
- Batch allocation: 1 batch of 35 units.
- Production time: 1 × 30 = 30 minutes.
- Grated coconut consumed: (35 / 10) × 0.5 = 1.75 kg.
- Remaining grated coconut: 3.7 - 1.75 = 1.95 kg.
- Remaining production time: 35 - 30 = 5 minutes.
- Unmet production target: 70 - 35 = 35 units.

**Binding constraint:** Available production time.

#### Priority 5 – Vegetable Rolls

The approved production target is zero. Therefore, no production is allocated regardless of forecast demand or remaining ingredient inventory.

- Approved production target: 0 units.
- Feasible production: 0 units.
- Batch allocation: None.
- Production time: 0 minutes.
- Ingredient consumption: None.
- Unmet production target: 0 units.

**Binding constraint:** Zero approved production target.

### 2.3 Consolidated Production Allocation

| Product | Approved Target | Proposed Quantity | Batch Allocation | Minutes | Unmet Target | Binding Constraint |
| --- | ---: | ---: | --- | ---: | ---: | --- |
| Fish roti | 120 | 100 | 5 × 20 | 200 | 20 | Fish shortage |
| Chicken kottu | 85 | 40 | 2 × 20 | 90 | 45 | Wheat flour shortage |
| Rice and curry packs | 50 | 10 | 1 × 10 | 50 | 40 | Chicken shortage and batch increments |
| Pol sambol sachets | 70 | 35 | 1 × 35 | 30 | 35 | Available production time |
| Vegetable rolls | 0 | 0 | None | 0 | 0 | Zero approved target |
| **Total** | **325** | **185** | **9 batches** | **370** | **140** | — |

**Unmet production target formula:**

    Unmet production target
    = Approved production target - Feasible production

The proposed allocation follows the strict production priority order without reducing higher-priority production to increase lower-priority output.

The 140 unmet units represent unmet approved production targets, not confirmed unmet customer demand.

### 2.4 Production Target Achievement

**Calculation formula:**

    Target achievement (%)
    = (Proposed production / Approved production target) × 100

| Product | Target Achievement |
| --- | ---: |
| Fish roti | 83.33% |
| Chicken kottu | 47.06% |
| Rice and curry packs | 20.00% |
| Pol sambol sachets | 50.00% |
| Vegetable rolls | Not applicable |
| **Overall Target Achievement** | **56.92%** |

**Overall target achievement calculation:**

    (185 / 325) × 100 = 56.92%

The vegetable rolls target achievement percentage is not applicable because the approved production target is zero.

---

## 3. Ingredient Requirements and Reconciliation

### 3.1 Calculation Methodology

Ingredient requirements are calculated using the supplied consumption rates per 10 product units.

**Ingredient requirement:**

    Ingredient requirement
    = (Production quantity / 10) × Ingredient quantity per 10 units

**Full-target ingredient shortage:**

    Full-target ingredient shortage
    = MAX(0, Full-target requirement - Confirmed eligible stock)

**Projected remaining inventory:**

    Projected remaining stock
    = Confirmed eligible stock - Scheduled consumption

For example, the full-target wheat flour requirement is:

    [(120 / 10) × 1.2] + [(85 / 10) × 2.0]
    = 14.4 + 17.0
    = 31.4 kg

The scheduled wheat flour consumption is:

    [(100 / 10) × 1.2] + [(40 / 10) × 2.0]
    = 12 + 8
    = 20 kg

### 3.2 Consolidated Ingredient Reconciliation

| Ingredient | Unit | Confirmed Eligible Stock | Full-Target Requirement | Full-Target Shortage | Scheduled Consumption | Projected Remaining Stock |
| --- | --- | ---: | ---: | ---: | ---: | ---: |
| Wheat flour | kg | 20.00 | 31.40 | 11.40 | 20.00 | 0.00 |
| Rice | kg | 15.00 | 7.50 | 0.00 | 1.50 | 13.50 |
| Chicken | kg | 10.00 | 25.30 | 15.30 | 9.20 | 0.80 |
| Grated coconut | kg | 4.00 | 5.00 | 1.00 | 2.05 | 1.95 |
| Fish | kg | 8.00 | 9.60 | 1.60 | 8.00 | 0.00 |
| Vegetables | kg | 10.00 | 0.00 | 0.00 | 0.00 | 10.00 |
| Eggs | units | 60 | 85 | 25 | 40 | 20 |

### 3.3 Ingredient Reconciliation Findings

- **Wheat flour:** Fully consumed by the proposed fish roti and chicken kottu production.
- **Fish:** Fully consumed by the proposed fish roti production.
- **Chicken:** The remaining 0.80 kg is insufficient for an additional permitted five-unit batch of rice and curry packs, which requires 1 kg.
- **Grated coconut:** Remaining inventory could support further pol sambol production, but insufficient production time prevents another batch.
- **Rice:** Remaining inventory is available after the proposed allocations, subject to subsequent eligibility verification.
- **Eggs:** Remaining inventory cannot support additional chicken kottu production because wheat flour is exhausted.
- **Vegetables:** Remain unused because vegetable rolls have a zero approved production target.

All scheduled ingredient consumption is within confirmed available inventory.

No ingredient has a negative projected balance.

No ingredient inventory has been allocated more than once.

No pending supplier deliveries, provisional purchases, expired ingredients or unverified stock have been included.

Full-target shortages represent theoretical ingredient gaps against approved targets and do not constitute authorised purchasing quantities.

---

## 4. Daily Production Schedule and Capacity

### 4.1 Proposed Daily Batch Schedule

Actual shift starting times have not been supplied. Therefore, the following schedule uses elapsed production minutes beginning at minute zero.

Batch references are proposed identifiers created for this draft schedule.

| Production Date | Batch Reference | Product | Quantity | Start Minute | End Minute | Duration (Minutes) | Concurrent Staff |
| --- | --- | --- | ---: | ---: | ---: | ---: | ---: |
| 5 Dec 2026 | FR-01 | Fish roti | 20 | 0 | 40 | 40 | 2 |
| 5 Dec 2026 | FR-02 | Fish roti | 20 | 40 | 80 | 40 | 2 |
| 5 Dec 2026 | FR-03 | Fish roti | 20 | 80 | 120 | 40 | 2 |
| 5 Dec 2026 | FR-04 | Fish roti | 20 | 120 | 160 | 40 | 2 |
| 5 Dec 2026 | FR-05 | Fish roti | 20 | 160 | 200 | 40 | 2 |
| 5 Dec 2026 | CK-01 | Chicken kottu | 20 | 200 | 245 | 45 | 2 |
| 5 Dec 2026 | CK-02 | Chicken kottu | 20 | 245 | 290 | 45 | 2 |
| 5 Dec 2026 | RC-01 | Rice and curry packs | 10 | 290 | 340 | 50 | 2 |
| 5 Dec 2026 | PS-01 | Pol sambol sachets | 35 | 340 | 370 | 30 | 2 |
| **Total** | **9 batches** | — | **185** | — | — | **370** | — |

No production is scheduled on 6 or 7 December 2026 due to insufficient staffing.

### 4.2 Daily Capacity Summary

| Date | Available Staff | Supplied Minutes | Feasible Available Minutes | Scheduled Minutes | Remaining Feasible Minutes | Staffing Restriction |
| --- | ---: | ---: | ---: | ---: | ---: | --- |
| 5 Dec 2026 | 2 | 375 | 375 | 370 | 5 | Staffing requirement satisfied |
| 6 Dec 2026 | 1 | 360 | 0 | 0 | 0 | Insufficient concurrent staff |
| 7 Dec 2026 | 0 | 0 | 0 | 0 | 0 | No staff available |
| **Total** | — | **735** | **375** | **370** | **5** | — |

The 360 minutes listed for 6 December are unavailable for batch production because the minimum staffing requirement cannot be satisfied.

These minutes are not included in feasible production capacity.

Production minutes are not pooled across dates without validating the applicable staffing and daily capacity constraints.

### 4.3 Capacity Utilisation

**Calculation formula:**

    Capacity utilisation (%)
    = (Scheduled production minutes / Feasible available production minutes) × 100

**Calculation:**

    Capacity utilisation
    = (370 / 375) × 100
    = 98.67%

| Performance Indicator | Calculated Result |
| --- | ---: |
| Total approved production target | 325 units |
| Total proposed production | 185 units |
| Total unmet production target | 140 units |
| Overall production target achievement | 56.92% |
| Theoretical full-target batch requirement | 15 batches |
| Proposed production batches | 9 batches |
| Theoretical full-target production time | 625 minutes |
| Total supplied production time | 735 minutes |
| Feasible available production time | 375 minutes |
| Total scheduled production time | 370 minutes |
| Remaining feasible production time | 5 minutes |
| Production capacity utilisation | 98.67% |
| Production time excluded due to insufficient staffing | 360 minutes |
| Theoretical full-target capacity shortfall | 250 minutes |

Capacity utilisation for 6 and 7 December is not applicable because feasible available production time is zero.

The remaining five minutes on 5 December cannot accommodate another batch because the shortest supplied batch duration is 30 minutes.

### 4.4 Schedule Validation

| Validation Requirement | Schedule Findings |
| --- | --- |
| Approved production targets | No target exceeded |
| Product-specific weekly limits | No weekly limit exceeded |
| Ingredient inventory | All consumption within verified stock |
| Ingredient allocation | No double-counting or duplicate allocation |
| Maximum batch sizes | All batch quantities within permitted limits |
| Partial batch increments | All quantities comply with five-unit increments |
| Fixed batch durations | Full duration applied to every batch |
| Concurrent staffing | Two employees allocated throughout every batch |
| Shared production station | No overlapping batches |
| Daily production capacity | All batches completed within 375 available minutes |
| Ingredient eligibility | All production scheduled on an eligible date |
| Batch splitting | No batches split across dates |
| Production priority | Strict priority order maintained |
| Zero approved production targets | No vegetable rolls production scheduled |
| Unconfirmed deliveries | Excluded |
| Provisional purchases | Excluded |
| Overtime and additional staff | Not assumed |
| Ingredient substitutions | Not assumed |
| Quantity reconciliation | All nine batches reconcile to 185 proposed units |
| Production time reconciliation | All scheduled batches reconcile to 370 minutes |

The proposed schedule is mathematically and operationally feasible within the supplied synthetic constraints, subject to production manager approval.

---

## 5. Management Summary and Priority Actions

### 5.1 Management Summary

Flavors of Ceylon can feasibly produce **185 of the 325 approved product units**, achieving **56.92% of its production target**.

The proposed schedule comprises nine batches on 5 December 2026, consuming 370 of 375 feasible production minutes and achieving **98.67% capacity utilisation**.

Fish, wheat flour and chicken availability restrict higher-priority production. Insufficient staffing on 6 December removes 360 potential production minutes, while limited remaining time prevents further pol sambol production.

The schedule maintains strict production priorities, verified inventory limits, batch restrictions and shared-station requirements. The remaining 140 units represent unmet production targets requiring management review. Unconfirmed supplier deliveries and provisional purchasing requirements remain excluded.

### 5.2 Recommended Priority Actions

| Priority | Recommended Action |
| ---: | --- |
| 1 | Obtain production manager approval for the proposed schedule and allocations. |
| 2 | Review staffing availability for 6 December before considering additional production. |
| 3 | Review full-target ingredient shortages and obtain procurement approval for any necessary replenishment. |
| 4 | Verify supplier pricing, delivery commitments and received ingredient eligibility before updating inventory. |
| 5 | Reassess unmet production targets following confirmed changes to staffing, inventory or approved capacity. |

### 5.3 Assumptions and Limitations

- All production calculations are based exclusively on supplied synthetic business information.
- Actual shift starting times are unavailable.
- Elapsed production minutes are used instead of actual clock times.
- Batch references are proposed identifiers for this draft.
- Staffing availability is applied to the supplied net scheduling periods.
- No additional staffing or overtime is assumed.
- No ingredient substitutions are assumed.
- No unconfirmed supplier deliveries are included.
- No provisional purchasing requirements are included.
- Ingredient eligibility beyond the supplied verified production dates is not assumed.
- Unmet production targets are not treated as confirmed unmet customer demand.
- No actual food safety certification or production authorisation is provided.

### 5.4 Final Schedule Status

> **DRAFT – PENDING PRODUCTION MANAGER APPROVAL**
>
> All proposed production quantities, ingredient allocations and batch schedules require production manager review and approval before implementation.

**Disclaimer:** All recipes, quantities, staffing records, production durations, capacities and dates are synthetic and intended solely for academic testing. This proposed schedule does not certify ingredient suitability, establish actual food safety standards, authorise production or override approved food safety procedures.

---

**End of P04 v1.1 – Test B Output**

#### Evaluation

Pending evaluation.

---

## 8. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 9/10 | 18/20 (90%) |
| v1.1 | Pending | Pending | Pending |

### Initial Evaluation Scores

| Criterion | Test A | Test B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 2 |
| Business Relevance | 1 | 1 |
| Responsible AI | 2 | 2 |
| Total | 9/10 | 9/10 |

### Improvement Opportunities

- Introduce a concise five-section report.
- Standardise priority-based resource allocation.
- Explicitly validate daily staffing and batch
  scheduling feasibility.
- Consolidate ingredient consumption calculations.
- Distinguish full-target ingredient shortages
  from scheduled production consumption.
- Avoid unsupported risk thresholds.
- Remove unnecessary charts and self-assessment.
- Retain existing operational safeguards.

All numerical benchmarks were achieved during
initial testing.

The evaluation measures response quality under
synthetic scenarios rather than actual commercial
manufacturing performance.

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
