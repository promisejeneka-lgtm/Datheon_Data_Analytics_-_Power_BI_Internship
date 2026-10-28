# Task 3: Customer Cohort & Churn Analytics

Datheon Data Analytics & Power BI Internship

**Author:** Promise Jeneka Taiwo

## What this project is about
Using the IBM Telco Customer Churn dataset (7,043 customers), I grouped customers into cohorts by tenure and contract type, measured churn, and looked for the factors that push customers to leave.

## Files
- `Task3_Churn_Analytics.ipynb`: the full notebook with code, charts and written findings
- `telco_customer_churn.csv`: the dataset used

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## How to run it
1. `pip install pandas numpy matplotlib seaborn notebook`
2. Keep the notebook and the CSV in the same folder
3. Run `jupyter notebook` and run all cells

## Data cleaning
- No missing values, no duplicate customers.
- `TotalCharges` was stored as text. 11 rows were blank, all brand new customers with 0 months of tenure, so I set them to 0.
- Created a churn flag, tenure cohorts (12-month bands) and monthly charge bands.

## What I did
- Baseline churn rate and revenue lost to churn
- Tenure cohorts and a cohort matrix (tenure cohort by contract type)
- Retention curves by contract type (Kaplan-Meier method)
- Churn by payment method, monthly charge, service tier and tech support
- A churn heatmap by service tier and a high-risk segment

## Main findings
- Baseline churn is 26.5%, which is $139,131 of monthly revenue.
- Month-to-month contracts churn at 42.7%, against 11.3% (1-year) and 2.8% (2-year).
- First-year customers churn at 47.4%.
- Fiber optic customers with no tech support on month-to-month
