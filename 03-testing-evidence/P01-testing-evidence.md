# P01 — Product Demand Forecasting: Testing Evidence

## 1. Testing Information

| Detail | Information |
|---|---|
| Prompt ID | P01 |
| Business | Flavors of Ceylon |
| Business Function | Demand Planning |
| AI Tool | To be recorded during testing |
| AI Model | To be recorded if available |
| Data Type | Synthetic business data |
| Testing Status | Completed — v1.2 Selected |

## 2. Testing Objective

Evaluate whether the AI prompt can analyse historical
food product sales, identify demand patterns and
produce useful demand estimates for production planning.

Testing also evaluates the handling of missing data,
stock shortages, uncertainty and unsupported assumptions.

---

## 3. Test Case A — Standard Scenario

The production manager requires Week 5 demand
estimates based on historical weekly sales.

### Test Input

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | 120 | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 80 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | 50 | 60 | 70 |

All figures represent units sold.

No stock shortages or unusual promotional events
are reported for this scenario.

### Expected Output

- Identify increasing sales patterns.
- Identify decreasing sales patterns.
- Identify stable sales patterns.
- Provide reasonable Week 5 demand estimates.
- Explain the forecasting method or assumptions.
- Present clear production recommendations.
- Avoid unsupported business information.

---

## 4. Test Case B — Challenging Scenario

The production manager requires Week 5 demand
estimates, but some sales records are incomplete.

### Test Input

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | Missing | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 25 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | Missing | 60 | Missing |

Additional information:

- Fish roti Week 3 sales are unavailable due to a
  reporting system error.
- Chicken kottu was out of stock for four days
  during Week 4.
- Some pol sambol sales records are unavailable.
- No promotional campaign information is supplied.

### Expected Output

- Identify all missing sales records.
- Do not interpret missing values as zero.
- Recognise that stock shortages can reduce
  recorded sales independently of customer demand.
- Avoid inventing missing sales information.
- Communicate forecasting uncertainty.
- Recommend appropriate human review.

---

## 5. Version v1.0 — Initial Prompt Testing

### Testing Date and AI Model

25 November 2026 | ChatGPT

### Test Case A — Actual AI Output


# Flavors of Ceylon – Week 5 Demand Forecast

## 1. Demand Analysis and Production Recommendations

Based on the supplied historical sales data, the linear trend forecasting method has been selected to estimate Week 5 demand by calculating the average weekly change in units sold.

### Historical Sales Data

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | 120 | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 80 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | 50 | 60 | 70 |
| **Total** | **350** | **380** | **410** | **440** |

### Week 5 Demand Forecast

| Product | Week 4 Sales | Weekly Change | Demand Trend | Week 5 Forecast | Recommended Production |
|---|---:|---:|---|---:|---:|
| Fish roti | 140 | +20 | Increasing ↑ | 160 | 160 |
| Vegetable rolls | 90 | -10 | Decreasing ↓ | 80 | 80 |
| Chicken kottu | 80 | +10 | Increasing ↑ | 90 | 90 |
| Rice and curry packs | 60 | 0 | Stable → | 60 | 60 |
| Pol sambol sachets | 70 | +10 | Increasing ↑ | 80 | 80 |
| **Total** | **440** | **+30** | **Increasing** | **470** | **470** |

## 2. Product Demand Trends

- **Total Week 5 forecast:** 470 units
- **Week 4 sales:** 440 units
- **Expected increase:** 30 units
- **Percentage growth:** 6.82%
- **Products with increasing demand:** 3
- **Products with decreasing demand:** 1
- **Products with stable demand:** 1

### Demand Trend Summary

| Product | Week 1 | Week 2 | Week 3 | Week 4 | Week 5 (Forecast) |
|---|---:|---:|---:|---:|---:|
| Fish roti | 80 | 100 | 120 | 140 | **160** |
| Vegetable rolls | 120 | 110 | 100 | 90 | **80** |
| Chicken kottu | 50 | 60 | 70 | 80 | **90** |
| Rice and curry packs | 60 | 60 | 60 | 60 | **60** |
| Pol sambol sachets | 40 | 50 | 60 | 70 | **80** |

## 3. Reasons for Production Recommendations

| Product | Reason for Recommendation |
|---|---|
| Fish roti | Demand consistently increases by 20 units each week. Increase production to satisfy growing demand. |
| Vegetable rolls | Sales decrease by 10 units each week. Reduce production to minimise excess inventory and food waste. |
| Chicken kottu | Consistent growth of 10 units per week supports increased production. |
| Rice and curry packs | Demand remains unchanged throughout the four weeks. Maintain the existing production quantity. |
| Pol sambol sachets | Sales increase by 10 units each week, indicating a positive demand trend. |

## 4. Forecasting Method

The linear trend forecasting method is used to calculate the estimated demand for Week 5.

**Formula:**

Average weekly change = (Week 4 sales - Week 1 sales) / 3

Week 5 forecast = Week 4 sales + Average weekly change

**Example: Fish roti**

- Average weekly change = (140 - 80) / 3
- Average weekly change = 20 units
- Week 5 forecast = 140 + 20
- **Estimated demand = 160 units**

## 5. Assumptions and Limitations

- Historical sales accurately represent customer demand because no stock shortages were reported.
- Existing demand trends are assumed to continue during Week 5.
- No unusual promotional activities, price changes or external market disruptions are assumed to occur during Week 5.
- No opening inventory or safety stock requirements have been provided. Therefore, recommended production quantities equal forecast demand.
- Four weeks of historical data may not be sufficient to identify seasonality or long-term changes in customer preferences.
- Actual customer demand may differ from the forecast.
- Human review is required before finalising production decisions.

## 6. Final Recommendation

Flavors of Ceylon should plan to produce **470 units for Week 5**, representing a **6.82% increase** compared to Week 4 sales.

The production manager should prioritise fish roti, chicken kottu and pol sambol sachets while reducing vegetable roll production to minimise food waste.

The forecast should be reviewed against actual sales and available inventory before finalising production schedules.

All estimates are based exclusively on the supplied business data.

---

**End of AI-generated output**

### Test Case B — Actual AI Output


# Flavors of Ceylon – P01 v1.0 – Test B

## Test Scenario: Incomplete Sales Data and Stock Shortages

### 1. Demand Analysis and Production Recommendations

The historical sales data has been analysed using a linear trend forecasting approach. Missing sales records and stock shortages have been considered to avoid inaccurate demand estimates and inappropriate production decisions.

| Product | Week 1 | Week 2 | Week 3 | Week 4 | Week 5 Forecast | Demand Trend | Recommended Production | Confidence |
|---|---:|---:|---:|---:|---:|---|---:|---|
| Fish roti | 80 | 100 | Missing | 140 | 160 | Increasing | 160 | Medium |
| Vegetable rolls | 120 | 110 | 100 | 90 | 80 | Decreasing | 80 | High |
| Chicken kottu | 50 | 60 | 70 | 25 | 90 | Likely increasing | 90 | Medium |
| Rice and curry packs | 60 | 60 | 60 | 60 | 60 | Stable | 60 | High |
| Pol sambol sachets | 40 | Missing | 60 | Missing | 80 | Potentially increasing | 80 | Low |
| **Total** | — | — | — | — | **470** | — | **470** | — |

*All quantities are expressed in units. Confidence ratings are qualitative assessments based on data completeness and consistency.*

---

### 2. Week 5 Demand Forecast

**Total estimated demand: 470 units**

| Product | Forecast | Visual Representation |
|---|---:|---|
| Fish roti | 160 | ████████████████ |
| Vegetable rolls | 80 | ████████ |
| Chicken kottu | 90 | █████████ |
| Rice and curry packs | 60 | ██████ |
| Pol sambol sachets | 80 | ████████ |

*Each block represents 10 units.*

---

### 3. Reasons Behind Production Recommendations

| Product | Reason for Recommendation |
|---|---|
| Fish roti | Available sales indicate an increase of 20 units per week. Week 3 is estimated at 120 units, supporting a Week 5 forecast of 160 units. |
| Vegetable rolls | Sales consistently decline by 10 units each week. Reducing production to 80 units could minimise excess inventory and food waste. |
| Chicken kottu | Week 4 sales were affected by a four-day stock shortage rather than necessarily a decline in demand. The previous growth trend of 10 units per week supports a forecast of 90 units. |
| Rice and curry packs | Sales remain consistent at 60 units every week. Maintaining the existing production quantity is appropriate. |
| Pol sambol sachets | Available records suggest an average increase of 10 units per week. However, missing records reduce forecast reliability. The estimated 80 units should be treated as provisional. |

---

### 4. Assumptions and Limitations

- Missing sales records are treated as unavailable data, not zero sales.
- Historical demand trends are assumed to continue into Week 5.
- Chicken kottu is assumed to be available throughout Week 5.
- No promotional impact is included because promotional information is unavailable.
- Production recommendations assume no opening inventory and sufficient production capacity.
- Only four weeks of historical data are available, limiting forecast reliability.
- Confidence ratings are qualitative rather than statistically validated.

---

### 5. Final Recommendation

Flavors of Ceylon should provisionally plan to produce **470 units for Week 5**, prioritising fish roti and chicken kottu while reducing vegetable roll production to minimise food waste.

The production manager should verify missing sales records, monitor product availability and review actual customer demand before approving final production quantities.

Particular attention should be given to pol sambol sachets due to incomplete sales records.

**Human oversight is essential**, as AI-generated demand forecasts are estimates rather than guaranteed sales outcomes.

### Observed Strengths

- Correctly identified increasing, decreasing and
  stable product sales trends.
- Accurately calculated the Test Case A forecasts,
  with a total estimated demand of 470 units.
- Correctly calculated the 6.82% estimated increase
  compared with Week 4 sales.
- Selected and explained a linear trend forecasting
  approach.
- Recognised missing sales records in Test Case B
  without treating them as zero.
- Identified the impact of the chicken kottu stockout
  on recorded sales.
- Acknowledged forecasting assumptions, data
  limitations and human review requirements.

### Observed Weaknesses

- Production quantities were equated with forecast
  demand without verified finished-product inventory,
  safety stock or production capacity information.
- A missing fish roti sales record was estimated.
  Although labelled as an estimate, it was not
  independently verified.
- Pol sambol demand was estimated using only two
  available historical observations.
- Forecast calculation steps were not consistently
  provided for every product.
- Qualitative confidence ratings were not supported
  by standardised classification rules.
- Test Case B provided a combined production
  recommendation of 470 units despite differences
  in individual forecast reliability.

### Initial Evaluation Results

| Criterion | Test Case A | Test Case B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 1 |
| Business Relevance | 1 | 1 |
| Responsible AI | 2 | 1 |
| Total | 9/10 | 7/10 |

Combined evaluation score: 16/20 (80%).

### Initial Evaluation Conclusion

The v1.0 prompt demonstrated strong performance
when analysing simple historical sales patterns.

However, the challenging scenario revealed
opportunities to improve missing-data handling,
forecast calculation transparency, data reliability
classification and production decision support.

Although both scenarios produced an estimated
demand of 470 units, the second scenario contained
greater uncertainty.

The next prompt version will introduce explicit
data validation rules, a standard forecasting
method, minimum data requirements and clearer
separation between demand forecasts and production
recommendations.

These evaluation scores measure the quality of
the AI responses against the project criteria.
They do not measure actual future sales accuracy.

---

## 6. Version v1.1 — Revised Prompt Testing

### Testing Date and AI Model

25 November 2026

### Test Case A — Actual AI Output


# Flavors of Ceylon
## P01 – Demand Forecasting and Production Planning
### Version 2.0 – Test A Output

---

## 1. Test Scenario

The production manager requires Week 5 demand estimates based on complete historical weekly sales data.

### Historical Sales Data

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | 120 | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 80 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | 50 | 60 | 70 |

All figures represent units sold.

No stock shortages or unusual promotional events are reported for this scenario.

---

## 2. Data Validation

| Data validation criteria | Findings |
|---|---|
| Total products analysed | 5 |
| Historical sales records | 20 |
| Valid sales records | 20 |
| Missing records | None |
| Invalid or inconsistent records | None identified |
| Stockout-affected records | None reported |
| Unusual promotional events | None reported |
| Records excluded | None |

All historical observations are suitable for baseline demand trend calculations.

Recorded sales represent actual units sold, while Week 5 forecasts represent estimated future demand.

---

## 3. Week 5 Demand Forecast

| Product name | Usable observations | Missing or excluded records | Average weekly change | Sales trend | Week 5 forecast (units) | Data reliability | Recommended planning action |
|---|---:|---|---:|---|---:|---|---|
| Fish roti | 4 | None | +20 | Increasing | 160 | High | Prepare for higher demand |
| Vegetable rolls | 4 | None | -10 | Decreasing | 80 | High | Review potential overproduction |
| Chicken kottu | 4 | None | +10 | Increasing | 90 | High | Prepare for higher demand |
| Rice and curry packs | 4 | None | 0 | Stable | 60 | High | Maintain current demand planning baseline |
| Pol sambol sachets | 4 | None | +10 | Increasing | 80 | High | Prepare for higher demand |
| **Total estimated demand** | **20** | **None** | **+30** | **Increasing** | **470** | N/A | **Review production requirements** |

