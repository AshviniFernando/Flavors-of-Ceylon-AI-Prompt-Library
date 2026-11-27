# P10 — Weekly Business Performance Reporting: Testing Evidence

## 1. Testing Information

| Detail | Information |
|---|---|
| Prompt ID | P10 |
| Business | Flavors of Ceylon |
| Business Function | Management and Business Intelligence |
| Initial Version | v1.0 |
| Data Type | Synthetic integrated business data |
| Testing Status | In Progress |

## 2. Testing Objective

Evaluate whether generative AI can integrate sales,
demand forecasts, inventory, procurement, production,
financial information, food safety, customer feedback
and marketing records into a professional weekly
management report.

Testing evaluates numerical accuracy, KPI calculation,
evidence reconciliation, management relevance,
uncertainty handling and responsible AI safeguards.

## 3. Integrated Business Workflow

P10 integrates information from:

- P01: Product demand forecasting.
- P02: Ingredient inventory and replenishment.
- P03: Supplier purchase order preparation.
- P04: Production and batch planning.
- P05: Food safety and quality incident reporting.
- P06: Product label and allergen information review.
- P07: Customer enquiry response.
- P08: Customer complaint and feedback analysis.
- P09: Digital marketing content generation.

AI-generated plans must not be treated as evidence
of completed operational activities.

Management decisions remain subject to appropriate
human verification and authorisation.

## 4. Test Case A — Standard Weekly Management Report

### Test Input

WEEKLY REPORTING INFORMATION

Business: Flavors of Ceylon.
Business location: Dandenong South,
Victoria, Australia.

Report reference: FOC-WBR-2026-001.
Report preparation date: 8 December 2026.

Reporting period:
1–7 December 2026, inclusive.

Responsible reviewer:
Business Operations Manager.

Specialist reviewers:
Finance Manager.
Production Manager.
Food Safety Supervisor.
Quality Assurance Manager.
Customer Experience Manager.
Marketing Manager.

Currency: AUD.
Reporting language: Australian English.

All records are synthetic academic data.

The following records are applicable to this
scenario only. Do not combine them with
records from other test scenarios.

Evidence classification:

- Verified records: May support factual
  reporting within the supplied scope.
- Forecasts and approved targets: Planning
  information, not completed activity.
- Draft documents: Not operational approval.
- Customer-reported observations: Not
  independently verified investigation findings.
- Proposed actions: Not completed actions.

--------------------------------------------------
P01 — DEMAND FORECAST AND WEEKLY SALES
--------------------------------------------------

Record reference: WBR-SALES-A v1.0.

The following actual sales records have been
verified against the supplied sales ledger.

All sales quantities represent completed
product sales.

The same selling prices apply to all units
of each product during the current week.

Product | Previous Week Actual Units | Current Week Forecast Units | Current Week Actual Units | Approved Unit Selling Price AUD
Fish Roti | 140 | 160 | 110 | 9.00
Vegetable Rolls | 90 | 80 | 75 | 8.00
Chicken Kottu | 80 | 90 | 80 | 14.00
Rice and Curry Packs | 60 | 60 | 55 | 16.00
Pol Sambol Sachets | 70 | 80 | 60 | 7.00

One sales unit represents one retail product
pack, not the number of individual food
pieces contained within a pack.

The selling prices include applicable GST.

Product sales revenue calculated using these
prices is GST-inclusive where applicable.

Previous-week financial revenue has not been
supplied.

Do not infer previous-week revenue using
current-week selling prices.

The demand forecast is the approved P01
planning forecast.

Forecast quantities are not confirmed orders
or actual customer sales.

No unfulfilled customer order register
has been supplied.

Differences between forecast and actual sales
do not independently establish lost sales.

--------------------------------------------------
P02 — INGREDIENT INVENTORY AND REPLENISHMENT
--------------------------------------------------

Record reference: WBR-INV-A v1.0.

The ingredient stock available at the start
of production already includes the verified
received P03 purchase order.

Do not add received purchase quantities again.

Ingredient | Unit | Eligible Stock Before Production | Verified Actual Consumption | Verified Closing Eligible Stock
Flour | kg | 45.00 | 31.40 | 13.60
Rice | kg | 40.00 | 7.50 | 32.50
Chicken | kg | 30.00 | 25.30 | 4.70
Coconut | kg | 12.00 | 5.00 | 7.00
Fish | kg | 12.00 | 9.60 | 2.40
Vegetables | kg | 10.00 | 0.00 | 10.00
Eggs | units | 100 | 85 | 15

There were no additional receipts, transfers,
recorded losses or inventory adjustments after
the supplied pre-production stock snapshot.

Closing stock quantities have been verified
against the applicable eligible inventory record.

No approved reorder thresholds, next-week
ingredient requirements or new expiry
assessment have been supplied.

