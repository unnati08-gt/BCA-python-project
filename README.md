# BCA-python-project
BCA 4th sem Python project
Project Description
Mutual Fund Investment Trends & Portfolio Performance Analytics is a data analytics project developed as part of the BCA 4th Semester curriculum.
The project focuses on analyzing mutual fund investment behavior, growth trends, and portfolio performance using financial KPIs and risk-return metrics.
Using Python-based data analysis and visualization techniques, the project evaluates Assets Under Management (AUM), SIP contributions, NAV growth, CAGR, volatility, Sharpe ratio, drawdowns, and benchmark comparison (NIFTY 50).
The analysis provides actionable insights useful for investors, analysts, and FinTech platforms to support data-driven investment decisions.
🎯 Key Features / KPIs (Key Pass)
Assets Under Management (AUM) Growth
Net Fund Inflows & Outflows
SIP Contribution Trends
NAV Growth Rate
Compound Annual Growth Rate (CAGR)
Rolling Returns (12-Month)
Volatility (Risk Measurement)
Sharpe Ratio (Risk-Adjusted Return)
Fund vs Benchmark (NIFTY 50) Performance
Asset Allocation (Equity / Debt / Hybrid)
Category-wise AUM Distribution
Month-on-Month (MoM) & Year-on-Year (YoY) Growth
Maximum Drawdown Analysis
Risk–Return Summary
🧠 Methodology
Data Generation & Collection
Created realistic mutual fund datasets using Python
Monthly data covering a 36-month period
Data Cleaning & Preprocessing
Handled missing values
Converted date formats
Prepared structured DataFrames using Pandas
KPI Calculation
Calculated growth, return, and risk metrics
Implemented financial formulas such as CAGR, Sharpe Ratio, Drawdown
Risk & Return Analysis
Evaluated volatility and downside risk
Compared fund performance against benchmark index
Data Visualization
Used charts and graphs to represent insights clearly
Enabled easy interpretation of trends and performance
Insight Generation
Derived conclusions useful for investors and fund managers
📁 Dataset Description
The dataset is programmatically generated using Python to simulate real-world mutual fund data.
Designed to resemble publicly available datasets from AMFI and NSE.
Time Period: 36 months (monthly data)
Dataset Fields:
Date – Monthly time index
AUM – Assets Under Management
SIP – Monthly SIP contribution value
NAV – Net Asset Value of the fund
Benchmark – Benchmark index value (NIFTY 50)
Dataset Creation (Sample Code):
Copy code
Python
import pandas as pd
import numpy as np

dates = pd.date_range(start="2022-01-01", periods=36, freq='M')

data = pd.DataFrame({
    "Date": dates,
    "AUM": np.cumsum(np.random.uniform(50, 120, size=36)) + 1000,
    "SIP": np.random.uniform(80, 150, size=36),
    "NAV": np.cumsum(np.random.uniform(0.8, 2.5, size=36)) + 10,
    "Benchmark": np.cumsum(np.random.uniform(0.6, 2.0, size=36)) + 10
})

data.set_index("Date", inplace=True)
🛠️ Tools & Technologies
Python
Pandas & NumPy
Matplotlib / Seaborn
Jupyter Notebook
CSV / Excel datasets
📌 Project Suitability
This project is highly suitable for:
FinTech Analytics
Mutual Fund Performance Evaluation
Investment Advisory Platforms
Portfolio Risk Analysis
Data Analyst & Financial Analyst roles