---

## 4. Forecast Calculation Breakdown

### Forecasting Method

The simple linear trend extrapolation method is applied to estimate Week 5 demand.

**Formula 1 – Average Weekly Change**

```text
Average weekly change =
(Latest usable sales - Earliest usable sales)
/ Number of elapsed weeks
```

**Formula 2 – Target-Week Forecast**

```text
Forecast demand =
Latest usable sales + (Average weekly change x Number of weeks to target week)
```

### Product Calculations

#### Fish Roti

- Average weekly change = (140 - 80) / 3
- Average weekly change = 20 units
- Week 5 forecast = 140 + (20 x 1)
- **Estimated demand = 160 units**

#### Vegetable Rolls

- Average weekly change = (90 - 120) / 3
- Average weekly change = -10 units
- Week 5 forecast = 90 + (-10 x 1)
- **Estimated demand = 80 units**

#### Chicken Kottu

- Average weekly change = (80 - 50) / 3
- Average weekly change = 10 units
- Week 5 forecast = 80 + (10 x 1)
- **Estimated demand = 90 units**

#### Rice and Curry Packs

- Average weekly change = (60 - 60) / 3
- Average weekly change = 0 units
- Week 5 forecast = 60 + (0 x 1)
- **Estimated demand = 60 units**

#### Pol Sambol Sachets

- Average weekly change = (70 - 40) / 3
- Average weekly change = 10 units
- Week 5 forecast = 70 + (10 x 1)
- **Estimated demand = 80 units**

### Total Estimated Demand

```text
160 + 80 + 90 + 60 + 80 = 470 units
```

**Total estimated Week 5 demand: 470 units.**

All products have sufficient usable observations. No rounding adjustments, negative forecast corrections or forecast exclusions are required.

---

## 5. Sales Trend Analysis

| Product | Week 1 | Week 2 | Week 3 | Week 4 | Week 5 (Estimated) |
|---|---:|---:|---:|---:|---:|
| Fish roti | 80 | 100 | 120 | 140 | 160 |
| Vegetable rolls | 120 | 110 | 100 | 90 | 80 |
| Chicken kottu | 50 | 60 | 70 | 80 | 90 |
| Rice and curry packs | 60 | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | 50 | 60 | 70 | 80 |
| **Total** | **350** | **380** | **410** | **440** | **470** |

### Overall Demand Growth

| Performance indicator | Result |
|---|---:|
| Week 4 recorded sales | 440 units |
| Week 5 estimated demand | 470 units |
| Estimated increase | 30 units |
| Estimated percentage increase | 6.82% |

### Trend Classification

| Sales trend | Products | Number of products |
|---|---|---:|
| Increasing | Fish roti, Chicken kottu, Pol sambol sachets | 3 |
| Decreasing | Vegetable rolls | 1 |
| Stable | Rice and curry packs | 1 |
| Undetermined | None | 0 |

Fish roti demonstrates the strongest positive sales trend, increasing by 20 units per week.

Vegetable rolls demonstrate a consistent decline, indicating a potential risk of excess inventory and food waste if production is not adjusted appropriately.

Chicken kottu and pol sambol sachets demonstrate consistent growth, while rice and curry packs maintain stable sales.

---

## 6. Data Reliability Assessment

| Product | Usable observations | Reliability level | Reason |
|---|---:|---|---|
| Fish roti | 4 | High | Complete historical records |
| Vegetable rolls | 4 | High | Complete historical records |
| Chicken kottu | 4 | High | Complete historical records |
| Rice and curry packs | 4 | High | Complete historical records |
| Pol sambol sachets | 4 | High | Complete historical records |

All five products are classified as having **High data reliability** because each product has four usable historical observations, with no missing or reported stockout-affected records.

No irregular sales patterns have been identified within the supplied historical period.

High data reliability describes the completeness and quality of the supplied information. It does not represent statistical forecast confidence or guarantee forecasting accuracy.

---

## 7. Production Planning Recommendations

### Production Requirement Formula

```text
Production requirement =
Forecast demand + Target safety stock
- Usable finished-product inventory
```

Negative production requirements must be adjusted to zero.

However, the supplied business information does not include finished-product inventory, target safety stock or production capacity.

Therefore, actual production quantities cannot be determined.

| Product | Forecast demand | Finished-product inventory | Target safety stock | Production capacity | Production decision |
|---|---:|---|---|---|---|
| Fish roti | 160 | Not supplied | Not supplied | Not supplied | Production quantity pending verification. |
| Vegetable rolls | 80 | Not supplied | Not supplied | Not supplied | Production quantity pending verification. |
| Chicken kottu | 90 | Not supplied | Not supplied | Not supplied | Production quantity pending verification. |
| Rice and curry packs | 60 | Not supplied | Not supplied | Not supplied | Production quantity pending verification. |
| Pol sambol sachets | 80 | Not supplied | Not supplied | Not supplied | Production quantity pending verification. |

- **Total estimated demand:** 470 units.
- **Total production requirement:** Pending verification.
- **Production capacity assessment:** Cannot be completed using the supplied information.

Estimated product demand must not be interpreted as approved production quantities.

---

## 8. Assumptions and Limitations

| Category | Explanation |
|---|---|
| Historical data | All supplied sales figures are treated as valid recorded sales. |
| Demand assumption | Historical sales are used as a proxy for demand because no stockouts are reported. |
| Forecasting assumption | Existing linear sales trends are assumed to continue into Week 5. |
| Historical period | Only four weeks of historical observations are available. |
| Seasonality | The forecasting method does not account for seasonal demand changes. |
| Market conditions | Unexpected changes in customer behaviour or market conditions are not incorporated. |
| Operational information | Inventory, safety stock and production capacity are unavailable. |
| Forecast accuracy | Forecasts are estimates rather than guaranteed future sales. |
| Human oversight | All recommendations require production manager verification. |

---

## 9. Management Summary

Flavors of Ceylon is expected to experience increasing overall demand in Week 5, with an estimated total demand of **470 units**, representing a projected increase of **6.82%** compared with Week 4 recorded sales.

Fish roti, chicken kottu and pol sambol sachets demonstrate increasing sales trends and should receive greater planning attention.

Vegetable rolls demonstrate declining sales, requiring careful inventory management to minimise potential overproduction and food waste.

Rice and curry packs demonstrate stable demand.

Although all five products have high data reliability, the limited historical period and simple forecasting method restrict prediction accuracy.

### Recommended Next Steps

- Prioritise demand planning for fish roti, chicken kottu and pol sambol sachets.
- Review vegetable roll inventory to minimise potential excess stock.
- Maintain the demand planning baseline for rice and curry packs.
- Verify usable finished-product inventory.
- Confirm target safety stock requirements.
- Assess available production capacity.
- Compare Week 5 actual sales against forecast estimates.
- Obtain production manager approval before finalising manufacturing quantities.

---

## 10. Final Outcome

Numerical demand forecasts have been successfully generated for all five products using the supplied historical sales data.

No historical figures have been invented, modified or excluded.

| Final assessment | Result |
|---|---|
| Forecasted products | 5 out of 5 |
| Withheld forecasts | 0 |
| Total estimated demand | 470 units |
| Data reliability | High for all products |
| Production quantities | Pending verification |
| Management review | Required |

---

> **Disclaimer:** This report is intended for business decision support only. Estimated demand must not be interpreted as approved production quantities. All recommendations require production manager review before operational implementation.


### Test Case B — Actual AI Output


# Flavors of Ceylon
## P01 – Demand Forecasting and Production Planning
### Version 1.1 – Test B Output

---

## 1. Test Overview

| Category | Description |
|---|---|
| Business Name | Flavors of Ceylon |
| Industry | Australian Food Manufacturing |
| Prompt ID | P01 |
| Prompt Version | Version 1.1 |
| Test Scenario | Test B – Incomplete Sales Data and Stockout Disruption |
| Historical Period | Weeks 1–4 |
| Forecast Period | Week 5 |
| Objective | Forecast product demand and support production planning |

---

## 2. Historical Sales Data

All available figures represent units sold.

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | Missing | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 25 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | Missing | 60 | Missing |

### Additional Information

- Fish roti Week 3 sales are unavailable due to a reporting system error.
- Chicken kottu was out of stock for four days during Week 4.
- Some pol sambol sales records are unavailable.
- No promotional campaign information is supplied.

---

## 3. Data Validation

The historical sales records were reviewed before generating Week 5 demand forecasts.

| Product | Data Quality Issue | Validation Action |
|---|---|---|
| Fish roti | Week 3 sales missing | Exclude Week 3 and retain actual week positions |
| Vegetable rolls | No reported issues | Use all four observations |
| Chicken kottu | Week 4 stockout lasting four days | Exclude Week 4 from baseline trend calculations |
| Rice and curry packs | No reported issues | Use all four observations |
| Pol sambol sachets | Weeks 2 and 4 missing | Withhold forecast due to insufficient observations |

### Data Validation Findings

- No negative or invalid numerical sales records were identified.
- Missing sales records were not interpreted as zero sales.
- Missing historical figures were not invented or estimated.
- Chicken kottu's Week 4 recorded sales of 25 units were excluded from baseline demand calculations.
- Stockout-affected sales do not necessarily represent unrestricted customer demand.
- Pol sambol sachets have insufficient usable observations for numerical forecasting.

---

## 4. Forecasting Method

A simple linear trend extrapolation method is applied.

At least three usable weekly observations are required before generating a numerical forecast.

### Average Weekly Change

Average weekly change = (Latest usable sales - Earliest usable sales) / Number of elapsed weeks

### Target-Week Forecast

Forecast = Latest usable sales + (Average weekly change × Weeks until target week)

### Forecasting Rules

- Use actual week positions.
- Exclude missing and stockout-affected observations.
- Round final forecasts to the nearest whole unit, with half units rounded upwards.
- Set negative forecasts to zero and flag the limitation.
- Withhold forecasts when fewer than three usable observations are available.

---

## 5. Week 5 Demand Forecast

| Product | Usable Observations | Missing or Excluded Records | Average Weekly Change | Sales Trend | Week 5 Forecast | Data Reliability | Recommended Planning Action |
|---|---:|---|---:|---|---|---|---|
| Fish roti | 3 | Week 3 missing | +20 | Increasing | 160 units | Medium | Prepare for increasing demand and recover missing sales records |
| Vegetable rolls | 4 | None | -10 | Decreasing | 80 units | High | Review declining demand to minimise excess inventory |
| Chicken kottu | 3 | Week 4 stockout | +10 | Increasing | 90 units | Medium | Prioritise product availability and investigate stockouts |
| Rice and curry packs | 4 | None | 0 | Stable | 60 units | High | Maintain stable demand planning |
| Pol sambol sachets | 2 | Weeks 2 and 4 missing | N/A | Undetermined | Insufficient data — forecast withheld. | Insufficient | Recover missing records before forecasting |

---

## 6. Detailed Calculation Breakdown

### 6.1 Fish Roti

- Earliest usable sales: 80 units (Week 1)
- Latest usable sales: 140 units (Week 4)
- Usable observations: 3
- Elapsed weeks: 3
- Weeks until target week: 1

**Average weekly change:**

(140 - 80) / (4 - 1) = 20 units

**Week 5 forecast:**

140 + (20 × 1) = 160 units

**Estimated demand: 160 units**

**Sales trend:** Increasing

**Data reliability:** Medium

Week 3 is missing, but three usable observations remain. Actual elapsed weeks are retained in the calculation.

### 6.2 Vegetable Rolls

- Earliest usable sales: 120 units (Week 1)
- Latest usable sales: 90 units (Week 4)
- Usable observations: 4
- Elapsed weeks: 3
- Weeks until target week: 1

**Average weekly change:**

(90 - 120) / (4 - 1) = -10 units

**Week 5 forecast:**

90 + (-10 × 1) = 80 units

**Estimated demand: 80 units**

**Sales trend:** Decreasing

**Data reliability:** High

Historical sales demonstrate a consistent decline of 10 units per week.

### 6.3 Chicken Kottu

- Earliest usable sales: 50 units (Week 1)
- Latest usable sales: 70 units (Week 3)
- Usable observations: 3
- Elapsed weeks: 2
- Weeks until target week: 2

Week 4 sales are excluded because of the reported stockout.

**Average weekly change:**

(70 - 50) / (3 - 1) = 10 units

**Week 5 forecast:**

70 + (10 × 2) = 90 units

**Estimated demand: 90 units**

**Sales trend:** Increasing

**Data reliability:** Medium

The calculation uses the actual two-week interval between Week 3 and Week 5.

The actual customer demand lost during the Week 4 stockout remains unknown.

### 6.4 Rice and Curry Packs

- Earliest usable sales: 60 units (Week 1)
- Latest usable sales: 60 units (Week 4)
- Usable observations: 4
- Elapsed weeks: 3
- Weeks until target week: 1

**Average weekly change:**

(60 - 60) / (4 - 1) = 0 units

**Week 5 forecast:**

60 + (0 × 1) = 60 units

**Estimated demand: 60 units**

**Sales trend:** Stable

**Data reliability:** High

Historical sales demonstrate a stable pattern.

### 6.5 Pol Sambol Sachets

