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

# **Flavors of Ceylon – Week 5 Demand Forecast**

## **1. Demand analysis and production recommendations**

Based on the supplied historical sales data, the **linear trend forecasting method** has been selected to estimate Week 5 demand by calculating the average weekly change in units sold.

| Product              | Week 4 sales | Weekly change | Demand trend   | Week 5 forecast | Recommended production |
| -------------------- | ------------ | ------------- | -------------- | --------------- | ---------------------- |
| Fish roti            | 140          | +20           | Increasing ↑   | 160             | 160                    |
| Vegetable rolls      | 90           | −10           | Decreasing ↓   | 80              | 80                     |
| Chicken kottu        | 80           | +10           | Increasing ↑   | 90              | 90                     |
| Rice and curry packs | 60           | 0             | Stable →       | 60              | 60                     |
| Pol sambol sachets   | 70           | +10           | Increasing ↑   | 80              | 80                     |
| **Total**            | **440**      | **+30**       | **Increasing** | **470**         | **470**                |

## **2. Product demand trends**

Week 5 forecast

# **470 units**

↑ 6.82% compared to Week 4

Increasing demand

# **3 of 5**

Products

Fish rotiVegetable rollsChicken kottuRice and curryPol sambol

04590135180Week 1Week 2Week 3Week 4Week 5 (Forecast)

Weeks 1–4: historical sales. Week 5: estimated demand.

## **3. Reasons for production recommendations**

| Product              | Reason for recommendation                                                                            |
| -------------------- | ---------------------------------------------------------------------------------------------------- |
| Fish roti            | Demand consistently increases by 20 units each week. Increase production to satisfy growing demand.  |
| Vegetable rolls      | Sales decrease by 10 units each week. Reduce production to minimise excess inventory and food waste. |
| Chicken kottu        | Consistent growth of 10 units per week supports increased production.                                |
| Rice and curry packs | Demand remains unchanged throughout the four weeks. Maintain the existing production quantity.       |
| Pol sambol sachets   | Sales increase by 10 units each week, indicating a positive demand trend.                            |

## **4. Forecasting method**

**Formula:**

Week 5 forecast = Week 4 sales + Average weekly change

For example, Fish roti:

\\[ \text{Average weekly change}=\frac{140-80}{3}=20 \\]

\\[ \text{Week 5 forecast}=140+20=160 \\]

## **5. Assumptions and limitations**

- Historical sales accurately represent customer demand because no stock shortages were reported.
- Existing demand trends will continue during Week 5.
- No unusual promotional activities, price changes or external market disruptions will occur during Week 5.
- No opening inventory or safety stock requirements have been provided. Therefore, recommended production quantities equal forecast demand.
- Four weeks of historical data may not be sufficient to identify seasonality or long-term changes in customer preferences.

## **6. Final recommendation**

Flavors of Ceylon should plan to produce **470 units for Week 5**, representing a 6.82% increase compared to Week 4 sales. The production manager should prioritise fish roti, chicken kottu and pol sambol sachets while reducing vegetable roll production to minimise food waste.

The forecast should be reviewed against actual sales and available inventory before finalising production schedules. All estimates are based exclusively on the supplied business data.

### Test Case B — Actual AI Output

# **Flavors of Ceylon – Week 5 Demand Forecast**

## **1. Demand analysis and production recommendations**

The historical sales data has been analysed using a linear trend forecasting approach. Missing sales records and stock shortages have been considered to avoid inaccurate demand estimates and inappropriate production decisions.

| Product              | Week 1 | Week 2  | Week 3  | Week 4  | Week 5 forecast | Demand trend             | Recommended production | Forecast confidence |
| -------------------- | ------ | ------- | ------- | ------- | --------------- | ------------------------ | ---------------------- | ------------------- |
| Fish roti            | 80     | 100     | Missing | 140     | 160             | ↑ Increasing             | 160                    | Medium              |
| Vegetable rolls      | 120    | 110     | 100     | 90      | 80              | ↓ Decreasing             | 80                     | High                |
| Chicken kottu        | 50     | 60      | 70      | 25      | 90              | ↑ Likely increasing      | 90                     | Medium              |
| Rice and curry packs | 60     | 60      | 60      | 60      | 60              | Stable                   | 60                     | High                |
| Pol sambol sachets   | 40     | Missing | 60      | Missing | 80              | ↑ Potentially increasing | 80                     | Low                 |
| **Total**            | —      | —       | —       | —       | **470**         | —                        | **470**                | —                   |

*All quantities are expressed in units. Confidence ratings are qualitative assessments based on data completeness and consistency.*

## **2. Week 5 demand forecast**

Total estimated demand

# **470 units**

Fish roti

160 units

Vegetable rolls

80 units

Chicken kottu

90 units

Rice and curry packs

60 units

Pol sambol sachets

80 units

Increasing

Decreasing

Stable

## **3. Reasons behind production recommendations**

| Product                  | Reason for recommendation                                                                                                                                                            |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Fish roti**            | Available sales indicate an increase of 20 units per week. Week 3 is estimated at 120 units, supporting a Week 5 forecast of 160 units.                                              |
| **Vegetable rolls**      | Sales consistently decline by 10 units each week. Reducing production to 80 units could minimise excess inventory and food waste.                                                    |
| **Chicken kottu**        | Week 4 sales were affected by a four-day stock shortage rather than necessarily a decline in demand. The previous growth trend of 10 units per week supports a forecast of 90 units. |
| **Rice and curry packs** | Sales remain consistent at 60 units every week. Maintaining the existing production quantity is appropriate.                                                                         |
| **Pol sambol sachets**   | Available records suggest an average increase of 10 units per week. However, missing records reduce forecast reliability. The estimated 80 units should be treated as provisional.   |

## **4. Assumptions and limitations**

- Missing sales records are treated as unavailable data, not zero sales.
- Historical demand trends are assumed to continue into Week 5.
- Chicken kottu is assumed to be available throughout Week 5.
- No promotional impact is included because promotional information is unavailable.
- Production recommendations assume no opening inventory and sufficient production capacity.
- Only four weeks of historical data are available, limiting forecast reliability.

## **5. Final recommendation**

Flavors of Ceylon should provisionally plan to produce **470 units for Week 5**, prioritising fish roti and chicken kottu while reducing vegetable roll production to minimise food waste.

The production manager should verify missing sales records, monitor product availability and review actual customer demand before approving final production quantities. Particular attention should be given to pol sambol sachets due to incomplete sales records.

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

Pending.

### Test Case A — Actual AI Output

Pending.

### Test Case B — Actual AI Output

Pending.

### Observed Improvements

Pending.

### Remaining Limitations

Pending.

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
