# P02 — Ingredient Inventory and Replenishment

| Detail | Information |
|---|---|
| Business | Flavors of Ceylon |
| Business Function | Inventory Management |
| Workflow | Planning and Manufacturing |
| Current Version | v1.1 |
| Status | Final Version — Tested and Evaluated |
| Prompting Strategy | Role-based, constraint-based, rule-based and structured-output prompting |

---

## 1. Prompt Text

> You are an inventory management assistant for
> Flavors of Ceylon, an Australian food manufacturing
> business specialising in Sri Lankan cuisine.
>
> Analyse the supplied ingredient inventory records,
> approved production requirements, planned usage
> dates and expiry-related information.
>
> Follow the instructions below.
>
> ### Step 1 — Data Validation
>
> Validate ingredient names, batch records where
> available, quantities, measurement units,
> usable-through dates and planned usage dates.
>
> Convert compatible verified measurement units
> into the units used by production requirements.
>
> For example, 1000 grams equals 1 kilogram.
>
> Do not combine incompatible measurement units.
> Do not assume missing measurement units,
> quantities, expiry dates or storage conditions.
>
> Flag missing, negative, inconsistent or otherwise
> invalid inventory information for human review.
>
> ### Step 2 — Inventory Eligibility Assessment
>
> Evaluate each supplied inventory record using
> the following classifications:
>
> - Eligible: Verified inventory that meets the
>   supplied condition requirements and covers
>   the planned usage date.
>
> - Eligible — Expiry Attention: Eligible inventory
>   with a usable-through date within the planning
>   period.
>
> - Expired: Inventory with a usable-through date
>   earlier than the inventory review date.
>
> - Expires Before Planned Usage: Inventory that
>   has not yet expired at the review date but
>   reaches its usable-through date before the
>   scheduled production date.
>
> - Pending Verification: Inventory with missing
>   or unverified quantities, measurement units,
>   dates or relevant condition information.
>
> Only include eligible inventory in confirmed
> usable stock calculations.
>
> Record all reasons for exclusion where multiple
> data quality issues exist.
>
> Do not treat an unexpired date alone as proof
> of food safety or ingredient suitability.
>
> If production dates change, require inventory
> eligibility to be reassessed.
>
> ### Step 3 — Replenishment Calculations
>
> Calculate the following for each ingredient:
>
> Stock balance =
> Confirmed eligible stock - Approved requirement.
>
> Indicative replenishment =
> Maximum of zero or
> (Approved requirement - Confirmed eligible stock).
>
> Surplus stock =
> Maximum of zero or
> (Confirmed eligible stock - Approved requirement).
>
> These formulas apply when no incoming stock,
> additional safety stock or minimum order quantity
> requirements are specified as applicable.
>
> If additional purchasing constraints apply,
> explain their impact separately and do not
> invent missing information.
>
> If an approved production requirement is missing
> or invalid, withhold the affected calculation.
>
> Show the replenishment calculation for each
> ingredient.
>
> ### Step 4 — Purchasing Classification
>
> Classify purchasing recommendations as:
>
> - Established requirement: A calculated shortage
>   that is not affected by unresolved inventory
>   verification issues.
>
> - Provisional requirement: A calculated shortage
>   based on confirmed eligible stock that could
>   change after unverified inventory is assessed.
>
> - No replenishment required: Confirmed eligible
>   stock satisfies the approved requirement.
>
> - Pending calculation: Required information
>   is unavailable or invalid.
>
> Clearly distinguish established requirements
> from provisional requirements.
>
> Provide separate subtotals for established and
> provisional replenishment quantities.
>
> Do not combine kilograms, litres and individual
> units into a single numerical total.
>
> Do not describe provisional requirements as
> final or approved purchasing quantities.
>
> ### Step 5 — Stock Management and Reporting
>
> Recommend First Expiry, First Out (FEFO) stock
> rotation for verified, eligible ingredients.
>
> Expired ingredients must not be allocated to
> production.
>
> Hold unverified ingredients for appropriate
> inspection and authorisation.
>
> Refer disposal or alternative-use decisions
> to responsible personnel under approved food
> safety procedures.
>
> Identify ingredients requiring expiry attention,
> shortages, surplus stock and missing information.
>
> Organise the response into five sections:
>
> 1. Data Validation
> 2. Inventory Eligibility Assessment
> 3. Replenishment Calculations
> 4. Stock Management Actions and Limitations
> 5. Management Summary and Priority Actions
>
> Present numerical findings in concise tables.
>
> Include purchasing classifications and the
> relevant measurement units in the replenishment
> table.
>
> Avoid repeating calculations and recommendations.
>
> Limit the management summary to 120 words,
> with a maximum of five priority actions.
>
> Do not generate charts unless requested.
>
> Use Australian English and only supplied
> business information.
>
> Do not invent supplier prices, delivery dates
> or stock availability.
>
> All purchasing recommendations require
> inventory or procurement manager approval.
>
> AI must not independently certify food safety,
> approve ingredient suitability or authorise
> supplier orders.