- Week 1 sales: 40 units
- Week 3 sales: 60 units
- Missing records: Weeks 2 and 4
- Usable observations: 2

The minimum requirement of three usable observations is not satisfied.

**Insufficient data — forecast withheld.**

**Sales trend:** Undetermined

**Data reliability:** Insufficient

---

## 7. Estimated Demand Subtotal

| Product | Week 5 Estimated Demand |
|---|---:|
| Fish roti | 160 units |
| Vegetable rolls | 80 units |
| Chicken kottu | 90 units |
| Rice and curry packs | 60 units |
| Pol sambol sachets | Forecast withheld |
| **Estimated Demand Subtotal** | **390 units** |

### Subtotal Calculation

160 + 80 + 90 + 60 = 390 units

### Forecast Coverage

- Total products: 5
- Successfully forecasted products: 4
- Forecasts withheld: 1
- Forecast coverage: 80%

> **Important:** The subtotal of 390 units is not the total business demand because pol sambol sachets have insufficient usable sales records.

All numerical forecasts are non-negative whole numbers. Therefore, no rounding adjustments or zero-floor corrections were required.

---

## 8. Demand Forecast Visualisation

The following text-based chart presents Week 5 estimated demand.

Each block represents 10 units.

```text
Fish roti             ████████████████ 160
Vegetable rolls       ████████          80
Chicken kottu         █████████         90
Rice and curry packs  ██████            60
Pol sambol sachets    Forecast withheld
```

**Estimated demand subtotal: 390 units**

### Historical Sales and Forecast Comparison

| Product | Week 1 | Week 2 | Week 3 | Week 4 | Week 5 Forecast |
|---|---:|---:|---:|---:|---:|
| Fish roti | 80 | 100 | Missing | 140 | 160 |
| Vegetable rolls | 120 | 110 | 100 | 90 | 80 |
| Chicken kottu | 50 | 60 | 70 | 25 (Stockout) | 90 |
| Rice and curry packs | 60 | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | Missing | 60 | Missing | Withheld |

Weeks 1–4 represent recorded historical sales.

Week 5 represents estimated demand, not confirmed customer orders.

---

## 9. Data Reliability Assessment

| Product | Reliability | Justification |
|---|---|---|
| Fish roti | Medium | Three usable observations with one missing record |
| Vegetable rolls | High | Four usable observations with no reported missing or stockout-affected records |
| Chicken kottu | Medium | Three usable observations with one stockout-affected record |
| Rice and curry packs | High | Four usable observations with no reported missing or stockout-affected records |
| Pol sambol sachets | Insufficient | Only two usable observations |

Data reliability classifications describe historical data availability and quality, not statistical forecast confidence or guaranteed prediction accuracy.

---

## 10. Production Planning Recommendations

Estimated demand must be distinguished from actual manufacturing requirements.

### Production Requirement Formula

Production requirement = Forecast demand + Target safety stock - Usable finished-product inventory

Negative production requirements must be set to zero.

However, the following operational information has not been supplied:

- Usable finished-product inventory.
- Target safety stock.
- Available production capacity.
- Other relevant operational constraints.

Therefore, final production quantities cannot be calculated or approved.

| Product | Estimated Demand | Production Requirement Status |
|---|---:|---|
| Fish roti | 160 units | Production quantity pending verification. |
| Vegetable rolls | 80 units | Production quantity pending verification. |
| Chicken kottu | 90 units | Production quantity pending verification. |
| Rice and curry packs | 60 units | Production quantity pending verification. |
| Pol sambol sachets | Forecast withheld | Production quantity pending verification. |

No production capacity assessment can be completed because the necessary capacity information is unavailable.

---

## 11. Risks and Limitations

| Risk or Limitation | Potential Business Impact | Recommended Mitigation |
|---|---|---|
| Missing historical sales records | Reduced forecasting reliability | Recover and validate missing records |
| Stockout-affected sales | Underestimation of unrestricted customer demand | Maintain stockout records and improve availability |
| Short historical period | Limited understanding of long-term demand patterns | Collect additional historical sales data |
| Missing promotional information | Promotional demand changes cannot be assessed | Verify upcoming promotional activities |
| Unknown inventory levels | Risk of overproduction or underproduction | Confirm usable finished-product inventory |
| Unknown safety stock requirements | Inadequate inventory buffers | Establish verified safety stock targets |
| Unknown production capacity | Manufacturing feasibility cannot be confirmed | Verify available production capacity |
| Simple linear forecasting method | Cannot adequately account for seasonality or unexpected market changes | Review forecasts regularly using updated business information |

### Assumptions

- Baseline sales trends are assumed to continue into Week 5.
- Usable historical sales are treated as a proxy for demand.
- Missing records are not assumed to represent zero sales.
- No assumption is made that promotional campaigns did not occur.
- Forecast demand does not automatically represent required production quantities.
- The irregular decline in chicken kottu sales during Week 4 is associated with the reported stockout.
- The actual quantity of unmet demand during the stockout is unknown.

---

## 12. Management Summary

The Week 5 demand forecasting analysis identifies the following key findings.

### Key Sales Trends

- **Fish roti:** Increasing baseline sales trend, with estimated demand of 160 units.
- **Vegetable rolls:** Decreasing sales trend, with estimated demand of 80 units.
- **Chicken kottu:** Increasing baseline sales trend after excluding stockout-affected sales, with estimated demand of 90 units.
- **Rice and curry packs:** Stable sales trend, with estimated demand of 60 units.
- **Pol sambol sachets:** Undetermined sales trend due to insufficient usable observations.

### Products Requiring Planning Attention

Fish roti and chicken kottu require attention because of their increasing baseline sales trends.

Vegetable rolls require careful demand planning to minimise potential overproduction and food waste.

Pol sambol sachets require additional verified sales records before a numerical forecast can be generated.

### Data Quality Concerns

- Fish roti Week 3 sales records are missing.
- Chicken kottu Week 4 sales are affected by a stockout.
- Pol sambol sachets have two missing weekly sales records.
- Promotional campaign information is unavailable.

### Recommended Next Steps

1. Recover missing fish roti and pol sambol sachet sales records.
2. Investigate the causes of chicken kottu stockouts.
3. Improve inventory monitoring and product availability.
4. Review the decreasing demand trend for vegetable rolls.
5. Verify finished-product inventory levels.
6. Establish appropriate safety stock targets.
7. Confirm available production capacity.
8. Verify upcoming promotional campaigns.
9. Recalculate production requirements using verified information.
10. Obtain production manager approval before implementation.

---

## 13. Final Conclusion

The improved demand forecasting prompt successfully generates Week 5 demand estimates while addressing incomplete historical records and stockout-related disruptions.

The forecasting process excludes unsuitable observations, retains actual elapsed weeks and prevents unsupported forecasts from being generated.

The estimated demand subtotal is 390 units across four products. This does not represent the total business demand because the forecast for pol sambol sachets has been withheld.

The analysis improves transparency and supports evidence-based production planning while reducing the risk of misleading forecasting results.

However, actual production quantities remain pending verification because the required inventory, safety stock and production capacity information is unavailable.

---

## 14. Prompt Performance Evaluation

| Evaluation Criteria | Test Result |
|---|---|
| Identifies missing sales records | Pass |
| Avoids treating missing records as zero | Pass |
| Avoids inventing historical sales figures | Pass |
| Excludes stockout-affected sales | Pass |
| Uses actual elapsed weeks | Pass |
| Applies the minimum observation requirement | Pass |
| Generates correct numerical forecasts | Pass |
| Classifies sales trends correctly | Pass |
| Assigns data reliability levels correctly | Pass |
| Withholds unsupported forecasts | Pass |
| Reports a subtotal instead of total business demand | Pass |
| Separates estimated demand from production requirements | Pass |
| Identifies operational information requiring verification | Pass |
| Provides management recommendations | Pass |
| Identifies assumptions, risks and limitations | Pass |

### Overall Test Evaluation

**Result: Successful**

Version 1.1 demonstrates appropriate handling of incomplete sales data, stockout disruptions and insufficient operational information in this test scenario.

The prompt supports responsible business decision-making by avoiding unsupported forecasts and manufacturing recommendations.

The evaluation is based on this test output and does not guarantee performance across all future business scenarios.

---

## 15. Human Review and Decision Disclaimer

> All forecasts are indicative estimates provided for business decision support only.
>
> Production quantities remain pending verification.
>
> All outputs require production manager review and approval before operational use.

---

**End of Test B Output – P01 Version 1.1**

### Observed Improvements

- Correctly validated all 20 historical sales records
  in Test Case A.
- Generated accurate forecasts for all five products,
  with a total estimated demand of 470 units.
- Provided transparent forecasting calculations
  for every forecasted product.
- Applied consistent data reliability classifications.
- Correctly identified all missing sales records
  in Test Case B.
- Preserved missing historical observations without
  estimating or replacing them.
- Excluded stockout-affected chicken kottu sales
  from baseline demand calculations.
- Correctly used actual elapsed weeks when
  calculating demand forecasts.
- Withheld the pol sambol forecast because only
  two usable historical observations were available.
- Reported 390 units as a partial demand subtotal
  rather than total business demand.
- Clearly separated demand estimates from actual
  manufacturing requirements.
- Withheld production quantities until inventory,
  safety stock and capacity information could
  be verified.
- Strengthened human review and approval requirements.

### Remaining Limitations

- The generated reports are lengthy and contain
  some repeated information across sections.
- The forecasting method relies on the earliest
  and latest usable sales observations and may
  overlook irregular intermediate sales patterns.
- The method does not account for seasonality,
  sudden demand changes or external market factors.
- Data reliability classifications do not represent
  statistical forecast confidence.
- The production requirement formula was presented
  but could not be tested numerically because
  operational information was unavailable.
- Forecast accuracy against actual future sales
  has not been established.
- Repeat-run consistency has not been evaluated.

### Evaluation Results

| Criterion | Test Case A | Test Case B |
|---|---:|---:|
| Accuracy | 2 | 2 |
| Completeness | 2 | 2 |
| Consistency | 2 | 2 |
| Business Relevance | 2 | 2 |
| Responsible AI | 2 | 2 |
| Total | 10/10 | 10/10 |

Combined evaluation score: 20/20 (100%).

### Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---:|---:|---:|
| v1.0 | 9/10 | 7/10 | 16/20 (80%) |
| v1.1 | 10/10 | 10/10 | 20/20 (100%) |

Absolute improvement: 20 percentage points.

Relative improvement in evaluation score: 25%.

### Evaluation Conclusion

The revised v1.1 prompt successfully addressed
the major weaknesses identified during initial
testing.

It improved calculation transparency, missing-data
handling, reliability classification and responsible
production planning.

Both scenarios satisfied the selected project
evaluation criteria.

However, further refinement may improve report
efficiency and production capacity handling.

Additional testing using complete operational
information is recommended to evaluate the
production requirement calculation.

The evaluation results measure response quality
for the selected synthetic scenarios and do not
establish actual commercial forecasting accuracy.

---

## 7. Version v1.2 — Further Refined Prompt Testing

### Testing Date and AI Model

25 November 2026 | ChatGPT

### Test Case A — Actual AI Output

# Flavors of Ceylon – Demand Forecasting and Production Planning

## Test A – Complete Historical Sales

| Test Information | Description |
|---|---|
| Prompt ID | P01 |
| Prompt version | v1.1 |
| Test scenario | Complete historical sales |
| Business | Flavors of Ceylon |
| Forecast period | Week 5 |
| Forecasting method | Simple linear trend extrapolation |
| Expected result | 470 units estimated demand |
| Actual result | 470 units estimated demand |
| Test status | PASS |

---

## 1. Data Validation

The analysis uses the historical sales figures supplied in the previous Test A scenario.

### Historical Sales Records

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | 120 | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 80 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | 50 | 60 | 70 |
| **Total recorded sales** | **350** | **380** | **410** | **440** |

### Data Validation Results

| Validation Criterion | Result |
|---|---|
| Total historical records | 20 |
| Usable records | 20 |
| Missing records | None |
| Invalid records | None |
| Reported stockouts | None |
| Excluded records | None |
| Reported promotional events | None |
| Irregular sales patterns | None identified |
| Forecast eligibility | All five products |

All historical figures represent recorded units sold rather than estimated customer demand.

No missing values were replaced, and no historical sales figures were invented.

---

## 2. Demand Forecast and Calculation Breakdown

### Week 5 Demand Forecast

| Product | Usable Observations | Missing or Excluded Records | Average Weekly Change | Sales Trend | Week 5 Forecast | Data Reliability | Recommended Planning Action |
|---|---:|---|---:|---|---:|---|---|
| Fish roti | 4 | None | +20 | Increasing | 160 | High | Plan for higher demand |
| Vegetable rolls | 4 | None | -10 | Decreasing | 80 | High | Adjust demand planning downwards |
| Chicken kottu | 4 | None | +10 | Increasing | 90 | High | Plan for higher demand |
| Rice and curry packs | 4 | None | 0 | Stable | 60 | High | Maintain existing demand plan |
| Pol sambol sachets | 4 | None | +10 | Increasing | 80 | High | Plan for higher demand |
| **Total** | **20** | **None** | **+30** | **Increasing** | **470** | — | — |

### Forecasting Formulas

**Average weekly change:**