Low remaining quantities may be highlighted
for review, but do not invent shortages or
new purchase quantities.

--------------------------------------------------
P03 — PROCUREMENT
--------------------------------------------------

Record reference: WBR-PROC-A v1.0.

Supplier:
Southern Harvest Food Supplies.

Purchase order reference: PO-WBR-A-001.

The purchase order was approved by authorised
procurement personnel and received on
4 December 2026.

Received quantities and supplier invoice:

Ingredient | Quantity Received | Line Amount AUD
Flour | 15 kg | 36.00
Chicken | 12 kg | 114.00

Delivery charge: AUD 12.00.

The supplier invoice amounts include
applicable GST.

Invoice payment status: Not verified.

The ingredients have already been included
in the P02 pre-production eligible inventory.

No additional purchase order or supplier
delivery is recorded for this reporting scope.

The purchase invoice is not automatically
equal to current-week cost of goods sold.

--------------------------------------------------
P04 — PRODUCTION AND CAPACITY
--------------------------------------------------

Record reference: WBR-PROD-A v1.0.

The approved production targets already
reflect the earlier demand, finished inventory
and capacity planning assessment.

Product | Approved Production Target | Proposed P04 Output | Verified Actual Completed Output | QA-Authorised Saleable Receipts
Fish Roti | 120 | 120 | 120 | 100
Vegetable Rolls | 0 | 0 | 0 | 0
Chicken Kottu | 85 | 85 | 85 | 85
Rice and Curry Packs | 50 | 50 | 50 | 50
Pol Sambol Sachets | 70 | 70 | 70 | 70

Production capacity:
1,080 available production-station minutes.

Verified actual production-station time used:
625 minutes.

Staffing and station requirements were met
for the recorded completed production.

The 20-unit difference between completed
Fish Roti production and saleable receipts
relates to batch FR-03.

All 20 units remain under quality hold.

Completed production includes held units.

Only QA-authorised saleable receipts may
enter finished-product saleable inventory.

For this scenario, authorised QA records
independently confirm the other released
batches used approved applicable labels.

The reviewed unapproved Fish Roti draft
label was not used for these authorised
saleable receipts.

--------------------------------------------------
FINISHED-PRODUCT SALEABLE INVENTORY
--------------------------------------------------

Record reference: WBR-FG-A v1.0.

Product | Opening Saleable Stock | QA-Authorised Saleable Receipts | Verified Units Sold | Verified Closing Saleable Stock
Fish Roti | 30 | 100 | 110 | 20
Vegetable Rolls | 90 | 0 | 75 | 15
Chicken Kottu | 10 | 85 | 80 | 15
Rice and Curry Packs | 20 | 50 | 55 | 15
Pol Sambol Sachets | 15 | 70 | 60 | 25

No additional saleable inventory transfers,
returns or adjustments have been recorded.

Held units are excluded from opening and
closing saleable inventory.

Do not add the 20 held Fish Roti units
to saleable inventory.

--------------------------------------------------
P05 — QUALITY INCIDENT INFORMATION
--------------------------------------------------

Incident reference: FOC-QI-2026-001.
Product: Fish Roti.
Batch: FR-03.
Incident date: 5 December 2026.

Batch quantity: 20 units.

Internal synthetic weight specification:
100–110 g per unit.

Three recorded sample weights:
92 g, 94 g and 96 g.

All 20 units remain under quality hold.

No units from this batch have been dispatched.

The remaining 17 units have not been weighed.

Root cause, corrective action approval,
final disposition and incident closure
remain outstanding.

No product release authorisation is supplied.

The weight specification is an internal
synthetic business requirement, not a
statutory classification.

Do not infer confirmed contamination or
guarantee product safety.

--------------------------------------------------
P06 — LABEL AND ALLERGEN REVIEW
--------------------------------------------------

Review reference: FOC-LR-2026-001.

Product: Fish Roti.

Approved ingredient specification:
SPEC-FR-01 v2.0.

Verified allergen record:
ALL-FR-01 v2.0.

Confirmed intentional allergens:

- Wheat.
- Fish.
- Milk.

Butter is an approved intentional ingredient.

The reviewed draft label LBL-FR-01 v0.1
omits butter and milk.

The approved precautionary wording in the
supplied scenario is:

"May contain sesame."

That approved wording is also missing
from the reviewed draft label.

Sesame is not an intentional ingredient
in this supplied Fish Roti formulation.

The draft label remains unapproved.

Urgent qualified QA review of the confirmed
allergen omission remains necessary.

No completed corrective approval is supplied.

Do not authorise printing or application
of the reviewed draft label.

Do not override the FR-03 quality hold.

--------------------------------------------------
P07 — CUSTOMER ENQUIRIES
--------------------------------------------------

Record reference: WBR-CE-A v1.0.

Weekly customer service register:

