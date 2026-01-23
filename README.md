# Yanki eCommerce Data Engineering — ETL Pipeline (Python & PostgreSQL)

This project implements a practical **end-to-end ETL (Extract, Transform, Load) data pipeline** for eCommerce datasets using **Python, Pandas, NumPy, and PostgreSQL**.

It demonstrates how raw business data can be systematically cleaned, transformed, and loaded into a relational database to make it analytics-ready.

---

## Project Overview

In real-world data engineering, raw data is rarely usable in its original form.  
This project simulates a typical **data engineering workflow** where:

- Raw CSV data is ingested
- Data quality issues are handled
- Data is standardized and transformed
- Cleaned data is persisted into a structured PostgreSQL database

This mirrors how production data pipelines operate in analytics teams.

---

## Technologies Used

| Tool | Purpose |
|-----|---------|
| **Python** | Core programming language |
| **Pandas** | Data cleaning and transformation |
| **NumPy** | Efficient numerical processing |
| **PostgreSQL** | Structured data storage |
| **psycopg2** | Database connectivity |
| **Jupyter Notebook** | ETL workflow execution |

---

## Project Structure

yanki_etl.ipynb # Main ETL pipeline
dataset/ # Raw input data
dataset/cleaneddata/ # Processed/cleaned output data

yaml
Copy code

---

## 🔄 ETL Workflow

### 1️⃣ Extract
- Raw eCommerce CSV datasets are loaded into Pandas DataFrames

### 2️⃣ Transform
- Missing values handled
- Column formats standardized
- Data cleaned and validated
- Inconsistencies removed using Pandas & NumPy operations

### 3️⃣ Load
- Cleaned datasets are inserted into PostgreSQL tables using `psycopg2`
- Data becomes structured and ready for analytics/reporting

---

## What This Demonstrates

This project showcases:

- Practical ETL design using Python
- Data cleaning techniques used in production
- Database loading and persistence
- Preparing business data for analytics use
- Foundational data engineering skills

---

## How to Run

### Step 1 — Install dependencies

```bash
pip install pandas numpy psycopg2 jupyter
Step 2 — Configure PostgreSQL
Create a database and update the connection details inside the notebook:

python
Copy code
conn = psycopg2.connect(
    host="localhost",
    database="your_database",
    user="your_user",
    password="your_password"
)
Step 3 — Run the ETL
bash
Copy code
jupyter notebook
Open yanki_etl.ipynb and run all cells sequentially.

Output
Cleaned CSV files saved in dataset/cleaneddata/

Structured data stored in PostgreSQL tables

Why This Project Matters
This project reflects the core responsibility of a Data Engineer:

Turning messy raw data into structured, reliable, analytics-ready datasets.

👤 Author
Randy Inala Philip