> Average weekly change = (Latest usable sales - Earliest usable sales) / Number of elapsed weeks

**Target-week forecast:**

> Forecast = Latest usable sales + (Average weekly change × Number of weeks ahead)

### Calculation Breakdown

| Product | Average Weekly Change Calculation | Week 5 Forecast Calculation | Forecast |
|---|---|---|---:|
| Fish roti | (140 - 80) / 3 = 20 | 140 + (20 × 1) | 160 |
| Vegetable rolls | (90 - 120) / 3 = -10 | 90 + (-10 × 1) | 80 |
| Chicken kottu | (80 - 50) / 3 = 10 | 80 + (10 × 1) | 90 |
| Rice and curry packs | (60 - 60) / 3 = 0 | 60 + (0 × 1) | 60 |
| Pol sambol sachets | (70 - 40) / 3 = 10 | 70 + (10 × 1) | 80 |

### Total Estimated Demand

160 + 80 + 90 + 60 + 80 = **470 units**

### Estimated Demand Growth

(470 - 440) / 440 × 100 = **6.82%**

### Key Forecast Results

| Performance Indicator | Result |
|---|---:|
| Week 4 recorded sales | 440 units |
| Week 5 estimated demand | 470 units |
| Estimated increase | 30 units |
| Estimated percentage increase | 6.82% |
| Products successfully forecasted | 5 out of 5 |
| Products with increasing trends | 3 |
| Products with decreasing trends | 1 |
| Products with stable trends | 1 |
| Forecasts withheld | 0 |

All forecasts are non-negative whole units. No rounding adjustments are required.

All products meet the high data reliability criteria because four usable historical observations are available without missing or stockout-affected records.

> **Result:** The calculated total estimated demand of 470 units matches the expected Test A result.

---

## 3. Production Planning and Capacity Analysis

Estimated customer demand is 470 units. However, actual production requirements cannot be determined because usable finished-product inventory, target safety stock and available production capacity have not been supplied.

### Production Planning Results

| Product | Forecast Demand | Usable Finished-Product Inventory | Target Safety Stock | Required Production | Available Production Capacity | Capacity-Limited Production | Production Shortfall | Estimated Demand Shortfall | Safety Stock Shortfall | Recommended Action |
|---|---:|---|---|---|---|---|---|---|---|---|
| Fish roti | 160 | — | — | — | — | — | — | — | — | Verify operational data |
| Vegetable rolls | 80 | — | — | — | — | — | — | — | — | Verify operational data |
| Chicken kottu | 90 | — | — | — | — | — | — | — | — | Verify operational data |
| Rice and curry packs | 60 | — | — | — | — | — | — | — | — | Verify operational data |
| Pol sambol sachets | 80 | — | — | — | — | — | — | — | — | Verify operational data |
| **Total** | **470** | — | — | — | — | — | — | — | — | Pending verification |

**Note:** A dash (—) indicates unavailable information or a calculation that cannot be completed. It does not represent zero.

> **Production quantity pending verification.**

This status applies to all five products.

### Operational Readiness Assessment

| Production Planning Criterion | Status |
|---|---|
| Total estimated customer demand | 470 units |
| Total required production | Pending verification |
| Capacity-limited production | Pending verification |
| Products requiring no additional production | Cannot be determined |
| Production shortfall | Cannot be determined |
| Estimated unmet customer demand | Cannot be determined |
| Projected closing inventory | Cannot be determined |
| Safety stock shortfall | Cannot be determined |
| Shared production resource availability | Not supplied |
| Overall manufacturing feasibility | Not confirmed |

### Production Planning Safeguards

- Estimated customer demand must not be interpreted as required production.
- Missing operational information must not be treated as zero.
- Production quantities must not be calculated using unverified operational information.
- Unused production capacity for one product must not be assumed to be transferable to another.
- Unmet customer demand must be distinguished from safety stock shortfalls.
- Shared production resources and operational restrictions must be reviewed before confirming manufacturing feasibility.
- All production quantities require production manager approval.

---

## 4. Assumptions and Limitations

| Category | Assumption or Limitation |
|---|---|
| Historical data | Only the four historical weeks supplied in Test A are used. |
| Forecasting method | Assumes the historical linear sales trend continues into Week 5. |
| Data reliability | High reliability indicates complete usable records, not guaranteed forecast accuracy. |
| Seasonality | The forecasting method does not account for seasonal demand variations. |
| Market changes | Unexpected customer behaviour and market changes are not incorporated. |
| Promotional activities | No unusual promotional events are reported. |
| Historical sales | Recorded units sold may not necessarily represent actual customer demand. |
| Operational information | Finished-product inventory, safety stock and production capacity are unavailable. |
| Forecast accuracy | Future actual sales are unavailable for measuring forecast error. |
| Human oversight | All recommendations require production manager review and approval. |

---

## 5. Management Summary and Priority Actions

Flavors of Ceylon is forecast to experience Week 5 demand of **470 units**, representing a 6.82% increase compared with Week 4 recorded sales. Fish roti, chicken kottu and pol sambol sachets show increasing sales trends, while vegetable rolls are declining and rice and curry packs remain stable. All products meet the high data reliability criteria. However, production quantities cannot be confirmed without verified operational information.

### Priority Actions

1. Prioritise planning for products with increasing demand.
2. Adjust vegetable roll demand planning downwards.
3. Verify finished-product inventory and safety stock requirements.
4. Confirm product-specific capacity and shared resource constraints.
5. Obtain production manager approval before implementation.

---

## 6. Test Evaluation

### Expected Results vs Actual Results

| Test Criterion | Expected Result | Actual Result | Status |
|---|---|---|---|
| Historical data validation | Complete usable records | 20 usable records | PASS |
| Missing-data handling | No invented historical values | No missing values or invented records | PASS |
| Forecast result | 470 units | 470 units | PASS |
| Sales trend classification | Correct classifications | All five products classified correctly | PASS |
| Data reliability classification | High | High for all five products | PASS |
| Calculation transparency | All forecasts explained | All calculations provided | PASS |
| Missing operational data handling | Production quantities withheld | Production quantity pending verification | PASS |
| Negative forecast prevention | No negative quantities | No negative quantities | PASS |
| Demand and production distinction | Clearly separated | Clearly separated | PASS |
| Management summary | Maximum 120 words | Within word limit | PASS |
| Human oversight | Management approval required | Approval requirement included | PASS |

### Strengths Identified

- Produces consistent and transparent numerical forecasts.
- Correctly uses elapsed weeks in forecasting calculations.
- Provides clear product-level sales trend classifications.
- Separates estimated demand from production requirements.
- Avoids unsupported assumptions about operational information.
- Includes appropriate human oversight safeguards.
- Supports structured and repeatable demand planning.

### Remaining Limitations

- The forecasting method cannot identify seasonal or complex demand patterns.
- Four historical weeks provide limited evidence for future demand.
- High data reliability does not guarantee forecast accuracy.
- Actual production quantities cannot be calculated without additional operational data.
- Further testing is required using incomplete records, stockouts, irregular demand and capacity restrictions.

### Overall Test Status

**PASS**

- Expected estimated demand: 470 units
- Actual estimated demand: 470 units
- Difference from expected result: 0 units
- Expected result achieved: Yes

### Conclusion

Prompt P01 v1.1 successfully meets the expected Test A demand forecast of 470 units.

The prompt demonstrates transparent forecasting calculations, consistent sales trend classifications, appropriate data reliability assessments and responsible handling of missing operational information.

The result confirms agreement with the expected test outcome but does not establish statistical forecast accuracy or manufacturing feasibility.

Further testing under alternative business scenarios is required to evaluate the robustness of the prompt.

---

*All outputs are for decision support and require production manager review before operational implementation.*

### Test Case B — Actual AI Output

# Flavors of Ceylon – P01 v1.2 – Test B

## Test Overview

| Attribute | Description |
| --- | --- |
| Business | Flavors of Ceylon |
| Prompt ID | P01 |
| Prompt Version | v1.2 |
| Workflow | Demand Forecasting and Production Planning |
| Test | Test B |
| Scenario | Incomplete data and stockouts |
| Forecast Period | Week 5 |
| Expected Key Result | 390-unit partial subtotal |
| Actual Result | 390-unit partial subtotal |
| Test Status | PASS |

---

## 1. Data Validation

The analysis uses historical weekly sales data for Weeks 1–4. All available numerical figures represent recorded units sold rather than confirmed customer demand.

### Historical Sales Data

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
| --- | ---: | ---: | ---: | ---: |
| Fish roti | 80 | 100 | Missing | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 25 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | Missing | 60 | Missing |

### Identified Data Quality Issues

| Product | Data Issue | Validation Decision |
| --- | --- | --- |
| Fish roti | Week 3 sales unavailable | Exclude missing record |
| Vegetable rolls | No identified issues | Use all four observations |
| Chicken kottu | Week 4 stockout | Exclude Week 4 from baseline forecasting |
| Rice and curry packs | No identified issues | Use all four observations |
| Pol sambol sachets | Weeks 2 and 4 unavailable | Withhold forecast |

### Validation Findings

- Missing records have not been interpreted as zero sales.
- No historical sales figures have been invented.
- Chicken kottu's Week 4 recorded sales of 25 units are retained as historical information but excluded from baseline demand calculations.
- Pol sambol sachets have fewer than three usable observations.
- Recorded sales and estimated customer demand are treated separately.

---

## 2. Demand Forecast and Calculation Breakdown

### Forecasting Method

Simple linear trend extrapolation is applied using actual historical week positions.

**Average weekly change:**

Average weekly change = (Latest usable sales - Earliest usable sales) / Number of elapsed weeks

**Demand forecast:**

Forecast = Latest usable sales + (Average weekly change × Number of weeks between the latest usable observation and target week)

A minimum of three usable weekly observations is required to generate a numerical forecast.

### Week 5 Demand Forecast

| Product | Usable Observations | Missing or Excluded Records | Average Weekly Change | Sales Trend | Week 5 Forecast | Data Reliability | Recommended Planning Action |
| --- | ---: | --- | ---: | --- | ---: | --- | --- |
| Fish roti | 3 | Week 3 | +20 | Increasing | 160 | Medium | Plan for higher demand |
| Vegetable rolls | 4 | None | -10 | Decreasing | 80 | High | Reduce planned volume |
| Chicken kottu | 3 | Week 4 | +10 | Increasing | 90 | Medium | Review stock availability |
| Rice and curry packs | 4 | None | 0 | Stable | 60 | High | Maintain current planning level |
| Pol sambol sachets | 2 | Weeks 2 and 4 | N/A | Undetermined | Withheld | Insufficient | Recover missing records |

### Calculation Breakdown

#### 2.1 Fish Roti

- Earliest usable observation: Week 1 = 80 units
- Latest usable observation: Week 4 = 140 units
- Usable observations: 3
- Elapsed weeks: 4 - 1 = 3
- Weeks until target week: 5 - 4 = 1

Average weekly change:

`(140 - 80) / 3 = 20 units`

Week 5 forecast:

`140 + (20 × 1) = 160 units`

**Final forecast: 160 units**

**Sales trend:** Increasing

**Data reliability:** Medium

---

#### 2.2 Vegetable Rolls

- Earliest usable observation: Week 1 = 120 units
- Latest usable observation: Week 4 = 90 units
- Usable observations: 4
- Elapsed weeks: 4 - 1 = 3
- Weeks until target week: 5 - 4 = 1

Average weekly change:

`(90 - 120) / 3 = -10 units`

Week 5 forecast:

`90 + (-10 × 1) = 80 units`

**Final forecast: 80 units**

**Sales trend:** Decreasing

**Data reliability:** High

---

#### 2.3 Chicken Kottu

- Earliest usable observation: Week 1 = 50 units
- Latest usable observation: Week 3 = 70 units
- Usable observations: 3
- Excluded observation: Week 4 due to stockout
- Elapsed weeks: 3 - 1 = 2
- Weeks until target week: 5 - 3 = 2

Average weekly change:

`(70 - 50) / 2 = 10 units`

Week 5 forecast:

`70 + (10 × 2) = 90 units`

**Final forecast: 90 units**

**Sales trend:** Increasing

**Data reliability:** Medium

Week 4 recorded sales are excluded because the reported stockout restricted product availability.

---

#### 2.4 Rice and Curry Packs

- Earliest usable observation: Week 1 = 60 units
- Latest usable observation: Week 4 = 60 units
- Usable observations: 4
- Elapsed weeks: 4 - 1 = 3
- Weeks until target week: 5 - 4 = 1

Average weekly change:

`(60 - 60) / 3 = 0 units`

Week 5 forecast:

`60 + (0 × 1) = 60 units`

**Final forecast: 60 units**

**Sales trend:** Stable

**Data reliability:** High

---

#### 2.5 Pol Sambol Sachets

- Available observations: Weeks 1 and 3
- Missing observations: Weeks 2 and 4
- Minimum required observations: 3
- Actual usable observations: 2

**Insufficient data — forecast withheld.**

**Sales trend:** Undetermined

**Data reliability:** Insufficient

No numerical forecast has been generated because the minimum observation requirement has not been satisfied.

### Partial Demand Subtotal

