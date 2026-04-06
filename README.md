# M5 Forecasting Accuracy Project

## Problem

The goal of this project is to build an accurate demand forecasting system using Walmart’s historical sales data from the M5 Forecasting Accuracy competition. The objective is to predict future sales at various hierarchical levels (item, store, state) while handling challenges like seasonality, sparsity, and external factors.

---

## Data

The dataset consists of:

* **Sales Data**: Daily unit sales for 30,000+ items across multiple stores
* **Calendar Data**: Information on dates, events, SNAP days, and holidays
* **Sell Prices**: Weekly pricing data for each item-store combination

Key challenges:

* High dimensionality (time series × items × stores)
* Intermittent demand
* External influence (events, promotions, SNAP)

---

## Approach

Current progress focuses on **data understanding and feature engineering**:

1. **Data Transformation**

   * Converted wide format sales data into long format
   * Merged with calendar and price datasets

2. **Data Cleaning**

   * Handled missing values in price and calendar features
   * Checked for inconsistencies across joins

3. **Feature Engineering**

   * Time-based features (day, week, month, year)
   * Event-based features (holidays, SNAP days)
   * Lag features (planned for next steps)

4. **Exploratory Data Analysis**

   * Sales distribution analysis
   * Trend and seasonality inspection

5. **Feature Correlation Analysis**

   * Identified relationships between engineered features and sales
   * Evaluated feature importance directionally for modeling

---

## Result

* Successfully built a **clean, merged dataset** ready for modeling
* Identified **key drivers of demand patterns** through correlation analysis
* Established a **scalable preprocessing pipeline** for further experimentation

(Current stage: Pre-modeling / Feature Engineering)

---

## Next Steps

1. Build baseline models:

   * Naive forecast
   * Moving average

2. Advanced modeling:

   * Tree-based models (XGBoost / LightGBM)
   * Deep learning models (LSTM)

3. Feature enhancement:

   * Lag features (t-7, t-28)
   * Rolling statistics (mean, std)
   * Price elasticity features

4. Evaluation:

   * Implement WRMSSE metric (competition standard)

5. Deployment:

   * Build batch prediction pipeline
   * Visualize forecasts using Tableau

---

## GitHub Repository

Add your repository link here:

```
[https://github.com/yourusername/retail-demand-forecasting](https://github.com/majesty594/Retail_Demand_Forecasting/)
```
