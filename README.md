# Mini Mortgage Fund Compliance Check (Slice Project)

## 📌 Overview
This is a **small-scale prototype** of a larger compliance monitoring dashboard for a mortgage investment fund.  
It uses **dummy, non-proprietary data** (10–20 sample loans) to validate:

- Data ingestion pipelines
- SQL transformations
- Basic compliance checks
- Dashboard rendering

This project is the **slice** version of the full **Mortgage Fund Compliance & KPI Dashboard** hero project, intended to prove out the technical workflow before scaling to real or larger datasets.

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

