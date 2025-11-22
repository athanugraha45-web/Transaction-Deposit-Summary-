# Transaction & Deposit Summary Dashboard
This project documents the complete workflow of processing ATM transaction data — starting from merging raw data using Python, creating a 50,000-row sampled dataset, and building a Daily Operational Dashboard in Microsoft Excel.
The dashboard visualizes key daily ATM performance indicators such as total transactions and total deposit amount.

# Tools
Python (Pandas) → merging, cleaning, data processing, random sampling
Microsoft Excel → dashboard creation, Pivot Table, and Pivot Chart

# Data Processing Workflow
## Merge 4 Transaction Files
Performed using Python:
Combine all transaction files
Standardize Date and TransactionStartDateTime
Remove duplicates
Clean missing values

# Date Standardization
All date fields are unified into:
Date = YYYY-MM-DD
TransactionStartDateTime = YYYY-MM-DD HH:MM:SS
This ensures accurate joining, filtering, and analysis.

# Random Sampling (50,000 Rows)
Used to reduce dataset size and speed up dashboard performance:

df_sample = df.sample(n=50000, random_state=42)
df_sample.to_csv('dataset_50k.csv', index=False)

# Dashboard Components

## The dashboard includes:

Daily Total Transactions

Total Deposit Amount

Top 5 ATMs by Transaction Count

## Visualization methods include:

Pivot Tables

Pivot Charts (line, bar, area)

Slicers & Date Filters

# Python Notebook

# All processing steps are documented in:

- <a href = "https://github.com/athanugraha45-web/Transaction-Deposit-Summary-/blob/main/Notebook.ipynb"> Data Cleaning and Processing </a>
Includes:

Data import & merging

Data cleaning & formatting

Feature engineering

Random sampling

Final data export

# Dashboard Preview
- <a href = "https://github.com/athanugraha45-web/Transaction-Deposit-Summary-/blob/main/Screenshot%20(132).png"> Result </a>
