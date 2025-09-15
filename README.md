# Telco Customer Churn – EDA & Logistic Regression Model  

Analyzed IBM’s Telco Churn dataset to identify why customers leave and trained a Logistic Regression model achieving **ROC-AUC = 0.84**.  

![Churn Count](assets/churn_count.png)

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
## Results

**Churn Rate:** 26.6%  
**ROC-AUC (Logistic Regression):** <paste AUC value here>

### Key Insights
- Month-to-month contracts have the highest churn risk.
- Customers with longer tenure churn far less often.
- AutoPay and credit card payments correlate with lower churn.
![aaa](https://github.com/user-attachments/assets/a4131579-e72f-4799-8a6c-d0f4103106f3)

![11111](https://github.com/user-attachments/assets/9c4565f3-03ca-41fd-b3af-81e83c54dd29)

