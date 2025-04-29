# dynamic-credit-spread-regime-modeling
# Dynamic Credit Spread Regime Modeling and Macro Shock Simulation

## 📌 Overview

This project analyzes the behavior of corporate bond credit spreads over time using real-world economic indicators. It applies machine learning (Gaussian Mixture Models) to identify hidden economic regimes and studies how macroeconomic factors affect credit spreads in different market conditions. A GDP stress simulation is also conducted to evaluate spread sensitivity under crisis scenarios.

---

## 📊 Objectives

- Calculate historical credit spreads between corporate and treasury bonds.
- Identify hidden market regimes (Crisis vs Calm) using Gaussian Mixture Models.
- Perform regression analysis of macroeconomic drivers (CPI, GDP, Unemployment, Fed Funds) on credit spreads.
- Compare macro impact in each regime separately.
- Simulate spread behavior under a hypothetical 2% GDP drop (stress testing).

---

## 🧠 Key Techniques Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Gaussian Mixture Models (sklearn)
- Statsmodels for OLS regression
- Real financial datasets from FRED
- Stress scenario simulation

---

## 📂 Data Sources

All data pulled from [FRED Economic Data](https://fred.stlouisfed.org/):

- Corporate Bond Yields (BAMLCC0A0CMTRIV)
- 10-Year Treasury Yield (GS10)
- Consumer Price Index (CPIAUCSL)
- Real GDP (GDP)
- Unemployment Rate (UNRATE)
- Federal Funds Rate (FEDFUNDS)

---

## 📈 Output Plots

All key visualizations are saved in the `/plots/` folder:

- `spread_over_time.png`
- `regime_classification.png`
- `stress_scenario_spread.png`

---

## 🔬 Folder Structure

Credit-Spread-Regime-Modeling/
├── credit_spread_modeling.ipynb        # Main Jupyter notebook with full analysis
├── README.md                           # Project description and overview
├── credit_spread_regimes_final.csv     # Final output CSV file
├── /data/                              # Raw input datasets from FRED
│   ├── BAMLCC0A0CMTRIV.csv
│   ├── GS10.csv
│   ├── CPIAUCSL.csv
│   ├── GDP.csv
│   ├── UNRATE.csv
│   └── FEDFUNDS.csv
└── /plots/                             # Output charts
    ├── spread_over_time.png
    ├── regime_classification.png
    └── stress_scenario_spread.png