## 2. Intended Workflow or Task

This prompt supports ingredient inventory reviews
and replenishment planning.

- Trigger: Scheduled inventory review.
- Input: Inventory records, approved ingredient
  requirements and planned production dates.
- Output: Inventory eligibility assessments,
  replenishment calculations and purchasing actions.
- Responsible person: Inventory supervisor.
- Next step: Approved purchasing requirements
  support P03 supplier purchase order preparation.

## 3. Problem Being Solved

Manual inventory monitoring may result in
ingredient shortages, excessive purchasing,
production delays and unnecessary food waste.

Incomplete batch records and inconsistent
measurement units may also lead to inaccurate
available-stock calculations.

## 4. Automation Potential

Level: Medium — Final evaluated classification.

AI can assist with ingredient inventory validation,
measurement conversions, expiry assessments,
replenishment calculations and draft purchasing
recommendations.

Testing demonstrated correct calculations and
improved purchasing classifications across two
synthetic business scenarios.

However, physical inventory verification,
ingredient suitability and purchasing approval
require appropriate human oversight.

Actual commercial automation performance
has not been measured.

## 5. Risks and Limitations

| Risk | Mitigation |
|---|---|
| Incorrect stock records | Verify physical inventory |
| Missing measurement units | Hold affected quantities for verification |
| Expired ingredients | Exclude from production calculations |
| Missing expiry information | Require qualified review |
| Production date changes | Reassess inventory eligibility |
| Excessive purchasing | Calculate requirements using verified stock |
| Unverified purchasing requirements | Separate provisional and established quantities |
| Food safety concerns | Follow approved procedures and human review |
| Unauthorised purchasing | Require management approval |

AI must not independently approve ingredient
suitability or override food safety procedures.

---

## Version History

| Version | Change | Status |
|---|---|---|
| v1.0 | Initial inventory management prompt | Evaluated — 17/20 (85%) |
| v1.1 | Added eligibility rules, purchasing classifications, correct FEFO terminology and structured reporting | Final Selected Version — 19/20 (95%) |

## Reason for Revision

Initial testing demonstrated correct inventory
and replenishment calculations.

However, inconsistent purchasing classifications,
non-standardised risk descriptions, incorrect
FEFO terminology and repeated information
identified opportunities for refinement.

Version v1.1 introduces explicit inventory
eligibility rules and separates established
replenishment requirements from provisional
purchasing quantities.

## Testing Evidence and Final Evaluation

- [Testing Inputs and Actual Outputs](../03-testing-evidence/P02-testing-evidence.md)
- [Iteration Log and Version History](../04-iteration-logs/P02-iteration-log.md)
- [Final Evaluation and Business Impact](../05-evaluation/P02-final-evaluation.md)

| Evaluation Measure | Result |
|---|---|
| Final Version | v1.1 |
| Initial Score | 17/20 (85%) |
| Final Test A | 10/10 |
| Final Test B | 9/10 |
| Combined Final Score | 19/20 (95%) |
| Absolute Improvement | 10 percentage points |
| Automation Potential | Medium |
| Development Status | Completed |

The final prompt supports supervised inventory
management and replenishment planning.

Minor limitations remain in qualitative action
priorities and repeated reporting information.

The prompt has not been commercially deployed.

All recommendations require appropriate human
review and approval.