| Product | Estimated Week 5 Demand |
| --- | ---: |
| Fish roti | 160 |
| Vegetable rolls | 80 |
| Chicken kottu | 90 |
| Rice and curry packs | 60 |
| Pol sambol sachets | Withheld |
| **Partial Subtotal** | **390 units** |

Calculation:

`160 + 80 + 90 + 60 = 390 units`

> **Important:** The 390-unit subtotal represents estimated demand for four forecasted products only. It is not the total business demand because the Pol sambol sachets forecast has been withheld.

---

## 3. Production Planning and Capacity Analysis

### Operational Data Validation

The following operational information has not been supplied:

- Usable finished-product inventory
- Target safety stock
- Available product-specific production capacity
- Shared manufacturing resource restrictions

Missing operational values cannot be assumed to be zero.

Therefore, estimated customer demand cannot be directly converted into confirmed production quantities.

### Production Planning Formulas

The following formulas will be applied when verified operational information becomes available.

**Required production:**

`Maximum(0, Forecast demand + Target safety stock - Usable finished-product inventory)`

**Capacity-limited production:**

`Minimum(Required production, Available product-specific production capacity)`

**Production shortfall:**

`Required production - Capacity-limited production`

**Estimated demand shortfall:**

`Maximum(0, Forecast demand - Usable inventory - Capacity-limited production)`

**Projected closing inventory:**

`Maximum(0, Usable inventory + Capacity-limited production - Forecast demand)`

**Safety stock shortfall:**

`Maximum(0, Target safety stock - Projected closing inventory)`

### Production Planning Results

| Product | Forecast Demand | Usable Inventory | Target Safety Stock | Required Production | Available Capacity | Capacity-Limited Production | Production Shortfall | Estimated Demand Shortfall | Safety Stock Shortfall | Recommended Action |
| --- | ---: | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Fish roti | 160 | Unknown | Unknown | Pending | Unknown | Pending | Pending | Pending | Pending | Verify operational inputs |
| Vegetable rolls | 80 | Unknown | Unknown | Pending | Unknown | Pending | Pending | Pending | Pending | Review existing inventory |
| Chicken kottu | 90 | Unknown | Unknown | Pending | Unknown | Pending | Pending | Pending | Pending | Investigate previous stockout |
| Rice and curry packs | 60 | Unknown | Unknown | Pending | Unknown | Pending | Pending | Pending | Pending | Verify production requirements |
| Pol sambol sachets | Withheld | Unknown | Unknown | Pending | Unknown | Pending | Pending | Pending | Pending | Recover missing sales records |

**Production quantity pending verification.**

### Operational Safeguards

- Forecast demand does not represent confirmed production requirements.
- Missing operational information has not been assumed to be zero.
- Projected closing inventory cannot currently be calculated.
- Products requiring no additional production cannot currently be identified.
- Estimated unmet customer demand cannot be quantified.
- Safety stock shortfalls cannot be quantified.
- Unused production capacity cannot be assumed to be transferable between products.
- Shared production resources require management review.
- All future calculated production quantities require human approval.

---

## 4. Assumptions and Limitations

| Category | Assumption or Limitation |
| --- | --- |
| Forecasting method | Simple linear trend extrapolation is used with actual historical week positions. |
| Historical data | Recorded sales may not fully represent actual customer demand. |
| Missing records | No missing historical figures have been invented or substituted. |
| Stockouts | Chicken kottu's Week 4 sales were affected by restricted availability. |
| Irregular sales patterns | Chicken kottu's sudden recorded sales decline is identified as stockout-related. |
| Future availability | The chicken kottu forecast reflects its baseline sales trend rather than guaranteed Week 5 availability. |
| Seasonality | Seasonal demand fluctuations are not incorporated. |
| Promotions | Promotional effects are not incorporated. |
| Market changes | Unexpected changes in customer behaviour are not incorporated. |
| Data reliability | Reliability classifications describe data quality and availability, not statistical forecast confidence. |
| Operational feasibility | Inventory, safety stock and production capacity remain unverified. |
| Rounding | All numerical forecasts are expressed as non-negative whole units. |
| Human oversight | Production manager approval is required before implementation. |

---

## 5. Management Summary and Priority Actions

The Week 5 forecast produces a partial estimated demand of **390 units across four products**. Fish roti and chicken kottu show increasing trends, vegetable rolls show a decreasing trend, and rice and curry packs remain stable. Pol sambol sachets cannot be forecasted because historical observations are insufficient.

### Priority Actions

1. Recover missing fish roti and Pol sambol sales records.
2. Investigate chicken kottu stockout causes and prevent recurrence.
3. Review planned volumes against forecasted demand trends.
4. Verify inventory, safety stock and available production capacity.
5. Obtain production manager approval before confirming manufacturing quantities.

All forecasts are indicative and intended for management decision support.

---

## 6. Test Evaluation

### Expected Result vs Actual Result

| Evaluation Item | Expected Result | Actual Result | Status |
| --- | --- | --- | --- |
| Fish roti forecast | 160 units | 160 units | PASS |
| Vegetable rolls forecast | 80 units | 80 units | PASS |
| Chicken kottu forecast | 90 units | 90 units | PASS |
| Rice and curry packs forecast | 60 units | 60 units | PASS |
| Pol sambol sachets forecast | Withheld | Withheld | PASS |
| Partial demand subtotal | 390 units | 390 units | PASS |
| Total business demand | Not reported | Not reported | PASS |
| Production quantities | Pending verification | Pending verification | PASS |

### Prompt Performance Evaluation

| Evaluation Criterion | Result | Status |
| --- | --- | --- |
| Missing sales records identified | Correctly identified | PASS |
| Missing records treated as zero | No | PASS |
| Invented historical figures | None | PASS |
| Stockout-affected records excluded | Chicken kottu Week 4 | PASS |
| Minimum three-observation requirement | Correctly applied | PASS |
| Actual week positions used | Correctly applied | PASS |
| Calculation breakdown provided | All forecasted products | PASS |
| Insufficient forecast withheld | Pol sambol sachets | PASS |
| Sales trends classified | Correctly classified | PASS |
| Data reliability classified | Correctly classified | PASS |
| Expected partial subtotal achieved | 390 units | PASS |
| Partial subtotal distinguished from total demand | Yes | PASS |
| Missing operational inputs identified | Yes | PASS |
| Unsupported production quantities avoided | Yes | PASS |
| Demand and production distinguished | Yes | PASS |
| Human approval requirement retained | Yes | PASS |
| Numerical production formulas tested | Operational inputs unavailable | NOT TESTED |

### Observed Strengths

- Accurately identifies incomplete historical sales records.
- Excludes stockout-affected observations from baseline calculations.
- Uses actual elapsed weeks when calculating demand forecasts.
- Prevents unsupported numerical forecasts.
- Produces transparent and reproducible calculations.
- Distinguishes partial demand from total business demand.
- Prevents unsupported production recommendations.
- Supports responsible AI-assisted decision-making.

### Remaining Limitations

- Forecast accuracy cannot be statistically guaranteed.
- The method does not account for seasonal or irregular demand.
- Numerical production and capacity calculations cannot be fully evaluated because operational inputs are unavailable.
- Further testing with verified operational information is required.

### Iteration Evaluation

The revised P01 v1.2 prompt demonstrates effective handling of incomplete sales records, stockout-affected observations and insufficient historical data.

The prompt also includes operational safeguards that prevent estimated customer demand from being incorrectly interpreted as confirmed production requirements.

The missing-operational-data safeguards were successfully tested. However, the numerical production formulas require a separate test containing complete inventory, safety stock and capacity information.

### Final Test Outcome

> **PASS — Test B successfully achieved the expected 390-unit partial demand subtotal.**

All applicable test criteria were satisfied. Numerical production and capacity calculations remain untested due to unavailable operational data.

---

**Disclaimer:** All outputs are intended for business decision support and require production manager review before operational implementation.

### Final Observations

Pending.

---

## 8. Testing Integrity

All sales figures are fictional and created for
academic testing purposes.

Actual AI outputs will be recorded without
retrospective modification.

The results do not demonstrate actual commercial
forecasting performance.

## Related Files

- [P01 Prompt](../02-prompt-library/P01-product-demand-forecasting.md)
- [Testing Evidence Index](README.md)

---

## 9. Test Case C — Production Capacity and Inventory


# Flavors of Ceylon – Demand Forecasting and Production Planning

## P01 – Version 1.2 – Test C

### Test Overview

| Test Information | Details |
| --- | --- |
| Business | Flavors of Ceylon |
| Industry | Australian Food Manufacturing |
| Prompt ID | P01 |
| Prompt Version | v1.2 |
| Test ID | Test C |
| Scenario | Inventory and Capacity Constraints |
| Expected Required Production | 345 units |
| Expected Capacity-Limited Production | 325 units |
| Test Status | Pending Verification |

---

## 1. Data Validation

The test scenario and expected results have been supplied. However, the underlying historical sales and operational records are unavailable in the supplied test input.

| Required Information | Validation Status |
| --- | --- |
| Historical weekly product sales | Not supplied |
| Product names | Not supplied |
| Stockout information | Not supplied |
| Usable finished-product inventory | Not supplied |
| Target safety stock | Not supplied |
| Product-specific production capacity | Not supplied |

Missing information has not been interpreted as zero or replaced with estimated historical values.

---

## 2. Demand Forecast and Calculation Breakdown

| Product Name | Usable Observations | Missing Records | Average Weekly Change | Sales Trend | Next-Week Forecast | Data Reliability | Recommended Action |
| --- | ---: | --- | --- | --- | --- | --- | --- |
| Products not specified | 0 supplied | Historical sales | N/A | Undetermined | Withheld | Insufficient | Obtain sales records |

**Insufficient data — forecast withheld.**

### Forecasting Formulas

**Average Weekly Change**

Average weekly change = (Latest usable sales - Earliest usable sales) / Number of elapsed weeks

**Demand Forecast**

Forecast = Latest usable sales + (Average weekly change × Number of weeks ahead)

Individual product forecasts and total estimated demand cannot be calculated without historical sales records.

---

## 3. Production Planning and Capacity Analysis

**Production quantity pending verification.**

| Product Name | Forecast Demand | Usable Inventory | Target Safety Stock | Required Production | Available Capacity | Capacity-Limited Production | Production Shortfall | Estimated Demand Shortfall | Safety Stock Shortfall | Recommended Action |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Products not specified | N/A | N/A | N/A | Pending | N/A | Pending | Pending | Pending | Pending | Verify operational inputs |

### Production Planning Formulas

- Required production = Max(0, Forecast demand + Target safety stock - Usable inventory)
- Capacity-limited production = Min(Required production, Available product-specific capacity)
- Production shortfall = Required production - Capacity-limited production
- Estimated demand shortfall = Max(0, Forecast demand - Usable inventory - Capacity-limited production)
- Projected closing inventory = Max(0, Usable inventory + Capacity-limited production - Forecast demand)
- Safety stock shortfall = Max(0, Target safety stock - Projected closing inventory)

### Expected Test Outcome

The following results are based exclusively on the supplied expected values and are not independently verified production calculations.

| Performance Indicator | Expected or Derived Result |
| --- | ---: |
| Required production | 345 units |
| Capacity-limited production | 325 units |
| Implied production shortfall | 20 units |
| Production requirement coverage | 94.20% |

### Calculation Breakdown

**Production Shortfall**

345 - 325 = 20 units

**Production Requirement Coverage**

(325 / 345) × 100 = 94.20%

The 20-unit production shortfall does not necessarily represent unmet customer demand. It may represent a customer demand shortfall, a safety stock shortfall or a combination of both.

---

## 4. Assumptions and Limitations

- No missing historical or operational values have been invented.
- Missing records have not been interpreted as zero.
- Expected test results are treated as validation benchmarks rather than confirmed calculations.
- The forecasting method does not account for seasonality, irregular demand or unexpected market changes.
- Data reliability classifications do not represent statistical forecast confidence.
- Unused production capacity cannot automatically be transferred between products.
- Shared production resources and operational restrictions require management review.
- All production quantities require human approval.

---

## 5. Management Summary and Priority Actions

The expected Test C results indicate a production requirement of 345 units and capacity-limited production of 325 units, implying a production shortfall of 20 units.

However, historical sales, inventory, safety stock and production capacity records are unavailable. Therefore, individual demand forecasts and production quantities cannot be independently verified.

### Priority Actions

1. Obtain and validate historical weekly sales records.
2. Confirm available finished-product inventory.
3. Verify product-specific safety stock requirements.
4. Review production capacity and identify potential constraints.
5. Obtain production manager approval before implementation.

---

## 6. Test Evaluation

| Evaluation Criterion | Result |
| --- | --- |
| Missing-data identification | Pass |
| Prevention of fabricated sales figures | Pass |
| Demand and production distinction | Pass |
| Production shortfall arithmetic | Pass |
| Identification of capacity constraints | Partial |
| Verification of 345 required units | Pending |
| Verification of 325 capacity-limited units | Pending |
| Distinction between demand and safety stock shortfalls | Pass |
| Operational safeguards | Pass |
| Structured output format | Pass |
| Overall test result | Incomplete — additional input data required |

---

## 7. Iteration Testing Evidence

### Testing Objective

