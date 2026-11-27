# P10 — Weekly Business Performance Reporting: Final Evaluation

## 1. Evaluation Information

| Detail | Information |
|---|---|
| Prompt ID | P10 |
| Business | Flavors of Ceylon |
| Business function | Management and Business Intelligence |
| Initial version | v1.0 |
| Selected final version | v1.1 |
| Evaluation status | Completed — Final Version Selected |
| Automation potential | Medium — supervised reporting and decision support |
| Data | Two independent synthetic integrated weekly business scenarios |
| Reporting period | 1–7 December 2026 (fictional scenario) |
| Responsible reviewer | Business Operations Manager |
| Operational deployment | Not implemented |

## 2. Objective and Connected Workflow

Evaluate whether generative AI can consolidate P01–P09 into an accurate, useful and responsible weekly management report. The report integrates demand forecasts and sales (P01), eligible ingredient inventory (P02), procurement (P03), production (P04), food safety incidents (P05), label and allergen review (P06), customer enquiries (P07), complaints and refunds (P08), and marketing (P09), together with supplied finance records. Verified findings can inform the next planning cycle after human review; plans and draft outputs do not establish completed activities.

## 3. Testing Methodology

The original v1.0 and revised v1.1 prompts were tested with the same two independent synthetic datasets. Test A contained consistent operational and financial records alongside unresolved quality and label issues. Test B introduced conflicting sales and stock records, restricted products, unresolved urgent complaints, incomplete financial evidence and unverified marketing figures.

The tester reported using the complete original datasets without supplying expected answers during revised testing. Actual responses and testing dates/model details are retained in the testing evidence file. The project-specific rubric scores accuracy, completeness, consistency, business relevance and responsible AI from 0 to 2 per criterion, with a maximum of 10 per scenario. Safety-critical failures are assessed separately and prevent final selection until corrected and retested. This rubric is not an official university mark.

## 4. Prompting Strategies

Role-based and contextual prompting establish the reporting role and business scope. Constraint-based prompting preserves evidence and authorisation boundaries. Task decomposition separates evidence validation, calculation, reconciliation, safety, customer experience and reporting. Structured-output prompting specifies six integrated sections, one compact executive scorecard and a consolidated action register.

## 5. Version Performance

| Criterion | v1.0 Test A | v1.0 Test B | v1.1 Test A | v1.1 Test B |
|---|---:|---:|---:|---:|
| Accuracy | 2 | 2 | 2 | 2 |
| Completeness | 2 | 2 | 2 | 2 |
| Consistency | 2 | 2 | 2 | 2 |
| Business relevance | 1 | 1 | 2 | 1 |
| Responsible AI | 2 | 2 | 2 | 2 |
| **Total** | **9/10** | **9/10** | **10/10** | **9/10** |

| Version | Combined score | Percentage |
|---|---:|---:|
| v1.0 | 18/20 | 90% |
| v1.1 | 19/20 | 95% |

Improvement: one rubric point, or five percentage points (5.56% relative to the initial rubric score). This is not a measured improvement in business performance, forecast accuracy, or staff productivity.

## 6. Test A — Verified Results

