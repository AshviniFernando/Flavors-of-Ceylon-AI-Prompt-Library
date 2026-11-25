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
| Testing Status | Pending |

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

Pending.

### Test Case A — Actual AI Output

Pending.

### Test Case B — Actual AI Output

Pending.

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