Evaluate whether Prompt P01 v1.2 can distinguish customer demand forecasts from actual production requirements while considering finished-product inventory, safety stock and production capacity constraints.

### Expected Behaviour

- Calculate demand using valid historical sales records.
- Adjust production requirements based on inventory and safety stock.
- Apply product-specific production capacity limits.
- Identify production shortfalls.
- Distinguish unmet customer demand from safety stock shortfalls.
- Avoid generating unsupported production quantities.
- Flag missing operational information.

### Observed Behaviour

The AI correctly identified missing historical and operational information and withheld unsupported demand forecasts and production quantities.

The AI calculated an implied production shortfall of 20 units using the supplied expected results without presenting those results as independently verified calculations.

### Strengths

- Improved data validation.
- Prevention of fabricated business information.
- Clear distinction between demand and production quantities.
- Identification of operational limitations.
- Responsible decision-support recommendations.
- Consistent and structured reporting.

### Remaining Limitations

The expected production quantities could not be independently verified because the complete Test C dataset was not supplied.

### Recommended Next Step

Repeat Test C using complete historical sales, usable inventory, target safety stock and product-specific production capacity information.

### Conclusion

Prompt P01 v1.2 demonstrates appropriate missing-data handling and operational safeguards. However, its numerical forecasting and capacity-planning performance cannot be fully validated until the complete test dataset is provided.

**Final Status: Partially Validated — Retesting Required**

---

> **Disclaimer:** All outputs are for decision support and require production manager review before operational implementation.

### Testing Objective

Evaluate numerical production requirements,
available finished-product inventory, safety
stock targets and production capacity constraints.

### Test Input

The production manager requires Week 5 demand
estimates and indicative production planning.

#### Historical Weekly Sales

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | 120 | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 80 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | 50 | 60 | 70 |

#### Verified Operational Information

| Product | Usable Inventory | Target Safety Stock | Weekly Production Capacity |
|---|---:|---:|---:|
| Fish roti | 30 | 10 | 120 |
| Vegetable rolls | 90 | 5 | 60 |
| Chicken kottu | 10 | 5 | 100 |
| Rice and curry packs | 20 | 10 | 60 |
| Pol sambol sachets | 15 | 5 | 70 |

All figures represent units.

Inventory represents usable finished products
available at the beginning of Week 5.

Production capacities are independent weekly
limits for each product.

No shared resource constraints or other
operational restrictions are reported.

No stock shortages or unusual promotional
events are reported in the historical period.

All information is synthetic and treated as
verified for the purpose of this test.

### Expected Output

- Generate accurate demand forecasts.
- Calculate indicative production requirements.
- Set negative production requirements to zero.
- Identify production capacity shortfalls.
- Distinguish demand from feasible production.
- Flag decisions requiring management approval.

### v1.1 — Additional Baseline Test

Testing date: 25 November 2026

AI tool and model: ChatGPT

Actual AI output:

Pending testing.

### Observations

The v1.1 prompt successfully calculated numerical
production requirements using the supplied historical
sales and verified synthetic operational information.

The response correctly calculated:

- Total estimated demand: 470 units.
- Required production: 345 units.
- Capacity-limited production: 325 units.
- Total production shortfall: 20 units.
- Estimated unmet fish roti demand: 10 units.
- Fish roti safety stock shortfall: 10 units.

The prompt correctly identified that vegetable rolls
required no additional production because existing
inventory could satisfy forecast demand and the
target safety stock.

The response also recognised that unused production
capacity for other products could not automatically
be transferred to fish roti.

### Strengths

- Accurate forecasting and production calculations.
- Appropriate inventory and capacity analysis.
- Correct handling of negative production requirements.
- Clear distinction between demand and production.
- Appropriate management review recommendations.

### Remaining Limitations

- Lengthy report containing repeated information.
- Unrequested visualisations.
- Shortfall calculations were not presented in a
  standardised table for every product.
- Invalid operational inputs were not tested.

### Evaluation Scores

| Criterion | Score |
|---|---:|
| Accuracy | 2/2 |
| Completeness | 2/2 |
| Consistency | 2/2 |
| Business Relevance | 2/2 |
| Responsible AI | 2/2 |
| Total | 10/10 |

The v1.1 prompt achieved 30/30 across Test Cases
A, B and C.

These scores represent response quality against
the selected synthetic test criteria rather than
measured commercial forecasting performance.

### v1.2 — Additional Retest

Testing date: Pending.

AI tool and model: Pending.

Actual AI output:

Pending testing.

Observations:

Pending evaluation.

### Initial v1.2 Testing Procedure Review

The initial v1.2 testing attempt identified a
limitation in the testing procedure.

Expected test outcomes were supplied to the AI,
while the original input datasets were not
consistently reproduced.

Test Cases A and B referred to expected results
and previously supplied historical information.

Test Case C could not independently calculate
production requirements because the underlying
historical and operational data were unavailable.

However, the Test Case C response appropriately
identified missing information and avoided
fabricating production quantities.

### Evaluation Decision

The initial v1.2 runs are retained as development
evidence but excluded from the formal version
comparison.

No final evaluation scores have been assigned
to these runs.

### Corrective Action

Repeat all three test scenarios using:

- The exact v1.2 prompt.
- Complete original synthetic test inputs.
- Separate fresh AI conversations.
- The same AI model and settings where possible.
- No expected answers or evaluation benchmarks
  supplied to the AI.

### Lesson Learned

Reliable AI evaluation requires a controlled
testing procedure.

Providing expected answers before testing may
influence AI responses and reduce the validity
of the evaluation.

Missing test inputs may also prevent an otherwise
capable prompt from completing its intended task.

Expected results must therefore remain separate
from the actual AI testing instructions.

### Corrected v1.2 Retesting Status

Pending corrected testing.

---

## 10. Corrected v1.2 Retesting

### Testing Methodology

All three scenarios were repeated using the exact
v1.2 prompt and complete original synthetic input
data.

Expected results and evaluation benchmarks were
not supplied to the AI.

Each scenario was conducted in a separate fresh
conversation.

### Corrected Test A — Complete Historical Sales

Testing date: 25 November 2026

AI tool and model: ChatGPT

Input: Original Test Case A data.

#### Actual AI Output


# Flavors of Ceylon – Weekly Demand Forecast and Production Planning Report

## Test Information

| Item | Description |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Australian Food Manufacturing |
| Prompt ID | P01 |
| Prompt Version | v1.2 |
| Test Scenario | Test A – Complete Historical Sales Data (Retest) |
| Historical Period | Weeks 1–4 |
| Forecast Period | Week 5 |
| Forecasting Method | Simple Linear Trend Extrapolation |

---

## 1. Data Validation

The supplied historical sales data has been reviewed for completeness, consistency and reported operational disruptions.

| Product | Week 1 | Week 2 | Week 3 | Week 4 | Validation Status |
|---|---:|---:|---:|---:|---|
| Fish roti | 80 | 100 | 120 | 140 | Valid |
| Vegetable rolls | 120 | 110 | 100 | 90 | Valid |
| Chicken kottu | 50 | 60 | 70 | 80 | Valid |
| Rice and curry packs | 60 | 60 | 60 | 60 | Valid |
| Pol sambol sachets | 40 | 50 | 60 | 70 | Valid |

### Validation Findings

- All 20 historical sales records are available and valid.
- No missing, negative or inconsistent sales figures were identified.
- No stockouts or unusual promotional events were reported.
- All five products have four usable weekly observations.
- No historical records require exclusion.
- Historical figures represent recorded sales, while Week 5 forecasts represent estimated customer demand.

---

## 2. Demand Forecast and Calculation Breakdown

### Week 5 Demand Forecast

| Product | Usable Observations | Missing or Excluded Records | Average Weekly Change | Sales Trend | Week 5 Forecast (Units) | Data Reliability | Recommended Planning Action |
|---|---:|---|---:|---|---:|---|---|
| Fish roti | 4 | None | +20 | Increasing | 160 | High | Plan for higher demand |
| Vegetable rolls | 4 | None | -10 | Decreasing | 80 | High | Review production requirements to avoid excess inventory |
| Chicken kottu | 4 | None | +10 | Increasing | 90 | High | Prepare for increased demand |
| Rice and curry packs | 4 | None | 0 | Stable | 60 | High | Maintain the existing demand planning level |
| Pol sambol sachets | 4 | None | +10 | Increasing | 80 | High | Prepare for increased demand |
| **Total Estimated Demand** | | | | | **470** | | |

### Key Forecast Indicators

| Indicator | Result |
|---|---:|
| Week 4 recorded sales | 440 units |
| Week 5 estimated customer demand | 470 units |
| Estimated increase | 30 units |
| Estimated demand growth compared with Week 4 sales | 6.82% |
| Products with increasing sales trends | 3 |
| Products with decreasing sales trends | 1 |
| Products with stable sales trends | 1 |
| Products successfully forecasted | 5 out of 5 |

### Forecasting Formulas

**Average weekly change:**

```
Average weekly change =
(Latest usable sales - Earliest usable sales) / Number of elapsed weeks
```

**Target-week forecast:**

```
Forecast = Latest usable sales + (Average weekly change × Number of weeks until target week)
```

### Calculation Breakdown

| Product | Average Weekly Change Calculation | Week 5 Forecast Calculation | Final Forecast |
|---|---|---|---:|
| Fish roti | (140 - 80) / 3 = 20 | 140 + (20 × 1) | 160 |
| Vegetable rolls | (90 - 120) / 3 = -10 | 90 + (-10 × 1) | 80 |
| Chicken kottu | (80 - 50) / 3 = 10 | 80 + (10 × 1) | 90 |
| Rice and curry packs | (60 - 60) / 3 = 0 | 60 + (0 × 1) | 60 |
| Pol sambol sachets | (70 - 40) / 3 = 10 | 70 + (10 × 1) | 80 |

### Total Estimated Week 5 Demand

```
Total estimated demand = 160 + 80 + 90 + 60 + 80
                       = 470 units
```

### Estimated Demand Growth

```
Week 4 recorded sales = 140 + 90 + 80 + 60 + 70
                      = 440 units

Estimated growth = ((470 - 440) / 440) × 100
                 = 6.82%
```

All calculated forecasts are non-negative whole numbers. No rounding adjustments or zero-value corrections are required.

---

## 3. Production Planning and Capacity Analysis

Although demand forecasts are available for all products, the supplied information does not include:

- Usable finished-product inventory.
- Target safety stock levels.
- Product-specific production capacity.
- Shared production resource availability or other operational restrictions.

Therefore, required production and capacity-limited production cannot be verified.

### Production Planning Results

| Product | Forecast Demand | Usable Inventory | Target Safety Stock | Required Production | Available Capacity | Capacity-Limited Production | Production Shortfall | Estimated Demand Shortfall | Safety Stock Shortfall | Recommended Action |
|---|---:|---|---|---|---|---|---|---|---|---|
| Fish roti | 160 | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Verify operational inputs |
| Vegetable rolls | 80 | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Verify operational inputs |
| Chicken kottu | 90 | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Verify operational inputs |
| Rice and curry packs | 60 | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Verify operational inputs |
| Pol sambol sachets | 80 | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Verify operational inputs |

> **Production quantity pending verification.**

No missing operational values have been assumed to be zero.

Projected closing inventory cannot be calculated, and products requiring no additional production cannot yet be identified.

The forecast of 470 units represents estimated customer demand, not confirmed manufacturing requirements.

Production shortfalls, unmet customer demand and safety stock shortfalls cannot be determined until operational inputs are verified.

Unused production capacity must not be assumed to be transferable between products. Shared production resources and operational restrictions require management review before overall manufacturing feasibility can be confirmed.

---

## 4. Assumptions and Limitations

| Category | Assumption or Limitation |
|---|---|
| Data source | Only the supplied historical sales information has been used. |
| Forecasting period | Week 5 immediately follows Week 4. |
| Demand estimation | Recorded sales are used as a proxy for historical customer demand. |
| Trend continuation | Historical linear sales trends are assumed to continue into Week 5. |
| Historical coverage | Four weeks of historical data provide limited evidence of long-term demand behaviour. |
| Seasonality | The forecasting method does not account for seasonal changes. |
| Market conditions | Unexpected demand changes, competitor activities and future promotions are not incorporated. |
| Irregular patterns | No irregular sales patterns were identified within the supplied period. |
| Data reliability | High reliability reflects historical data completeness and quality, not statistical forecast confidence or guaranteed prediction accuracy. |
| Production feasibility | Inventory, safety stock, capacity and shared resource constraints remain unverified. |
| Human oversight | Forecasts and subsequent production calculations require production manager approval. |

---

## 5. Management Summary and Priority Actions

Flavors of Ceylon's estimated Week 5 customer demand is **470 units**, representing a **6.82% increase** compared with Week 4 recorded sales. Fish roti, chicken kottu and pol sambol sachets demonstrate increasing sales trends, while vegetable rolls show declining sales and rice and curry packs remain stable. All products have high data reliability.

### Priority Actions

1. Prioritise planning for products with increasing demand.
2. Review vegetable roll requirements to minimise potential waste.
3. Verify inventory levels and target safety stock.
4. Confirm product-specific capacity and shared resource constraints.
5. Obtain production manager approval before finalising manufacturing quantities.

---