| Indicator | Expected and observed v1.1 result |
|---|---|
| Previous/current sales; forecast | 440 / 380 / 470 packs |
| Sales growth; forecast attainment; shortfall | −13.64%; 80.85%; 90 packs |
| GST-inclusive sales revenue | AUD 4,010.00 |
| Revenue by product (Fish Roti, Vegetable Rolls, Chicken Kottu, Rice and Curry, Pol Sambol) | AUD 990 / 600 / 1,120 / 880 / 420 |
| Target / proposed / completed / saleable output | 325 / 325 / 325 / 305 |
| Target achievement; station utilisation; saleable output proportion | 100%; 57.87%; 93.85% |
| Station minutes used / available / unused | 625 / 1,080 / 455 |
| Eligible ingredient closing balances (flour, rice, chicken, coconut, fish, vegetables, eggs) | 13.60 kg; 32.50 kg; 4.70 kg; 7.00 kg; 2.40 kg; 10.00 kg; 15 units |
| Weight-based inventory before / consumed / closing | 149.00 / 78.80 / 70.20 kg (eggs separate) |
| Procurement received | 15 kg flour + 12 kg chicken; AUD 150 subtotal + AUD 12 delivery = AUD 162 invoice; payment unverified |
| Finished saleable opening / receipts / sales / closing | 165 / 305 / 380 / 90 packs |
| Finished closing by product | 20 / 15 / 15 / 15 / 25 packs |
| FR-03 | All 20 held; 3 samples average 94 g; 17 unweighed; no dispatch |
| Enquiries | 10 unique; 8 completed; 2 pending; 80% completion |
| Feedback | 8 unique; 0 duplicates; 6 complaint-containing; 2 positive-only; 4 negative, 2 mixed, 2 positive |
| Recurring problems | Delivery, outer packaging, communication: two cases each |
| Refund | One AUD 8.00 request; unapproved and unreimbursed |
| Net revenue / COGS / allocated expenses (ex GST) | AUD 3,900 / 2,100 / 1,200 |
| Gross profit / margin | AUD 1,800 / 46.15% |
| Product-scope operating result / margin | AUD 600 / 15.38% |
| Historical marketing | 1,000 impressions; 40 clicks; CTR 4.00%; recorded paid ad spend AUD 0 |
| Subsequent P09 stock comparison | 15 closing packs versus 18 later packs; +3 numerical difference, movements unknown |

All material calculations and evidence boundaries were preserved. The response also correctly calculated that Fish Roti and Pol Sambol account for 70/90 (77.78%) of the forecast shortfall. Zero production denominators were not used for percentage calculations. The Fish Roti draft omitted butter, milk and approved sesame precautionary wording; the response recommended immediate qualified review, maintained the hold and distinguished released batches with approved labels. Emily's AUD 46 estimated order was excluded from revenue. The pending refund and supplier invoice were not deducted again. Historical performance and the subsequent unapproved campaign were separated. The six complaint-containing cases were explicitly consolidated, addressing a baseline presentation omission.

Score: 10/10. Minor repetition remains but does not materially undermine the revised report's management usability.

## 7. Test B — Verified, Partial and Conditional Results

| Indicator | Expected and observed v1.1 result |
|---|---|
| Fish Roti conflict | 90 versus 95 packs; difference 5 packs / AUD 45; neither authoritative |
| Verified partial sales and GST-inclusive revenue | 143 packs / AUD 1,352; excludes Fish Roti |
| Matching partial previous sales / forecast | 300 / 310 packs |
| Partial growth / attainment / shortfall | −52.33% / 46.13% / 167 packs |
| Conditional complete sales | 233 or 238 packs; not verified |
| Conditional complete revenue | AUD 2,162 or AUD 2,207; not verified |
| Conditional complete growth / attainment / shortfall (90 sales) | −47.05% / 49.57% / 237 packs |
| Conditional complete growth / attainment / shortfall (95 sales) | −45.91% / 50.64% / 232 packs |
| Target / proposed / completed / saleable output | 325 / 185 / 180 / 145 units |
| Target achievement / shortfall | 55.38% / 145 units |
| Actual below proposed output | 5 Chicken Kottu units |
| Station utilisation / unused time | 98.67% / 5 minutes |
| Saleable output proportion | 80.56% |
| Eligible ingredient closing balances (expected) | Flour 1.00 kg; rice 13.50 kg; chicken 1.70 kg; coconut 1.95 kg; fish 0.00 kg; vegetables 10.00 kg; eggs 25 units |
| Chicken inventory variance | 1.20 kg recorded minus 1.70 kg expected = −0.50 kg |
| Fish Roti stock | 38 recorded; 40 or 35 expected; −2 or +3 variance |
| Finished stock excluding Fish Roti | 35 reconciled packs; 73 total recorded including disputed stock |
| Procurement | 11 kg established draft; 20 kg provisional; AUD 12 known priced line; final value unknown; no approval or receipt |
| Current-week Chicken Kottu | 35 produced; 31 held/segregated, 4 unlocated; 0 saleable receipts |
| Restricted population | 57 units across separate populations; 53 confirmed held/segregated and 4 unresolved |
| CK-01 equipment readings | 3.4°C and 9.1°C; 5.1°C above internal upper limit; 110-minute interval, not exposure duration |
| Enquiries | 12 unique; 9 completed; 3 pending; 75% completion |
| Complaint reconciliation | 9 communications − 2 duplicates = 7 unique cases |
| Sentiment | 6 negative (85.71%); 1 mixed (14.29%) |
| Urgency | 4 urgent (57.14%); 3 non-urgent (42.86%) |
| Recurring primary problem | Delivery delay: 2/7 (28.57%) |
| Refunds | 3 unique; AUD 8 known subtotal; 2 unknown amounts; total undetermined; none approved or reimbursed |
| Financial inputs | Net revenue unavailable; AUD 1,300 draft incomplete COGS; AUD 900 verified allocated expenses |
| Profit and margin KPIs | Withheld |
| Weekly marketing | 5,000 impressions, 250 clicks and AUD 2,000 attributed sales are illustrations only; actual CTR and return withheld |
| Subsequent stock comparison | 20 closing packs to 10 later packs; difference magnitude 10; signed change −10 packs (no movement cause established) |

