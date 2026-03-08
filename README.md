# Shrinkflation in Household Cleaning Products
### BUSN 32120 — Data Analysis with Python and SQL
**Group 34:** Ridhi Agarwal | University of Chicago Booth School of Business, Winter 2026

---

## Project Overview
This project analyzes macroeconomic evidence of **shrinkflation** in household cleaning products on behalf of a hypothetical legal client. Using 55 years of government price data, we test whether cleaning product prices diverged abnormally from general inflation — particularly in the post-2019 period.

## Files
| File | Description |
|---|---|
| `final_agarwal.ipynb` | Main analysis notebook — introduction, EDA, feature engineering, models, SQL, and conclusion |
| `sql_queries_agarwal.ipynb` | Standalone SQL-only notebook with all 10 required queries, each fully commented |

## Data Sources
- **FRED API** (Federal Reserve Economic Data) — CPI indices for cleaning products, all-items, core, household, and nondurable goods; NBER recession indicator
- **BLS API** (Bureau of Labor Statistics) — Average retail price of laundry detergent (series APU0000703112)

## Key Findings
- Cleaning product prices tracked general inflation closely for decades
- A persistent, anomalous divergence began around 2019 and did not revert after COVID
- The divergence holds across multiple comparison benchmarks (headline CPI, core CPI, nondurables)
- SQL and machine learning analysis quantify the magnitude and duration of the excess pricing

## Methods Used
- Python (Pandas, matplotlib, seaborn, scikit-learn, SQLite)
- Two linear regression models (baseline vs. feature-engineered) compared by RMSE and Adjusted R²
- Logistic regression for recession prediction
- 10 SQL queries including JOINs, window functions, GROUP BY, and subqueries