**Final Status:** Demand forecasting completed successfully. Production quantities remain pending verification.

> **Disclaimer:** All outputs are indicative, intended for decision support and require production manager review before operational implementation.

#### Evaluation

The corrected v1.2 response successfully validated
all 20 historical sales records and calculated
accurate forecasts for all five products under
the specified forecasting method.

Total estimated demand was 470 units, representing
a projected increase of 6.82% compared with Week 4
recorded sales.

The response correctly withheld production quantities
because inventory, safety stock and production
capacity information were unavailable.

Evaluation score: 10/10.

Status: Passed.

---

### Corrected Test B — Incomplete Data and Stockouts

Testing date: 25 November 2026

AI tool and model: ChatGPT

Input: Original Test Case B data.

#### Actual AI Output


# Flavors of Ceylon – Week 5 Demand Forecast and Production Planning Report

## Test Information

| Item | Details |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Australian food manufacturing |
| Prompt ID | P01 |
| Prompt Version | v1.2 |
| Test Scenario | Test B – Retest |
| Scenario Description | Incomplete sales records and stockout conditions |
| Historical Period | Weeks 1–4 |
| Forecast Period | Week 5 |
| Forecasting Method | Simple linear trend extrapolation |

---

## 1. Data Validation

The supplied historical sales data were reviewed to identify missing records, stockout-affected observations and data reliability issues.

### Historical Sales Data

| Product | Week 1 | Week 2 | Week 3 | Week 4 | Usable Observations |
|---|---:|---:|---:|---:|---:|
| Fish roti | 80 | 100 | Missing | 140 | 3 |
| Vegetable rolls | 120 | 110 | 100 | 90 | 4 |
| Chicken kottu | 50 | 60 | 70 | 25 (Stockout) | 3 |
| Rice and curry packs | 60 | 60 | 60 | 60 | 4 |
| Pol sambol sachets | 40 | Missing | 60 | Missing | 2 |

### Data Validation Findings

| Product | Identified Issue | Validation Decision |
|---|---|---|
| Fish roti | Week 3 reporting system error | Exclude the missing observation without estimating its value. |
| Vegetable rolls | No identified data issues | Include all four observations. |
| Chicken kottu | Four-day stockout during Week 4 | Retain 25 units as recorded sales but exclude Week 4 from baseline forecasting. |
| Rice and curry packs | No identified data issues | Include all four observations. |
| Pol sambol sachets | Missing Week 2 and Week 4 records | Withhold the forecast because fewer than three usable observations are available. |

### Validation Summary

- Total expected historical records: 20
- Missing records: 3
- Stockout-affected records: 1
- Invalid numerical records identified: 0
- Total usable observations: 16
- Products eligible for forecasting: 4 out of 5

Recorded sales represent actual units sold and may not reflect unrestricted customer demand.

Missing records have not been replaced with zero or estimated historical values.

---

## 2. Demand Forecast and Calculation Breakdown

### Week 5 Demand Forecast

| Product | Usable Observations | Missing or Excluded Records | Average Weekly Change | Sales Trend | Week 5 Forecast (Units) | Data Reliability | Recommended Planning Action |
|---|---:|---|---:|---|---:|---|---|
| Fish roti | 3 | Week 3 missing | +20 | Increasing | 160 | Medium | Prepare for increasing demand. |
| Vegetable rolls | 4 | None | -10 | Decreasing | 80 | High | Reduce the demand planning target. |
| Chicken kottu | 3 | Week 4 stockout | +10 | Increasing | 90 | Medium | Review stock availability and replenishment. |
| Rice and curry packs | 4 | None | 0 | Stable | 60 | High | Maintain the existing demand planning target. |
| Pol sambol sachets | 2 | Weeks 2 and 4 missing | N/A | Undetermined | Withheld | Insufficient | Recover missing sales records. |
| **Forecasted Subtotal** | | | | | **390** | | |

> **Important:** The subtotal of 390 units is not the total business demand because the pol sambol sachets forecast has been withheld.

### Forecast Calculation Methodology

**Average weekly change:**

```text
Average weekly change =
(Latest usable sales - Earliest usable sales)
/ Number of elapsed weeks
```

**Target-week forecast:**

```text
Forecast demand =
Latest usable sales +
(Average weekly change × Weeks to target)
```

### 2.1 Fish Roti

- Usable observations: Weeks 1, 2 and 4
- Earliest usable sales: 80 units
- Latest usable sales: 140 units
- Elapsed weeks: 4 - 1 = 3
- Weeks to target: 5 - 4 = 1

**Average weekly change:**

```text
(140 - 80) / 3 = 20 units per week
```

**Week 5 forecast:**

```text
140 + (20 × 1) = 160 units
```

**Estimated demand: 160 units**

Week 3 remains missing. The calculation uses actual elapsed weeks rather than the number of available observations.

### 2.2 Vegetable Rolls

- Usable observations: Weeks 1, 2, 3 and 4
- Earliest usable sales: 120 units
- Latest usable sales: 90 units
- Elapsed weeks: 4 - 1 = 3
- Weeks to target: 5 - 4 = 1

**Average weekly change:**

```text
(90 - 120) / 3 = -10 units per week
```

**Week 5 forecast:**

```text
90 + (-10 × 1) = 80 units
```

**Estimated demand: 80 units**

### 2.3 Chicken Kottu

- Usable observations: Weeks 1, 2 and 3
- Earliest usable sales: 50 units
- Latest usable sales: 70 units
- Elapsed weeks: 3 - 1 = 2
- Weeks to target: 5 - 3 = 2

**Average weekly change:**

```text
(70 - 50) / 2 = 10 units per week
```

**Week 5 forecast:**

```text
70 + (10 × 2) = 90 units
```

**Estimated demand: 90 units**

Week 4 recorded sales of 25 units are excluded because of the reported four-day stockout.

The forecast does not estimate or replace Week 4 historical sales.

### 2.4 Rice and Curry Packs

- Usable observations: Weeks 1, 2, 3 and 4
- Earliest usable sales: 60 units
- Latest usable sales: 60 units
- Elapsed weeks: 4 - 1 = 3
- Weeks to target: 5 - 4 = 1

**Average weekly change:**

```text
(60 - 60) / 3 = 0 units per week
```

**Week 5 forecast:**

```text
60 + (0 × 1) = 60 units
```

**Estimated demand: 60 units**

### 2.5 Pol Sambol Sachets

- Usable observations: Weeks 1 and 3
- Week 1 recorded sales: 40 units
- Week 3 recorded sales: 60 units
- Missing observations: Weeks 2 and 4
- Minimum required observations: 3
- Available usable observations: 2

**Insufficient data — forecast withheld.**

No numerical forecast or sales trend calculation is provided because the minimum data requirement has not been satisfied.

### Forecasted Demand Subtotal

```text
160 + 80 + 90 + 60 = 390 units
```

**Forecasted demand subtotal: 390 units**

**Products successfully forecasted: 4 out of 5**

All calculated forecasts are non-negative whole numbers. No rounding adjustments or negative forecast corrections are required.

The subtotal excludes pol sambol sachets and does not represent total business demand.

---

## 3. Production Planning and Capacity Analysis

The supplied information contains historical sales figures but does not provide verified operational information regarding:

- Usable finished-product inventory.
- Target safety stock.
- Product-specific production capacity.
- Shared production resources or operational restrictions.

Consequently, estimated customer demand cannot be converted into confirmed production quantities.

### Production Planning Results

| Product | Forecast Demand | Usable Inventory | Target Safety Stock | Required Production | Available Capacity | Capacity-Limited Production | Production Shortfall | Estimated Demand Shortfall | Safety Stock Shortfall | Recommended Action |
|---|---:|---|---|---|---|---|---|---|---|---|
| Fish roti | 160 | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Verify operational inputs. |
| Vegetable rolls | 80 | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Verify inventory and capacity. |
| Chicken kottu | 90 | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Prioritise stock and capacity verification. |
| Rice and curry packs | 60 | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Review existing inventory. |
| Pol sambol sachets | Withheld | Not supplied | Not supplied | Pending | Not supplied | Pending | Pending | Pending | Pending | Recover sales and operational records. |

> **Production quantity pending verification.**
>
> This status applies to all five products.

### Production Planning Safeguards

| Operational Consideration | Assessment |
|---|---|
| Required production | Cannot be calculated without inventory and safety stock information. |
| Capacity-limited production | Cannot be calculated without verified product-specific capacity. |
| Production shortfall | Cannot be determined. |
| Estimated customer demand shortfall | Cannot be determined. |
| Projected closing inventory | Cannot be calculated. |
| Safety stock shortfall | Cannot be determined and must be assessed separately from unmet customer demand. |
| Products requiring no additional production | None can be confirmed from the supplied information. |
| Shared production resources | Not specified; management verification is required. |
| Capacity transfers between products | No transfers assumed. |

The forecasted subtotal of 390 units represents estimated customer demand for four products, not a recommended manufacturing quantity or confirmed production schedule.

---

## 4. Assumptions and Limitations

| Factor | Assumption or Limitation |
|---|---|
| Data source | Only supplied historical business information has been used. |
| Forecasting method | Historical endpoint trends are assumed to continue into Week 5. |
| Missing data | Missing observations are neither treated as zero nor estimated. |
| Stockout impact | Chicken kottu Week 4 sales are considered unsuitable for unrestricted demand forecasting. Actual lost demand is unknown. |
| Promotional activities | No promotional information is supplied. Promotional effects cannot be assessed. |
| Seasonality | The forecasting method does not account for seasonal demand changes. |
| Historical period | Four weeks provide limited evidence of longer-term demand behaviour. |
| Irregular sales patterns | Chicken kottu Week 4 sales decline is associated with a reported stockout. No other irregularities are apparent in the usable observations, although missing data limit assessment. |
| Data reliability | High, Medium and Insufficient classifications describe data availability and quality, not statistical forecast confidence or guaranteed prediction accuracy. |
| Unexpected market changes | The forecasting method does not account for unexpected changes in customer demand or market conditions. |
| Operational feasibility | Manufacturing feasibility cannot be confirmed without verified operational information. |
| Human oversight | All forecasts and future production quantities require production manager review and approval. |

---

## 5. Management Summary and Priority Actions

Week 5 estimated demand is 390 units across four forecasted products. Fish roti and chicken kottu show increasing trends, vegetable rolls show declining sales, and rice and curry packs remain stable. The pol sambol sachets forecast is withheld due to insufficient data. Production quantities cannot be confirmed without verified operational inputs.

### Priority Actions

1. Prepare for increased fish roti and chicken kottu demand.
2. Adjust vegetable roll demand planning to 80 units.
3. Maintain the rice and curry demand target of 60 units.
4. Recover missing pol sambol and fish roti sales records.
5. Verify inventory, safety stock, production capacity and shared resource restrictions before approving manufacturing schedules.

---

**Final Assessment:** Demand forecasting completed for four products. Production planning remains pending verification.

**Approval Requirement:** All outputs are for decision support and require production manager review before operational implementation.

#### Evaluation

The corrected response identified three missing
sales records and one stockout-affected record,
leaving 16 usable historical observations.

The response correctly withheld the pol sambol
forecast and calculated a partial demand subtotal
of 390 units across four products.

Missing values were not invented or treated as zero.

Production quantities remained pending verification
because the necessary operational information was
unavailable.

Evaluation score: 10/10.

Status: Passed.

---

### Corrected Test C — Inventory and Capacity Constraints

Testing date: 25 November 2026

AI tool and model: ChatGPT

Input: Original Test Case C data.

#### Actual AI Output

# Flavors of Ceylon – Week 5 Demand Forecast and Production Planning Report

## Test Information

| Item | Description |
|---|---|
| Business | Flavors of Ceylon |
| Industry | Australian Food Manufacturing |
| Prompt ID | P01 |
| Prompt Version | v1.2 |
| Test Scenario | Test C – Retest |
| Forecast Period | Week 5 |
| Forecasting Method | Simple Linear Trend Extrapolation |
| Data Status | Synthetic and verified for testing purposes |
| Purpose | Demand forecasting and production planning |

---

## 1. Data Validation

The supplied historical sales and operational information have been reviewed before forecasting and production planning.

### 1.1 Historical Weekly Sales

| Product | Week 1 | Week 2 | Week 3 | Week 4 |
|---|---:|---:|---:|---:|
| Fish roti | 80 | 100 | 120 | 140 |
| Vegetable rolls | 120 | 110 | 100 | 90 |
| Chicken kottu | 50 | 60 | 70 | 80 |
| Rice and curry packs | 60 | 60 | 60 | 60 |
| Pol sambol sachets | 40 | 50 | 60 | 70 |

### 1.2 Verified Operational Information

| Product | Usable Inventory | Target Safety Stock | Weekly Production Capacity |
|---|---:|---:|---:|
| Fish roti | 30 | 10 | 120 |
| Vegetable rolls | 90 | 5 | 60 |
| Chicken kottu | 10 | 5 | 100 |
| Rice and curry packs | 20 | 10 | 60 |
| Pol sambol sachets | 15 | 5 | 70 |

### 1.3 Data Validation Results

