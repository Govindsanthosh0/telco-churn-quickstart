# Telco Customer Churn – Fast EDA & Baseline Model
**Goal:** Explain drivers of customer churn and train a baseline model in under 60 minutes.

## Dataset
- Source (IBM sample; mirrored for easy download): `WA_Fn-UseC_-Telco-Customer-Churn.csv` (7,043 rows).

## What’s inside
- `notebooks/01_eda.ipynb` — quick exploration, churn rate, visuals
- `notebooks/02_model.ipynb` — baseline Logistic Regression + feature importance
- `src/` — utility scripts
- `assets/` — generated charts and metrics
- `data/` — put raw CSVs under `data/raw/` (created automatically by notebooks)

## How to run
```bash
python -m venv .venv && (.venv\Scripts\activate || source .venv/bin/activate)
pip install -r requirements.txt
jupyter lab
```
Open the notebooks in order. The first cell downloads the dataset automatically.

## Results to report (after running)
- Overall churn rate
- AUC score of baseline model
- Top 10 drivers (absolute logistic coefficients)
