# Pharmacy Sales Forecasting — Time Series Analysis with Prophet

![Python](https://img.shields.io/badge/Python-3.10-blue) ![Prophet](https://img.shields.io/badge/Prophet-time%20series-green) ![statsmodels](https://img.shields.io/badge/statsmodels-decomposition-orange) ![Data](https://img.shields.io/badge/Data-6%20Years%20Weekly-lightblue)

**Time series forecasting of 8 pharmaceutical drug categories using seasonal decomposition and Facebook Prophet — with actionable inventory strategy recommendations for retail pharmacy chains.**

> Author: Afriyie Karikari Bempah, PharmD | [LinkedIn](https://linkedin.com/in/afriyiekarikaribempah) | [GitHub](https://github.com/akbempah1)

---

## Overview

This project applies time series forecasting to 6 years of weekly pharmacy sales data across 8 ATC drug categories. It combines classical seasonal decomposition (statsmodels) with Facebook Prophet to generate forecasts and translate them into actionable inventory strategies — directly applicable to retail pharmacy operations in Ghana through Aduru Analytics.

---

## Key Findings

| Finding | Implication |
|---|---|
| **R03 (respiratory) trend doubled over 6 years** | Growing demand requires proactive inventory scaling |
| **N05B (sedatives) declining post-2015** | Regulatory tightening on benzodiazepines visible in dispensing data |
| **Paracetamol MAPE = 17.6%** | High-volume chronic medications are highly forecastable |
| **Respiratory MAPE = 56.5%** | Flu epidemic spikes are fundamentally unpredictable — buffer stock essential |
| **Upper CI more useful than point forecast** | For seasonal drugs, plan to the upper confidence bound |

---

## Inventory Strategy Output

| Category | MAPE | Strategy |
|---|---|---|
| N02BE (Paracetamol) | 17.6% | Lean — weekly forecast-driven ordering |
| M01AB (Anti-inflammatory) | 24.6% | Lean — weekly forecast-driven ordering |
| N05B (Sedative) | 21.2% | Moderate buffer — monthly review |
| R03 (Respiratory) | 56.5% | Large buffer — epidemic risk |
| R06 (Antihistamine) | 58.6% | Large buffer — seasonal spikes |

---

## Technical Approach

- **Seasonal decomposition** — separates trend, seasonality, and residuals for 2 key categories
- **Facebook Prophet** — multiplicative seasonality model, yearly seasonality
- **Train/test split** — last 52 weeks held out as test set
- **MAE, RMSE, MAPE** — comprehensive accuracy evaluation
- **Business framing** — forecasts translated into inventory strategies

## Skills Demonstrated

- Time series analysis and seasonal decomposition
- Facebook Prophet forecasting
- Train/test evaluation for time series
- Business-framed output from analytical results
- Retail pharmacy domain knowledge

---

## Aduru Analytics Connection

This forecasting framework mirrors the inventory intelligence built into Aduru Analytics for KAM AID Pharmacy Ltd. across three branches in Greater Accra, Ghana — enabling data-driven procurement that reduces stockouts during peak illness seasons while minimizing excess working capital.

---

## How to Run

```bash
git clone https://github.com/akbempah1/pharmacy-sales-forecasting.git
pip install pandas numpy matplotlib statsmodels prophet scikit-learn jupyter
jupyter notebook pharmacy_sales_forecasting.ipynb
```

Dataset: [Pharma Sales Data — Kaggle](https://www.kaggle.com/datasets/milanzdravkovic/pharma-sales-data)

---

## Portfolio Series

- [Project 1 — Medicare Drug Spending](https://github.com/akbempah1/medicare-drug-spending-analysis)
- [Project 2 — FDA Adverse Events](https://github.com/akbempah1/fda-adverse-events-analysis)
- [Project 3 — Hospital Readmissions](https://github.com/akbempah1/hospital-readmissions-prediction)
- [Project 4 — Pharma Portfolio](https://github.com/akbempah1/pharma-stock-portfolio-analysis)
- [Project 5 — Credit Risk Scoring](https://github.com/akbempah1/credit-risk-scoring)
- [Project 6 — Africa Disease Burden](https://github.com/akbempah1/africa-disease-burden-analysis)
- [Project 7 — Malaria Prediction](https://github.com/akbempah1/malaria-prediction-africa)
- **Project 8 — Pharmacy Sales Forecasting** ← you are here