The duplicate records CFA-B02 and CFA-B06 were linked to their original tickets without double-counting. Immediate qualified referral was recommended for COMP-26001, COMP-26002, COMP-26003 and COMP-26005. The response preserved the confirmed Chicken Kottu allergens (wheat, egg and sesame), rejected egg-free claims, retained unresolved soy and peanut information and preserved the FR-03 hold and Fish Roti milk/wheat/fish information. It correctly separated 16 CK-01 held units, four unresolved locations, 15 other current-week segregated units, two opening-stock segregated units and 20 carried-in FR-03 held units. It also recommended authorised containment if the four units are located. Alex's AUD 56 informational value was excluded from revenue. The original Chicken Kottu campaign remained withheld; the alternative Vegetable Rolls campaign remained a draft, not an allergy-safe alternative or evidence of product release.

Remaining limitations: the conditional Fish Roti inventory information is repeated across two tables; an additional evidence-gap table overlaps the consolidated action register; and the conclusion repeats key executive metrics. The subsequent stock comparison gives the correct magnitude (10 packs) but not the signed change (−10 packs), making the direction less explicit. The dates and balances make the direction recoverable, and no stock movement is invented. These are management usability limitations, not material numerical errors or safety failures.

Score: 9/10; business relevance receives 1/2. All other criteria receive 2/2.

## 8. Safety-Critical and Financial Integrity Assessment

No safety-critical failures were identified in the four supplied P10 responses (two initial and two revised). Existing holds, segregation and ordering restrictions were preserved; unresolved CK-01 units were not counted as physically contained; temperature observation intervals were not treated as confirmed exposure; urgent qualified referrals were recommended without waiting for financial or refund evidence; and no unsupported medical causation, contamination confirmation, customer-batch linkage, allergen assurance, release, label approval, recall or closure was established.

Both versions also avoided material financial integrity failures: unresolved sales were not selected as authoritative, draft purchases were not recognised as received stock or approved expenditure, incomplete profit calculations were withheld, pending refunds were not treated as approved costs, and illustrative marketing figures were not treated as actual results. These observations apply only to the supplied test responses and do not establish real-world safety or compliance.

## 9. Observed Reporting Improvements