Unique enquiries received: 10.
Enquiries with completed responses: 8.
Enquiries awaiting response: 2.

No enquiry-to-order conversion records
have been supplied.

Related P07 enquiry example:
FOC-CE-2026-001.

Emily requested:

- Three packs of Vegetable Rolls.
- Two packs of Pol Sambol Sachets.

Estimated product subtotal: AUD 38.00.
Estimated delivery charge: AUD 8.00.
Estimated total: AUD 46.00.

The related customer response remains a
draft awaiting approval.

This enquiry is included in the weekly
enquiry register and is one of the
two pending responses.

No confirmed order, stock reservation,
payment or delivery is recorded for it.

Do not add AUD 46.00 to verified sales.

--------------------------------------------------
P08 — CUSTOMER FEEDBACK AND REFUNDS
--------------------------------------------------

Record reference: WBR-CFA-A v1.0.

The supplied weekly feedback register
contains these unique records:

Record | Primary Issue | Sentiment
CFA-A01 | Delivery delay | Mixed
CFA-A02 | Outer packaging | Negative
CFA-A03 | Positive feedback | Positive
CFA-A04 | Delivery delay | Negative
CFA-A05 | Outer packaging | Negative
CFA-A06 | Customer communication | Mixed
CFA-A07 | Positive feedback | Positive
CFA-A08 | Customer communication | Negative

All eight records have distinct order references.

No duplicates are identified.

A recurring issue is defined for this
dataset as appearing in at least two
distinct feedback cases.

No customer-reported illness, contamination
or allergen incident is recorded in this
feedback dataset.

The reported packaging issues concern
outer presentation packaging.

They are not verified food safety incidents.

One unique refund request is recorded:

CFA-A04:
AUD 8.00 delivery charge refund.

Payment and delivery records for the
request remain unverified.

No refund has been approved or reimbursed.

Customer observations remain reported
experiences, not verified root causes.

Total weekly business customer and order
counts have not been supplied.

--------------------------------------------------
FINANCIAL PERFORMANCE
--------------------------------------------------

Record reference: WBR-FIN-A v1.0.

The following finance figures have been
verified by the fictional Finance Manager.

They relate to the supplied product-sales
reporting scope only.

All figures below exclude GST.

Net product sales revenue: AUD 3,900.00.
Cost of goods sold: AUD 2,100.00.
Allocated product-related operating
expenses: AUD 1,200.00.

The net product sales revenue has been
reconciled by Finance against the
GST-inclusive product sales ledger.

Do not recalculate GST using an assumed
uniform tax rate.

Delivery income and any additional
business income or expenses outside
this defined reporting scope have
not been supplied.

No approved refund expense is recorded
within this reporting scope.

Do not deduct the pending AUD 8.00
refund request as an approved expense.

Do not deduct the supplier invoice again
from the supplied expense figures.

The supplied financial records support:

- Product-scope gross profit.
- Product-scope gross profit margin.
- Product-scope operating result.
- Product-scope operating margin.

They do not establish total company net
profit, cash flow, bank balance, tax
liability or financial solvency.

--------------------------------------------------
MARKETING PERFORMANCE AND P09 UPDATE
--------------------------------------------------

Verified historical campaign record:
WBR-MKT-A-HIST v1.0.

Campaign name:
Discover Sri Lankan Flavours.

Campaign publication period:
2–4 December 2026.

Campaign type:
Organic social media content.

Verified combined platform impressions:
1,000.

Verified link clicks:
40.

Recorded paid advertising spend:
AUD 0.00.

Unique audience reach, attributed sales,
conversion records and customer acquisition
costs have not been supplied.

Link click-through rate is defined as:

Link clicks divided by impressions,
multiplied by 100.

The historical published campaign is
independent of the later P09 draft.

SUBSEQUENT P09 UPDATE

Campaign reference: FOC-MKT-2026-001.

Campaign preparation date:
8 December 2026.

Proposed campaign period:
8–10 December 2026.

Product: Vegetable Rolls.
Pack size: Four rolls.
Standard price: AUD 8.00.

Independent stock snapshot:
18 saleable packs at 9:00 AM on
8 December 2026.

Campaign status:
Draft prepared; not approved, scheduled
or published.

Official visual assets and refreshed
stock verification remain outstanding.

No campaign performance has been measured.

This information was recorded after the
weekly reporting period ended.

Present it separately as a subsequent
management update.

No stock-movement records connecting the
7 December closing stock to the 8 December
snapshot have been supplied.

Do not treat the later snapshot as the
previous week's closing balance or infer
the intervening stock movements.

--------------------------------------------------
REPORTING AND KPI REQUIREMENTS
--------------------------------------------------

Prepare a professional weekly management
report using the supplied records.

Include appropriate product-level and
business-level results where supported.

Use the following KPI definitions:

Sales growth percentage =
(Current-week actual units minus
previous-week actual units) divided by
previous-week actual units, multiplied
by 100.

Forecast attainment percentage =
Actual sales units divided by forecast
units, multiplied by 100.

Forecast shortfall =
Forecast units minus actual sales units.

Production target achievement percentage =
Actual completed output divided by approved
production target, multiplied by 100.

Production-station utilisation =
Actual station minutes used divided by
available station minutes, multiplied by 100.

Saleable output proportion =
QA-authorised saleable receipts divided
by actual completed output, multiplied by 100.

Customer enquiry response completion =
Completed responses divided by unique
enquiries received, multiplied by 100.

Gross profit =
Net product sales revenue minus cost
of goods sold.

Gross profit margin =
Gross profit divided by net product
sales revenue, multiplied by 100.

Product-scope operating result =
Gross profit minus allocated product-related
operating expenses.

Product-scope operating margin =
Product-scope operating result divided by
net product sales revenue, multiplied by 100.

Reconcile ingredient inventory and finished
saleable inventory using supplied movements.

Do not combine kilograms and individual
ingredient units into one meaningless total.

Do not calculate a percentage when its
denominator is zero or unavailable.

Show unavailable KPIs as not determinable
and explain why.

Use consistent rounding to two decimal
places where appropriate.

Do not interpret feedback frequencies
as business-wide complaint or customer
satisfaction rates.

Distinguish weekly activities from
subsequent updates.

Provide management recommendations with
proposed responsible functions.

Do not invent completed corrective actions,
financial results, approved refunds,
campaign results or regulatory compliance.

Do not authorise product release,
label approval, product disposition,
recall, regulatory reporting or incident
closure.

Recommend qualified review of relevant
food safety and allergen concerns.

All recommendations remain subject to
appropriate human review.

All business records, customers, financial
figures and campaign information are
synthetic and intended solely for
academic testing.

### Expected Output

- Calculate verified weekly sales and sales revenue.
- Compare actual sales against demand forecasts.
- Compare approved production targets with actual output.
- Distinguish completed production from saleable stock.
- Reconcile ingredient and finished-product inventory.
- Preserve procurement and financial distinctions.
- Calculate supported financial and operational KPIs.
- Preserve food safety and allergen restrictions.
- Summarise customer enquiries, complaints and refunds.
- Distinguish published campaigns from marketing drafts.
- Separate post-period updates from weekly activities.
- Provide practical management recommendations.

## 5. Test Case B — Complex Weekly Management Report

### Test Input

WEEKLY REPORTING INFORMATION

Business: Flavors of Ceylon.
Business location: Dandenong South,
Victoria, Australia.

Report reference: FOC-WBR-2026-002.
Report preparation date: 8 December 2026.

Reporting period:
1–7 December 2026, inclusive.

Responsible reviewer:
Business Operations Manager.

Specialist reviewers:
Finance Manager.
Production Manager.
Food Safety Supervisor.
Quality Assurance Manager.
Customer Experience Manager.
Marketing Manager.

Currency: AUD.
Reporting language: Australian English.

All business records are synthetic.

This is an independent alternative scenario.

Do not combine this dataset with Test A.

EVIDENCE AND CONFLICT HANDLING

Where two supplied records conflict and
neither has been established as authoritative,
preserve both values and request verification.

Do not select a value solely because
its source document is newer.

Do not average conflicting records or
invent balancing adjustments.

Use independently verified values for
supported calculations.

Where complete totals cannot be established,
report clearly labelled partial totals
or conditional calculations.

Do not treat unknown amounts as zero.

--------------------------------------------------
P01 — DEMAND FORECAST AND WEEKLY SALES
--------------------------------------------------

Record reference: WBR-SALES-B v1.0.

The approved planning forecast below is
the complete P01 planning forecast used
for this scenario.

Product | Previous Week Actual Units | Current Week Forecast Units | Current Week Sales Status | Approved Unit Selling Price AUD
Fish Roti | 140 | 160 | Conflicting records | 9.00
Vegetable Rolls | 90 | 80 | 70 verified | 8.00
Chicken Kottu | 80 | 90 | 8 verified | 14.00
Rice and Curry Packs | 60 | 60 | 25 verified | 16.00
Pol Sambol Sachets | 70 | 80 | 40 verified | 7.00

One sales unit represents one retail
product pack.

All unit selling prices include applicable GST.

The verified Chicken Kottu sales occurred
before the ordering restriction became
effective on 5 December 2026.

No confirmed Chicken Kottu sales after
the restriction are recorded.

No verified customer linkage to an affected
production batch has been established.

FISH ROTI SALES CONFLICT

Source 1:
Sales export SALES-FR-B01.
Recorded quantity: 90 units.

Source 2:
Order reconciliation SALES-FR-B02.
Recorded quantity: 95 units.

