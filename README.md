
# 🏡 Predicting US House Prices (2003–2023)

This project explores the key macroeconomic, demographic, and financial factors that have influenced U.S. housing prices over the last two decades. Using publicly available datasets from the Federal Reserve Economic Data (FRED), the goal was to analyze patterns, visualize trends, and build predictive models for housing price forecasting.

---

## 📚 Table of Contents

1. [Introduction](#-introduction)
2. [Dataset](#-dataset)
3. [Data Preprocessing](#-data-preprocessing)
4. [Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
5. [Data Visualization](#-data-visualization)
6. [Model Building](#-model-building)
7. [Model Evaluation](#-model-evaluation)
8. [Conclusion](#-conclusion)
9. [Next Steps](#-next-steps)
10. [Dependencies](#-dependencies)
11. [References](#-references)

---

## 📌 Introduction

The goal of this project is to predict U.S. housing prices from 2003 to 2023 and identify key influencing factors such as interest rates, GDP, personal income, unemployment rates, and more. The project balances interpretability and predictive performance by employing both linear regression and XGBoost.

---

## 🗂️ Dataset

* Timeframe: 2003 to 2023
* Source: [FRED](https://fred.stlouisfed.org/)
* Key Features:

  * House Price Index
  * Per Capita GDP
  * Personal Income
  * Interest Rates (Federal Funds Rate, Mortgage Rate)
  * Unemployment Rate
  * Construction Spending
  * Total Housing Units, Total Households
  * Energy Index

---

## 🧹 Data Preprocessing

* Filtered data from 2003 onward
* Applied forward fill and interpolation for missing values
* Resampled quarterly data to monthly frequency
* Normalized and aligned feature columns for modeling

---

## 📊 Exploratory Data Analysis (EDA)

* Found strong correlation between GDP and personal income
* Detected seasonal patterns in construction activity
* Observed the influence of interest rate fluctuations on housing prices

---

## 📈 Data Visualization

* Time-series plots for major indicators
* Correlation heatmaps to uncover relationships
* Scatter plots to visualize price interactions with key features

---

## 🧠 Model Building

* **Linear Regression** for interpretability
* **XGBoost Regressor** for high-performance, non-linear modeling
* Final model selection: Linear Regression (for transparency)

---

## 🧪 Model Evaluation

**Top Linear Regression Coefficients:**

* Construction Spending: +34.15
* Per Capita GDP: +13.68
* Working Population: -8.10
* Personal Saving Rate: -4.26
* Mortgage Rate (15Y): +1.59

**XGBoost Top Features (by importance):**

1. Total Households
2. Construction Spending
3. Per Capita GDP
4. Personal Saving Rate
5. Unemployment Rate

---

## ✅ Conclusion

* **Key Drivers:** GDP, interest rates, energy prices, and construction activity
* **Model Insight:** Linear Regression offered interpretable coefficients; XGBoost captured complex patterns
* **Business Takeaway:** Economic health, labor force, and construction metrics directly shape real estate trends

---

## 🔮 Next Steps

* Apply advanced time series models like ARIMA or LSTM
* Introduce regional-level data granularity
* Analyze the impact of policy changes (e.g., rate hikes or stimulus packages)

## 📚 References

* [FRED - Economic Data](https://fred.stlouisfed.org/)
* [Research Paper on Housing Price Drivers](https://www.researchgate.net/publication/333855171_Driving_forces_for_the_US_residential_housing_price_a_predictive_analysis)

