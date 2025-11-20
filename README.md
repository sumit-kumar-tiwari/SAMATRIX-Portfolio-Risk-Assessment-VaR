# SAMATRIX-Portfolio-Risk-Assessment-VaR
A comprehensive risk assessment of a tech stock portfolio (AAPL, MSFT, GOOG, AMZN) using Value at Risk (VaR), Expected Shortfall (ES), and Monte Carlo Bootstrapping in Python.




# Portfolio Risk Assessment & Value at Risk (VaR) Analysis

## 📌 Project Overview
This project quantifies the daily financial risk of an equally weighted four-stock portfolio comprising **Apple (AAPL), Amazon (AMZN), Google (GOOG), and Microsoft (MSFT)**. 

Using 5 years of historical data, the project calculates **1-Day 95% Value at Risk (VaR)** using three distinct methodologies to estimate potential losses under normal and extreme market conditions.

## 🎯 Objectives
- Fetch and clean historical stock data using `yfinance`.
- Analyze statistical properties of returns (Mean, Variance, Skewness, Kurtosis).
- Calculate **Value at Risk (VaR)** using:
  1. **Parametric Method (Normal Distribution)**
  2. **Parametric Method (Student's t-Distribution)**
  3. **Historical Simulation**
- Perform **Backtesting** to validate the accuracy of the VaR models.
- Analyze **Portfolio Diversification** using Correlation Matrices.
- Estimate **Expected Shortfall (CVaR)** for tail-risk assessment.

## 🛠️ Technologies & Libraries Used
- **Python 3.x**
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`
- **Statistical Analysis:** `scipy.stats`
- **Financial Data:** `yfinance`

## 📊 Key Findings
- **Normal vs. t-Distribution:** The data exhibited "fat tails" (high kurtosis), meaning extreme market crashes happen more often than a Normal Distribution predicts.
- **VaR Results (95% Confidence):**
  - Parametric (Normal): ~2.56%
  - Historical: ~2.64%
  - Parametric (t-dist): ~2.85% (Most conservative estimate)
- **Backtesting:** The Historical VaR model showed an exception rate of **5.02%**, aligning almost perfectly with the expected 5% failure rate.

## 📈 Visualizations Included
- Daily Log-Return Histograms
- Correlation Heatmaps
- Portfolio Cumulative Returns & Drawdown Analysis
- Rolling 60-Day VaR (Dynamic Risk)

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/Portfolio-Risk-Assessment-VaR.git](https://github.com/your-username/Portfolio-Risk-Assessment-VaR.git)