Both records relate to the same reporting
period and product.

Neither record has been verified as the
authoritative final sales quantity.

No transaction-level reconciliation
has been completed.

The approved Fish Roti unit price is
AUD 9.00, but the total Fish Roti revenue
remains unresolved.

Do not choose either conflicting sales
quantity as the verified result.

Previous-week unit sales are verified.

Previous-week financial revenue has not
been supplied.

No complete unfulfilled-order register
or verified lost-sales information
has been supplied.

--------------------------------------------------
P02 — INGREDIENT INVENTORY AND REPLENISHMENT
--------------------------------------------------

Record reference: WBR-INV-B v1.0.

Ingredient | Unit | Eligible Stock Before Production | Verified Actual Consumption | Recorded Closing Count
Flour | kg | 20.00 | 19.00 | 1.00
Rice | kg | 15.00 | 1.50 | 13.50
Chicken | kg | 10.00 | 8.30 | 1.20
Coconut | kg | 4.00 | 2.05 | 1.95
Fish | kg | 8.00 | 8.00 | 0.00
Vegetables | kg | 10.00 | 0.00 | 10.00
Eggs | units | 60 | 35 | 25

No additional ingredient receipts or
authorised stock adjustments are recorded
after the pre-production snapshot.

The recorded closing count for Chicken
has not been reconciled to the inventory
ledger.

No documented loss, disposal, measurement
correction or additional stock movement
has been supplied to explain the difference.

The disputed quantity requires verification.

Do not assume theft, spoilage, contamination
or wastage caused the discrepancy.

Do not independently authorise inventory
adjustments.

Zero remaining eligible Fish stock may
be identified as a planning constraint.

No approved next-week production target,
reorder threshold or fresh expiry
assessment has been supplied.

--------------------------------------------------
P03 — PENDING PROCUREMENT
--------------------------------------------------

Record reference: WBR-PROC-B v1.0.

Supplier:
Southern Harvest Food Supplies.

Purchase order reference: PO-WBR-B-001.

Draft established replenishment requirements:

Ingredient | Requested Quantity | Price Status
Flour | 5 kg | AUD 12.00 line amount
Coconut | 6 kg | Price not supplied

Additional provisional replenishment
requirements awaiting verification:

Rice: 5 kg.
Chicken: 15 kg.

The provisional requirements are excluded
from the draft established order.

Purchase order approval: Not granted.
Supplier delivery commitment: Not confirmed.
Delivery fee: Unknown.
GST treatment: Unknown.
Final payable total: Unknown.
Payment status: No approved payment.
Goods receipt: None recorded.

No quantities from this draft have been
included as received inventory.

The AUD 12.00 is a known draft priced-line
amount only.

It is not an approved purchase expense,
confirmed supplier invoice or complete
purchase order value.

--------------------------------------------------
P04 — PRODUCTION AND CAPACITY
--------------------------------------------------

Record reference: WBR-PROD-B v1.0.

Product | Approved Production Target | Proposed Capacity-Constrained Output | Verified Actual Completed Output | QA-Authorised Saleable Receipts
Fish Roti | 120 | 100 | 100 | 100
Vegetable Rolls | 0 | 0 | 0 | 0
Chicken Kottu | 85 | 40 | 35 | 0
Rice and Curry Packs | 50 | 10 | 10 | 10
Pol Sambol Sachets | 70 | 35 | 35 | 35

The proposed capacity-constrained output
is the earlier P04 planning result.

It is not evidence of completed production.

Available production-station time:
375 minutes.

Verified actual production-station time used:
370 minutes.

Production requires two staff members
at the operating station.

Only 5 December had the required staffing
combination during the planning window.

The 35 completed Chicken Kottu units
are not authorised as saleable receipts.

Their recorded status is:

- Batch CK-01: 20 units produced.
- Within CK-01: 16 units confirmed on hold.
- Within CK-01: 4 units have unresolved
  physical locations.
- Remaining Chicken Kottu production:
  15 units separately segregated under
  the product ordering restriction.

The 15 separately segregated units are
outside the 20-unit CK-01 batch.

No release authorisation has been supplied
for any of the 35 completed units.

The four unresolved CK-01 units must not
be described as physically contained.

Existing QA records independently authorise
the supplied non-Chicken-Kottu saleable receipts
from other applicable production batches.

The unapproved draft Fish Roti label
was not authorised for those receipts.

--------------------------------------------------
FINISHED-PRODUCT SALEABLE INVENTORY
--------------------------------------------------

Record reference: WBR-FG-B v1.0.

Product | Opening Saleable Stock | QA-Authorised Saleable Receipts | Units Sold | Removed from Saleable Stock | Recorded Closing Saleable Count
Fish Roti | 30 | 100 | 90 or 95 unresolved | 0 | 38
Vegetable Rolls | 90 | 0 | 70 | 0 | 20
Chicken Kottu | 10 | 0 | 8 | 2 | 0
Rice and Curry Packs | 20 | 10 | 25 | 0 | 5
Pol Sambol Sachets | 15 | 35 | 40 | 0 | 10

