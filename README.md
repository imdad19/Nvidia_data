# NVIDIA Strategic-Financial Dataset (2015–2024)

This repository contains a curated dataset of quarterly financial, market, and AI-related strategic indicators for **NVIDIA Corporation**, spanning from **Q2 2015 through Q3 2024**. The dataset was constructed for use in empirical economic and data science research focused on the role of artificial intelligence (AI) in shaping firm-level performance.

---

## Overview

The data includes financial fundamentals (e.g., revenue, R&D expenses), stock performance, macroeconomic context (U.S. GDP growth), and several hand-constructed variables capturing NVIDIA’s contributions to the AI ecosystem through product launches and strategic investments.

This dataset is particularly well-suited for:

- Time series and econometric modeling (e.g., ARDL, ECM, VAR)
- Causal inference involving macro firm dynamics
- AI strategy benchmarking and forecasting
- Academic studies of technological innovation

---

## File Contents

### `Nvidia_data.csv`

A single CSV file with 38 quarterly observations (Q2 2015 – Q3 2024), including the following variables:

| Column Name                     | Description |
|--------------------------------|-------------|
| `date`                         | Quarter (Not fiscal)  |
| `market_cap`                   | Market capitalization (in USD billions) |
| `General_expenses`             | General and administrative expenses (in USD billions) |
| `s_price`                      | NVIDIA stock price at the end of the quarter (in USD) |
| `total_revenue`                | Quarterly total revenue (in USD billions) |
| `data_center_revenue_dominance` | Share of data center revenue as a percentage of total revenue (%) |
| `r_and_d_intensity`            | R&D expenses as a percentage of total revenue (%) |
| `invested_in_ai`               | Number of strategic AI startup investments made by NVIDIA during the quarter |
| `launched_ai_product`          | Number of new AI related products launched by NVIDIA during the quarter |
| `us_gdp_growth_rate`           | U.S. quarterly GDP growth rate (%) |
| `contribution_to_ai`           | Composite index quantifying NVIDIA's AI-related contributions by summing the number of product launched and startups invested in |
| `r_and_d_expenses_quarterly`  | Estimated **quarterly R&D expenses (in USD billions)**, derived from reported TTM values |

---

## Units and Scaling

To maintain consistency across financial modeling and analysis, units are standardized as follows:

- **Billions of USD**: `market_cap`, `General_expenses`, `total_revenue`, `r_and_d_expenses_quarterly`
- **USD (raw)**: `s_price` (per-share stock price)
- **Percentages**: `r_and_d_intensity`, `data_center_revenue_dominance`, `us_gdp_growth_rate`
- **Counts**: `invested_in_ai`, `launched_ai_product` (number of events per quarter)

---
## Use Cases and Applications

This dataset supports:

- Empirical financial modeling and economic research
- Causal analysis of innovation and investment outcomes
- Forecasting NVIDIA's market behavior in response to AI strategy
- Academic case studies in corporate innovation and R&D policy

Example research applications may include:

- ARDL and ECM models estimating the dynamic impact of AI investments on revenue
- Time series forecasting of R&D expenditure or stock price
- Panel studies of tech-sector firms using comparable datasets

---

## Citation

If you use this dataset in your research, publications, or presentations, please cite it as follows:

> **"NVIDIA Quarterly Strategic-Financial Indicators Dataset (2015–2024), curated by [Aouidane Imed Eddine & Benslimane Yasmine], 2025."**

You may optionally link back to this repository for access to source data and methodology.

---