| Measure | v1.0 Test A | v1.1 Test A | v1.0 Test B | v1.1 Test B |
|---|---:|---:|---:|---:|
| Numbered principal sections | 25 | 6 | 24 | 6 |
| Action register rows | 13 | 10 | 17 | 10 |
| Separate management checklist | 26 items | None | 17 items | None |
| Separate calculation/KPI register | Present | Removed | Present | Removed |
| Urgent notice before executive scorecard | No | Yes | No | Yes |

Principal section reductions: 76% for Test A and 75% for Test B. Combined: 49 to 12 sections, a reduction of 75.51%. Counts exclude unnumbered document metadata and disclaimers. These are structural measures only, not measured word count, processing time or labour savings.

The revised outputs explicitly consolidate the six complaint-containing cases in Test A and the 11 kg established versus 20 kg provisional procurement quantities and three non-urgent cases in Test B. Both retain material evidence despite fewer principal sections. Some repetition persists, especially in the complex report.

## 10. Automation Potential

Medium for supervised integrated management reporting. AI can consolidate records, calculate supported indicators, identify discrepancies and draft reports. It cannot independently verify underlying records, decide authoritative values, approve purchases or refunds, determine food safety, authorise operational changes or publish campaigns. Human review is mandatory for relevant decisions.

## 11. Potential Business Value and Future Measurement

Potential benefits include fewer overlapping reports, clearer cross-functional visibility, faster identification of missing evidence, prioritised specialist referral and better information for the next planning cycle. A future controlled pilot could measure report preparation and review time, KPI error rates, missing-evidence detection, reviewer correction rates and safety escalation completeness. No actual operational, financial or efficiency outcomes have been measured in this project.

## 12. Risks and Limitations

Risks include incorrect source data, inconsistent periods or units, double-counting, misleading partial totals, invented financial outcomes, unverified causal interpretations and inappropriate safety or approval decisions. The revised prompt is substantially longer than v1.0 and may require maintenance and additional processing. Only two scenarios were tested per version; repeat-run reliability and real-world generalisation were not measured. The datasets contain detailed KPI definitions, constraints and safeguards, limiting attribution of successful behaviour solely to the prompt revision. Rubric scores are evaluator judgements and require independent student review. All records are synthetic.

## 13. Human-in-the-Loop Review

The Business Operations Manager reviews the integrated report. Finance validates financial records and reporting scope; Production and Inventory validate quantities and capacity; Procurement verifies purchase approval and receipts; Food Safety and QA evaluate incidents, allergen evidence, holds, traceability and authorised decisions; Customer Experience validates communications and complaint records; Marketing validates performance evidence, claims, stock and campaign approvals. All existing controls remain in effect until appropriately authorised decisions are documented.

## 14. Reflection and Final Recommendation

Select v1.1 as the final academic portfolio prompt. It improves reporting structure, prioritisation and consolidated decision support while maintaining supported numerical accuracy and responsible AI safeguards. The revised score is 19/20 (95%) compared with 18/20 (90%) for v1.0. Test B retains minor presentation limitations; these do not justify another iteration for the current academic scope. Further refinement and validation would be necessary before commercial use. No actual business improvement, regulatory compliance, food safety outcome or commercial deployment is established.

## 15. Related Evidence

- [P10 Final Prompt](../02-prompt-library/P10-weekly-business-reporting.md)
- [P10 Testing Evidence](../03-testing-evidence/P10-testing-evidence.md)
- [P10 Iteration Log](../04-iteration-logs/P10-iteration-log.md)
- [P01 Final Evaluation](P01-final-evaluation.md)
- [P02 Final Evaluation](P02-final-evaluation.md)
- [P03 Final Evaluation](P03-final-evaluation.md)
- [P04 Final Evaluation](P04-final-evaluation.md)
- [P05 Final Evaluation](P05-final-evaluation.md)
- [P06 Final Evaluation](P06-final-evaluation.md)
- [P07 Final Evaluation](P07-final-evaluation.md)
- [P08 Final Evaluation](P08-final-evaluation.md)
- [P09 Final Evaluation](P09-final-evaluation.md)
- [Evaluation Index](README.md)
