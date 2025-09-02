# Mini Mortgage Fund Compliance Check (Slice Project)

## 📌 Overview
This is a **small-scale prototype** of a larger compliance monitoring dashboard for a mortgage investment fund.  

- Data ingestion pipelines
- SQL transformations
- Basic compliance checks
- Dashboard rendering

This project is the **slice** version of the full **Mortgage Fund Compliance & KPI Dashboard** hero project, intended to prove out the technical workflow before scaling to a larger datasets.

---

## 🛠️ Tools & Versions

| Tool / Framework       | Version Tested | Purpose |
|------------------------|---------------|---------|
| **Python**             | 3.11+         | Core scripting & data processing |
| **pandas**             | 2.0+          | Data cleaning & manipulation |
| **dbt Core**           | 1.7+          | Data transformation modeling |
| **Snowflake**          | Current (Enterprise Trial) | Cloud data warehouse |
| **Apache Airflow**     | 2.8+          | Basic task scheduling |
| **Great Expectations** | 0.18+         | Data validation & quality checks |
| **Git**                | 2.40+         | Version control |
| **Git Bash**           | Latest        | Command line interface for Git |
| **Marimo**             | Latest        | Interactive Python notebooks |
| **VS Code**            | Latest        | IDE for code editing |
| **Docker**             | 24+           | Containerization (optional, for Airflow/dbt setup) |

---

## 📂 Project Structure

mini_mortgage_compliance/
│
├── data/
│ ├── sample_loans.csv
│ ├── sample_loans.json
│ └── sample_loans.yaml
│
├── dbt/
│ ├── models/
│ └── profiles.yml
│
├── airflow/
│ ├── dags/
│ └── requirements.txt
│
├── great_expectations/
│ └── expectations/
│
├── notebooks/
│ └── exploration.ipynb
│
├── scripts/
│ ├── ingest.py
│ ├── transform.py
│ └── validate.py
│
└── README.md


---

##  Disclaimer ##

> **Note:** The dataset provided in `data/` is **entirely dummy data**, generated for educational purposes and **not proprietary**. No real customer or confidential information is included.

---

## Milestones ##

1. **Environment Setup** – Install and configure all required tools.  
2. **Data Loading** – Ingest CSV, JSON, and YAML formats into Snowflake.  
3. **Data Cleaning & Transformation** – Use `pandas` and `dbt` to standardize formats.  
4. **Validation** – Apply Great Expectations to ensure data quality.  
5. **Visualization** – Create a basic compliance dashboard in your preferred BI tool.  
6. **Automation** – Schedule recurring checks with Airflow.

---

## 📌 Status

This is the **slice version** — it validates the workflow and tools before expanding to the full dataset and complex logic.

---

## 🛠️ Tools & Versions ## 

- **Python** – 3.11  
- **Snowflake** – Enterprise Edition  
- **dbt** – 1.7+  
- **Apache Airflow** – 2.8+  
- **Great Expectations** – 0.18+  
- **pandas** – 2.1+  
- **Git Bash** – Latest stable  
- **Marimo** – Latest stable (for interactive notebooks)

---

## How to Run This Project ##

##Clone the Repository
```bash
git clone https://github.com/ruxandra-stefan/mini_mortgage_compliance.git
cd mini_mortgage_compliance

2Create a Virtual Environment

python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows

Install Dependencies
pip install -r airflow/requirements.txt
pip install dbt-core pandas great_expectations

Configure Snowflake


Data Ingestion

python scripts/ingest.py

Run Transformations with dbt

dbt run

Validate Data with Great Expectations

great_expectations checkpoint run loan_data_checkpoint

Explore Data

Open notebooks/exploration.ipynb in Jupyter, VS Code, or Marimo.
