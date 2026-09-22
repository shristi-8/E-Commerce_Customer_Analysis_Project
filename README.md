# E-Commerce Customer Analytics

A complete Data Analytics project using Python, SQL, and Power BI-ready outputs.

## Project Objective
Analyze customer behavior, order activity, customer value, preferred categories, geography, loyalty/engagement, and the dataset-provided fraud indicator.

## Tech Stack
- Python
- Jupyter Notebook
- Pandas & NumPy
- Matplotlib & Seaborn
- SQL
- Power BI (dashboard/reporting stage)

## Project Files
```text
ECommerce_Customer_Analytics/
├── ECommerce_Customer_Analytics.ipynb
├── requirements.txt
├── ECommerce_Project_Report.docx
├── README.md
├── synthetic_ecommerce_churn_dataset.csv
└── ecommerce_customer_cleaned.csv
```

## Dataset
The raw dataset contains 5,000 customer records and 13 columns:
- customer_id
- age
- gender
- country
- avg_order_value
- total_orders
- last_purchase
- is_fraudulent
- preferred_category
- email_open_rate
- customer_since
- loyalty_score
- churn_risk

`churn_risk` is treated as a numeric dataset field for descriptive analysis only; no predictive model is built.

## How to Run

### 1. Install Python
Use Python 3.10+ if possible.

### 2. Open the project folder
Open the folder in VS Code, Anaconda/Jupyter, or another Python environment.

### 3. Install dependencies
Open Terminal / Command Prompt in the project folder:

```bash
pip install -r requirements.txt
```

### 4. Start Jupyter
```bash
jupyter notebook
```

Or:
```bash
jupyter lab
```

### 5. Open the notebook
Open:
`ECommerce_Customer_Analytics.ipynb`

### 6. Run all cells
In Jupyter:
`Kernel → Restart & Run All`

The notebook will:
1. Load the raw CSV.
2. Inspect the data.
3. Clean column names and text.
4. Convert data types.
5. Convert date columns.
6. Remove duplicate rows.
7. Validate business ranges.
8. Impute missing numeric values using median.
9. Impute missing categorical values using mode.
10. Validate the cleaned dataset.
11. Save `ecommerce_customer_cleaned.csv`.
12. Perform EDA and KPI analysis.
13. Create customer segments.
14. Analyze categories, countries, loyalty/engagement and fraud indicators.
15. Print business-analysis outputs.

## Cleaning Logic
- Numeric missing values → median
- Categorical missing values → mode
- Exact duplicate rows → removed
- Invalid age → 0–120 validation
- Average order value → non-negative validation
- Total orders → non-negative validation
- Email open rate → 0–100 validation
- Loyalty score → 0–100 validation
- Churn risk → 0–1 validation
- Fraud indicator → 0/1 validation

## Important
The notebook is the primary reproducible analysis file. The DOCX report documents the project, methodology, findings, and execution steps.