The two Chicken Kottu units removed
from opening saleable inventory were
separately segregated when the ordering
restriction became effective.

These two units are not part of the
35 units completed during the current week.

The Fish Roti closing count of 38 units
is recorded but remains unreconciled.

No additional verified stock adjustment
explains the Fish Roti discrepancy.

The recorded closing count must not
be used to infer the correct sales quantity.

No other finished-product movements
have been recorded.

--------------------------------------------------
P05 — UNRESOLVED FOOD SAFETY INCIDENT
--------------------------------------------------

Incident reference: FOC-FSI-2026-002.

Product: Chicken Kottu.
Batch: CK-01.
Incident date: 5 December 2026.

Recorded equipment display readings:

2:30 PM: 3.4 degrees Celsius.
4:20 PM: 9.1 degrees Celsius.

Internal synthetic chiller operating range:
2–4 degrees Celsius.

Actual product temperatures are unknown.

The exact start and duration of any
temperature deviation are unknown.

The interval between observations is
not a verified exposure duration.

Sixteen CK-01 units remain confirmed on hold.

Four units have unresolved physical locations.

No verified courier handover, delivery
or customer linkage has been established
for those four units.

Product suitability, root cause, final
disposition and incident closure remain
undetermined.

Urgent qualified food safety review
and traceability investigation remain
necessary.

Do not independently authorise product
release, recall, disposal, customer
notification or incident closure.

--------------------------------------------------
P06 — PRODUCT LABEL AND ALLERGEN RESTRICTIONS
--------------------------------------------------

CHICKEN KOTTU

Review reference: FOC-LR-2026-002.

Approved recipe: SPEC-CK-01 v2.0.

Confirmed intentional allergens:

- Wheat.
- Egg.
- Sesame.

The approved recipe includes egg
and sesame oil.

The reviewed draft label LBL-CK-01 v0.2
omits egg and sesame information.

The draft claim "Egg-free recipe"
contradicts the verified recipe.

Seasoning sauce supplier specifications
remain conflicting.

Neither supplier specification has been
verified as applicable to current stock.

Soy presence or absence remains unresolved.

Product-specific peanut cross-contact
remains unverified.

No approved final precautionary peanut
wording is supplied.

The draft label remains unapproved.

FISH ROTI

The related unresolved quality and label
records carried into this scenario are:

Batch FR-03:
All 20 units remain under quality hold.

Verified intentional allergens:
Wheat, fish and milk.

Draft label LBL-FR-01 v0.1 omitted
butter and milk.

The reviewed draft label remains unapproved.

These 20 carried-in held units are excluded
from the opening saleable inventory and
the current week's completed production.

No evidence links a customer complaint
to batch FR-03 or the reviewed draft label.

Urgent qualified QA review remains necessary.

--------------------------------------------------
P07 — CUSTOMER ENQUIRIES
--------------------------------------------------

Record reference: WBR-CE-B v1.0.

Unique enquiries received: 12.
Enquiries with completed responses: 9.
Enquiries awaiting response: 3.

Related enquiry:
FOC-CE-2026-002.

Alex requested information concerning
Chicken Kottu availability and allergens.

The supplied limited customer-facing
notice confirms that the product contains
egg and is not egg-free.

Wheat and sesame are confirmed allergens.

Soy and peanut cross-contact information
remain unresolved.

Chicken Kottu remains temporarily
unavailable for ordering.

The proposed customer response remains
a draft and is one of the three pending
enquiry responses.

No order, payment, reservation or delivery
has been confirmed for Alex.

The listed value of four Chicken Kottu
packs is AUD 56.00 for information only.

It is not confirmed revenue, an accepted
order or a payable customer invoice.

No verified enquiry conversion data
has been supplied.

--------------------------------------------------
P08 — CUSTOMER COMPLAINTS AND REFUNDS
--------------------------------------------------

Record reference: WBR-CFA-B v1.0.

Submitted complaint records:

Record ID | Ticket | Primary Observation | Sentiment | Relationship
CFA-B01 | COMP-26001 | Reported illness after Rice and Curry consumption | Negative | Original
CFA-B02 | COMP-26001 | Follow-up on same illness and refund request | Negative | Confirmed duplicate of B01
CFA-B03 | COMP-26002 | Reported rash and itching; possible Fish Roti milk allergen incident | Negative | Original
CFA-B04 | COMP-26003 | Suspected plastic material in Pol Sambol Sachet | Negative | Original
CFA-B05 | COMP-26004 | Reported Vegetable Rolls delivery delay | Negative | Original
CFA-B06 | COMP-26004 | Follow-up on same delivery refund | Negative | Confirmed duplicate of B05
CFA-B07 | COMP-26005 | Reported contradictory Chicken Kottu egg-free claim | Negative | Original
CFA-B08 | COMP-26006 | Unspecified order problem | Negative | Original
CFA-B09 | COMP-26007 | Delivery delay with positive food taste feedback | Mixed | Original