| Validation Criteria | Findings | Status |
|---|---|---|
| Historical sales records | All 20 records are available | Pass |
| Missing sales records | None | Pass |
| Invalid or inconsistent records | None identified | Pass |
| Stockout-affected records | None reported | Pass |
| Unusual promotional events | None reported | Pass |
| Operational information | Complete for all five products | Pass |
| Measurement units | Consistently expressed in units | Pass |
| Shared resource constraints | None reported | Pass |
| Negative operational values | None identified | Pass |

All five products have four usable historical weekly observations. No historical records require exclusion, correction or estimation.

Historical sales represent recorded units sold, whereas Week 5 forecasts represent estimated customer demand.

---

## 2. Demand Forecast and Calculation Breakdown

### 2.1 Demand Forecast Results

| Product | Usable Observations | Missing or Excluded Records | Average Weekly Change | Sales Trend | Week 5 Forecast (Units) | Data Reliability | Recommended Planning Action |
|---|---:|---|---:|---|---:|---|---|
| Fish roti | 4 | None | +20 | Increasing | 160 | High | Prioritise growing demand |
| Vegetable rolls | 4 | None | -10 | Decreasing | 80 | High | Reduce production requirements |
| Chicken kottu | 4 | None | +10 | Increasing | 90 | High | Plan for increased demand |
| Rice and curry packs | 4 | None | 0 | Stable | 60 | High | Maintain stable supply |
| Pol sambol sachets | 4 | None | +10 | Increasing | 80 | High | Plan for increased demand |
| **Total** | **20** | **None** | **+30** | **Increasing** | **470** | — | — |

### 2.2 Demand Forecast Overview

| Key Performance Indicator | Result |
|---|---:|
| Total estimated Week 5 demand | 470 units |
| Products with increasing sales trends | 3 |
| Products with decreasing sales trends | 1 |
| Products with stable sales trends | 1 |
| Products with undetermined sales trends | 0 |
| Products with high data reliability | 5 |
| Forecasts withheld | 0 |

### 2.3 Forecasting Formulas

**Average weekly change:**

$$
\text{Average Weekly Change} =
\frac{\text{Latest Usable Sales} - \text{Earliest Usable Sales}}
{\text{Number of Elapsed Weeks}}
$$

**Target-week forecast:**

$$
\text{Forecast} = L + (C \times N)
$$

Where:

- L = Latest usable weekly sales.
- C = Average weekly change.
- N = Number of weeks between the latest usable observation and the target week.

The elapsed period between Week 1 and Week 4 is three weeks.

The forecast period between Week 4 and Week 5 is one week.

### 2.4 Individual Product Calculations

| Product | Average Weekly Change Calculation | Week 5 Forecast Calculation | Final Forecast |
|---|---|---|---:|
| Fish roti | (140 - 80) / 3 = +20 | 140 + (20 x 1) | 160 |
| Vegetable rolls | (90 - 120) / 3 = -10 | 90 + (-10 x 1) | 80 |
| Chicken kottu | (80 - 50) / 3 = +10 | 80 + (10 x 1) | 90 |
| Rice and curry packs | (60 - 60) / 3 = 0 | 60 + (0 x 1) | 60 |
| Pol sambol sachets | (70 - 40) / 3 = +10 | 70 + (10 x 1) | 80 |

### 2.5 Total Estimated Demand

$$
160 + 80 + 90 + 60 + 80 = 470
$$

**Total estimated Week 5 customer demand = 470 units.**

All forecasts are non-negative whole units. No rounding adjustments or forecast withdrawals are required.

---

## 3. Production Planning and Capacity Analysis

### 3.1 Production Planning Results

All quantities are expressed in units.

| Product | Forecast Demand | Usable Inventory | Target Safety Stock | Required Production | Available Capacity | Capacity-Limited Production | Production Shortfall | Estimated Demand Shortfall | Safety Stock Shortfall | Recommended Action |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---|
| Fish roti | 160 | 30 | 10 | 140 | 120 | 120 | 20 | 10 | 10 | Review capacity shortage |
| Vegetable rolls | 80 | 90 | 5 | 0 | 60 | 0 | 0 | 0 | 0 | No additional production |
| Chicken kottu | 90 | 10 | 5 | 85 | 100 | 85 | 0 | 0 | 0 | Produce 85 units |
| Rice and curry packs | 60 | 20 | 10 | 50 | 60 | 50 | 0 | 0 | 0 | Produce 50 units |
| Pol sambol sachets | 80 | 15 | 5 | 70 | 70 | 70 | 0 | 0 | 0 | Produce 70 units |
| **Total** | **470** | **165** | **35** | **345** | **410** | **325** | **20** | **10** | **10** | — |

### 3.2 Production Planning Overview

| Key Performance Indicator | Result |
|---|---:|
| Estimated customer demand | 470 units |
| Usable opening inventory | 165 units |
| Target safety stock | 35 units |
| Required production | 345 units |
| Total product-specific production capacity | 410 units |
| Capacity-limited production | 325 units |
| Production shortfall | 20 units |
| Estimated customer demand shortfall | 10 units |
| Safety stock shortfall | 10 units |
| Projected closing inventory | 30 units |
| Estimated customer demand fulfilled | 460 units |

### 3.3 Production Planning Formulas

**Required production:**

$$
\max(0,\text{Forecast Demand}+\text{Target Safety Stock}-\text{Usable Inventory})
$$

**Capacity-limited production:**

$$
\min(\text{Required Production},\text{Available Capacity})
$$

**Production shortfall:**

$$
\text{Required Production}-\text{Capacity-Limited Production}
$$

**Estimated demand shortfall:**

$$
\max(0,\text{Forecast Demand}-\text{Usable Inventory}-\text{Capacity-Limited Production})
$$

**Projected closing inventory:**

$$
\max(0,\text{Usable Inventory}+\text{Capacity-Limited Production}-\text{Forecast Demand})
$$

**Safety stock shortfall:**

$$
\max(0,\text{Target Safety Stock}-\text{Projected Closing Inventory})
$$

### 3.4 Required Production and Capacity Calculations

| Product | Required Production Calculation | Capacity-Limited Production Calculation | Production Shortfall |
|---|---|---|---:|
| Fish roti | Max(0, 160 + 10 - 30) = 140 | Min(140, 120) = 120 | 20 |
| Vegetable rolls | Max(0, 80 + 5 - 90) = 0 | Min(0, 60) = 0 | 0 |
| Chicken kottu | Max(0, 90 + 5 - 10) = 85 | Min(85, 100) = 85 | 0 |
| Rice and curry packs | Max(0, 60 + 10 - 20) = 50 | Min(50, 60) = 50 | 0 |
| Pol sambol sachets | Max(0, 80 + 5 - 15) = 70 | Min(70, 70) = 70 | 0 |
| **Total** | **345 units** | **325 units** | **20** |

### 3.5 Demand Fulfilment and Closing Inventory Calculations

| Product | Estimated Demand Shortfall | Projected Closing Inventory | Safety Stock Shortfall |
|---|---|---|---|
| Fish roti | Max(0, 160 - 30 - 120) = 10 | Max(0, 30 + 120 - 160) = 0 | Max(0, 10 - 0) = 10 |
| Vegetable rolls | Max(0, 80 - 90 - 0) = 0 | Max(0, 90 + 0 - 80) = 10 | Max(0, 5 - 10) = 0 |
| Chicken kottu | Max(0, 90 - 10 - 85) = 0 | Max(0, 10 + 85 - 90) = 5 | Max(0, 5 - 5) = 0 |
| Rice and curry packs | Max(0, 60 - 20 - 50) = 0 | Max(0, 20 + 50 - 60) = 10 | Max(0, 10 - 10) = 0 |
| Pol sambol sachets | Max(0, 80 - 15 - 70) = 0 | Max(0, 15 + 70 - 80) = 5 | Max(0, 5 - 5) = 0 |
| **Total** | **10 units** | **30 units** | **10 units** |

### 3.6 Operational Findings

#### Fish Roti – Capacity Constraint

Fish roti requires 140 units of additional production, but its weekly production capacity is limited to 120 units.

The resulting production shortfall of 20 units consists of:

- 10 units of estimated unmet customer demand.
- 10 units of unmet target safety stock.

> **Management Warning:** Fish roti production capacity is insufficient to satisfy forecast customer demand and achieve the target safety stock.

#### Vegetable Rolls – No Additional Production Required

The existing inventory of 90 units is sufficient to satisfy forecast demand of 80 units and the target safety stock of 5 units.

The projected closing inventory is 10 units.

No additional production is recommended.

#### Chicken Kottu – Sufficient Production Capacity

The required production of 85 units is within the available weekly capacity of 100 units.

Forecast customer demand and target safety stock can both be satisfied.

#### Rice and Curry Packs – Stable Production Requirements

The required production of 50 units is within the available weekly capacity of 60 units.

Forecast customer demand and target safety stock can both be satisfied.

#### Pol Sambol Sachets – Full Capacity Utilisation

The required production of 70 units equals the available weekly production capacity.

There is no remaining product-specific production capacity for unexpected additional demand.

#### Production Capacity Safeguard

Although combined production capacity is 410 units, unused capacity from other products cannot be assumed to resolve the fish roti capacity shortage.

No shared resource constraints or other operational restrictions are reported. Actual manufacturing feasibility remains subject to management review.

---

## 4. Assumptions and Limitations

| Category | Assumption or Limitation |
|---|---|
| Data source | Only the supplied synthetic business information has been used. |
| Historical sales | Recorded sales are used as the basis for estimating future demand. |
| Forecasting method | Historical linear sales trends are assumed to continue into Week 5. |
| Historical period | Four weeks of observations provide a limited forecasting history. |
| Irregular sales patterns | None identified in the supplied historical records. |
| Seasonality | Seasonal demand changes are not incorporated. |
| Market uncertainty | Unexpected demand changes and external market conditions are not incorporated. |
| Data reliability | High reliability indicates complete usable historical records, not statistical forecast confidence or guaranteed prediction accuracy. |
| Inventory | Supplied opening inventory is assumed usable and available to meet Week 5 demand. |
| Production capacity | Product-specific capacities are treated as independent weekly limits. |
| Capacity transfer | Unused capacity cannot be assumed to be transferable between products. |
| Operational restrictions | No shared resource constraints are reported; management must confirm actual feasibility. |
| Human oversight | All forecasts and production quantities require production manager approval. |

---

## 5. Management Summary and Priority Actions

Total Week 5 estimated demand is **470 units**, requiring **345 units** of additional production. Product-specific capacity limits reduce indicative production to **325 units**.

Fish roti is the only product with a production shortfall, resulting in 10 units of estimated unmet customer demand and 10 units of safety stock shortfall.

All products have high data reliability, although forecast accuracy is not guaranteed.

### Priority Actions

1. Investigate additional fish roti production capacity.
2. Prioritise customer demand before rebuilding fish roti safety stock.
3. Avoid unnecessary vegetable roll production.
4. Monitor pol sambol sachets operating at full production capacity.
5. Review and approve indicative production quantities before implementation.

---

**Final Assessment:** All five demand forecasts and production planning calculations have been completed using the supplied verified synthetic data. No missing information prevents numerical forecasting or indicative production planning.

> **Disclaimer:** This report is for decision support only. All estimated demand forecasts and indicative production quantities require production manager review and approval before operational implementation.

---

#### Evaluation

The corrected response successfully calculated:

- Estimated demand: 470 units.
- Required production: 345 units.
- Capacity-limited production: 325 units.
- Production shortfall: 20 units.
- Estimated customer demand shortfall: 10 units.
- Safety stock shortfall: 10 units.
- Projected closing inventory: 30 units.
- Estimated customer demand fulfilled: 460 units.

All calculations matched the independently
established evaluation benchmarks.

The response correctly identified the fish roti
capacity constraint and recognised that vegetable
rolls required no additional production.

Product-specific capacity limits and management
approval requirements were maintained.

Evaluation score: 10/10.

Status: Passed.

---

### Final Retesting Conclusion

All three corrected v1.2 tests were successfully
completed using the original synthetic datasets
without supplying expected numerical answers.

| Evaluation Criterion | Test A | Test B | Test C |
|---|---:|---:|---:|
| Accuracy | 2 | 2 | 2 |
| Completeness | 2 | 2 | 2 |
| Consistency | 2 | 2 | 2 |
| Business Relevance | 2 | 2 | 2 |
| Responsible AI | 2 | 2 | 2 |
| Total | 10/10 | 10/10 | 10/10 |

Combined final evaluation score: 30/30 (100%).

The comparable score across the two original
scenarios improved from 16/20 in v1.0 to
20/20 in v1.2.

The final version retained the successful v1.1
forecasting and data validation safeguards while
introducing standardised production capacity
and shortfall calculations.

The corrected outputs used the requested five
principal reporting sections and did not contain
unrequested charts.

Some repetition remains, and further testing
would be required to evaluate irregular demand,
invalid operational inputs, shared production
constraints and repeat-run reliability.

The initial v1.2 testing attempts remain excluded
from the formal evaluation because of test
input limitations.

Final selected version: v1.2.

Testing status: Completed for the selected scenarios.

These results measure AI response quality under
controlled synthetic scenarios, not actual
commercial forecasting accuracy.

## Final Evaluation

- [P01 Final Evaluation](../05-evaluation/P01-final-evaluation.md)
