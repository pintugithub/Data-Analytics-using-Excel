# Forecasting Investment Opportunities in Australian Clearing Banks Using VAR Modeling

This project applies a multivariate time series analysis using the **Vector Autoregression (VAR)** model to forecast the investment potential of four major Australian clearing banks: **ANZ**, **CBA**, **NAB**, and **WESTPAC**. The objective is to determine which bank's stock is most suitable for a **one-year investment**, based on historical trends in stock prices and traded volumes.

##  Project Overview

## Dataset

- **Source**: [Investing.com](https://www.investing.com/)
- **Variables**:  
  - Daily stock prices: Open, High, Low, Close  
  - Traded volumes  
  - Daily returns (log-transformed)
- **Time Period**: 2010–2025  
- **Frequency**: Daily

---

## Methodology

### 1. Data Preprocessing
- Calculated log-returns to ensure stationarity.
- Handled missing values and normalized variables.
- Plotted individual time series and generated descriptive statistics.

### 2. Forecasting Approach
- Chose **Vector Autoregression (VAR)** for modeling causality between share prices and trading volumes.
- Included lagged variables to enhance prediction accuracy.
- Generated one-year forecasts for all four banks.

### 3. Model Evaluation
- Evaluated using:
  - **R²** (Coefficient of Determination)
  - **RMSE** (Root Mean Square Error)
- Plots comparing actual vs forecasted values.

---

## Results Summary

| Bank     | R² Value | RMSE     | Investment Insight                     |
|----------|----------|----------|----------------------------------------|
| **NAB**      | 57.9%    | 0.0107   | **Most promising investment candidate** |
| **WESTPAC**  | 50.4%    | Moderate | Strong alternative                     |
| **CBA**      | 18.5%    | Higher   | Weak predictive relationship           |
| **ANZ**      | 17.4%    | Higher   | Least preferred                        |

---

## Key Insights

- **NAB** demonstrated the strongest causal relationship between traded volume and share prices.
- **WESTPAC** exhibited active trading trends, making it a solid alternative.
- **ANZ** and **CBA** showed weak inter-variable correlation, leading to lower forecast reliability.

---