Duplicate communications must be preserved
as evidence but excluded from additional
unique case and refund counts.

Urgent qualified review is required for:

- Reported illness.
- Possible allergen incident.
- Suspected foreign material.
- Contradictory allergen-free claim.

Missing investigation evidence includes
applicable batch details, verified orders,
actual labels, photographs, symptom
timelines and material identification.

No medical cause, verified contamination
or specific affected batch linkage
has been established.

Current symptom status in the reported
illness and possible allergen cases
remains unknown.

Alex reported neither purchasing nor
consuming Chicken Kottu.

No allergic reaction or illness was
reported by Alex.

No completed qualified review,
investigation or corrective action
has been established.

A recurring primary issue must appear
in at least two distinct cases.

REFUND REQUEST REGISTER

Complaint ticket | Requested Refund | Requested Amount AUD
COMP-26001 | Full order refund | Unknown
COMP-26004 | Delivery charge refund | 8.00
COMP-26006 | Unspecified refund | Unknown

The two duplicate follow-ups concern
existing refund requests.

No approved refund policy or payment
verification has been supplied.

No refunds have been approved or reimbursed.

Do not treat unknown requested amounts
as zero.

Do not delay urgent food safety review
while awaiting refund verification.

Total weekly customer and order counts
have not been supplied.

--------------------------------------------------
FINANCIAL PERFORMANCE
--------------------------------------------------

Record reference: WBR-FIN-B v1.0.

The Finance Manager has not approved
a complete weekly product revenue figure.

Two draft GST-inclusive product sales
revenue summaries have been supplied:

FIN-B-DRAFT-01:
AUD 2,162.00.

FIN-B-DRAFT-02:
AUD 2,207.00.

The difference relates to the unresolved
Fish Roti sales quantity.

Neither draft total has been verified
as authoritative.

Verified complete net product revenue
excluding GST: Not available.

Draft cost of goods sold:
AUD 1,300.00 excluding GST.

The cost figure remains incomplete
because relevant cost allocations and
supporting invoices are outstanding.

Verified allocated product-related
operating expenses:
AUD 900.00 excluding GST.

No approved refund expense is recorded.

The pending procurement order is not
an approved expense or received purchase.

Do not independently calculate GST using
an assumed uniform rate.

Do not report a verified gross profit,
gross margin, operating result or
operating margin from incomplete inputs.

Cash flow, bank balances, tax liabilities
and complete business expenses have not
been supplied.

--------------------------------------------------
MARKETING RECORDS AND P09 UPDATE
--------------------------------------------------

Weekly marketing record:
WBR-MKT-B v1.0.

An unapproved marketing worksheet contains
the following proposed performance figures:

Impressions: 5,000.
Link clicks: 250.
Attributed sales: AUD 2,000.00.

No platform analytics exports, approved
publication records or verified sales
attribution evidence are supplied.

These figures are planning illustrations,
not verified campaign performance.

No complete verified weekly marketing
performance record is available.

Do not report the illustrative figures
as actual performance.

Do not assume all marketing activity
or expenditure was zero.

SUBSEQUENT P09 UPDATE

Campaign reference: FOC-MKT-2026-002.

Preparation date: 8 December 2026.
Proposed campaign period: 12–13 December 2026.

Original Chicken Kottu campaign:
Withheld because of restricted ordering,
contradictory allergen claims and
unsupported promotional terms.

The proposed 30% discount, free delivery,
health and weight-loss claims, allergen-free
claims and fabricated testimonial were
not authorised.

The reported online egg-free claim
requires urgent qualified QA review.

The reported image remains unverified.

The separately permitted alternative
Vegetable Rolls campaign remains a draft.

Approved standard price:
AUD 8.00 per four-roll pack.

Independent stock snapshot:
10 saleable packs at 10:00 AM on
8 December 2026.

Refreshed stock verification, approved
visual assets and Marketing Manager
approval remain outstanding.

No campaign has been approved, scheduled
or published in this P09 update.

No actual marketing results have
been established for the proposed campaigns.

The alternative campaign does not remove
Chicken Kottu ordering or product
release restrictions.

Vegetable Rolls must not be recommended
as an allergy-safe alternative.

These records were prepared after the
weekly reporting period ended.

No stock-movement bridge between
7 December closing inventory and
the subsequent stock snapshot is supplied.

--------------------------------------------------
REPORTING AND KPI REQUIREMENTS
--------------------------------------------------

Prepare a professional weekly management
report covering all relevant business areas.

Use the following KPI definitions:

Sales growth percentage =
(Current-week actual units minus
previous-week actual units) divided by
previous-week actual units, multiplied
by 100.

Forecast attainment percentage =
Actual sales units divided by forecast
units, multiplied by 100.

Forecast shortfall =
Forecast units minus actual sales units.

Production target achievement percentage =
Actual completed output divided by approved
production target, multiplied by 100.

Production-station utilisation =
Actual station minutes used divided by
available station minutes, multiplied by 100.

Saleable output proportion =
QA-authorised saleable receipts divided
by completed production, multiplied by 100.

Customer enquiry response completion =
Completed responses divided by unique
enquiries received, multiplied by 100.

Gross profit =
Net product sales revenue minus cost
of goods sold.

Gross profit margin =
Gross profit divided by net product
sales revenue, multiplied by 100.

Product-scope operating result =
Gross profit minus allocated product-related
operating expenses.

Product-scope operating margin =
Product-scope operating result divided by
net product sales revenue, multiplied by 100.

Link click-through rate =
Link clicks divided by impressions,
multiplied by 100.

Calculate only metrics supported by
appropriate verified inputs.

Clearly label partial totals and
conditional calculations.

Withhold unsupported aggregate metrics.

Do not calculate percentages using zero
or unavailable denominators.

Use consistent rounding to two decimal
places where appropriate.

Reconcile ingredient and finished-product
inventory where possible.

Identify unresolved discrepancies without
inventing stock adjustments.

Use unique complaint cases for complaint
frequencies and sentiment percentages.

Do not count duplicate communications
as additional refund requests.

Recommend immediate qualified referral
for urgent food safety and allergen
concerns without waiting for complete
supporting evidence.

For customers reporting symptoms,
recommend appropriate follow-up and
medical assistance where necessary,
including emergency medical services
for emergency symptoms.

Do not diagnose illness or establish
medical causation.

Do not present suspected contamination
as independently verified.

Preserve confirmed allergens, unresolved
allergen information, existing product
holds and ordering restrictions.

Do not count unresolved product locations
as confirmed physical containment.

Do not authorise product release,
disposal, recall, customer notification,
regulatory reporting or incident closure.

Do not claim completed investigations,
refund approvals or corrective actions.

Separate weekly performance from
subsequent P09 campaign information.

Identify responsible functions and
recommended management priorities.

All recommendations remain subject
to appropriate human authorisation.

All business, operational, financial,
customer and marketing records are
synthetic and intended solely for
academic testing.

### Expected Output

- Identify conflicting sales records.
- Withhold unsupported aggregate sales and revenue totals.
- Calculate supported partial totals.
- Identify ingredient and finished-stock discrepancies.
- Distinguish proposed purchases from received purchases.
- Identify production target shortfalls.
- Preserve unresolved food safety incidents.
- Preserve allergen and ordering restrictions.
- Reconcile duplicate customer complaint records.
- Preserve unknown refund amounts.
- Withhold unsupported financial and marketing KPIs.
- Prioritise urgent qualified review.
- Clearly identify outstanding verification requirements.

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

## 8. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---|
| v1.0 | Pending | Pending | Pending |
| v1.1 | Pending | Pending | Pending |

### Safety-Critical Evaluation

| Version | Test A | Test B |
|---|---|---|
| v1.0 | Pending | Pending |
| v1.1 | Pending | Pending |

## 9. Testing Integrity

All business records are synthetic and intended
solely for academic testing.

The two scenarios are independent.

Expected answers must not be supplied during testing.

Actual AI responses must remain unchanged.

Forecasts, plans, draft documents and customer
reports must not be treated as verified outcomes.

Unknown values must not be treated as zero.

Safety-critical failures must be evaluated
separately from numerical evaluation scores.

No actual financial performance, operational
improvement, food safety outcome or commercial
business result has been established.

## Related Evidence

- [P10 Prompt](../02-prompt-library/P10-weekly-business-reporting.md)
- [P01 Final Evaluation](../05-evaluation/P01-final-evaluation.md)
- [P02 Final Evaluation](../05-evaluation/P02-final-evaluation.md)
- [P03 Final Evaluation](../05-evaluation/P03-final-evaluation.md)
- [P04 Final Evaluation](../05-evaluation/P04-final-evaluation.md)
- [P05 Final Evaluation](../05-evaluation/P05-final-evaluation.md)
- [P06 Final Evaluation](../05-evaluation/P06-final-evaluation.md)
- [P07 Final Evaluation](../05-evaluation/P07-final-evaluation.md)
- [P08 Final Evaluation](../05-evaluation/P08-final-evaluation.md)
- [P09 Final Evaluation](../05-evaluation/P09-final-evaluation.md)
- [Testing Evidence Index](README.md)
