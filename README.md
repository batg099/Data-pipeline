# Data Pipeline — Talend & Power BI

> End-to-end data pipeline covering extraction, storage, dimensional modeling and interactive visualization.

---

## Tech Stack

![Talend](https://img.shields.io/badge/Talend-Data%20Integration-blue)
![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![MySQL](https://img.shields.io/badge/Database-MySQL-orange)

---

## Project Overview

This project consists of building a full data pipeline in two phases:

1. **ETL with Talend** — ingest raw data, model it into a star schema, and load it into a relational database
2. **Visualization with Power BI** — connect to the database and build an interactive dashboard

---

## Star Schema

The dimensional model is structured as follows:

- `fact_table` — central fact table containing key measures
- `dim_*` — dimension tables linked to the fact table

---

## Repository Structure

```
 ┣ 📂 talend
 ┃ ┣ 📜 project.zip
 ┃ ┣ 📊 fact_table.csv
 ┃ ┗ 📊 dim_*.csv
 ┣ 📂 powerbi
 ┃ ┗ 📊 dashboard.pbix
 ┗ 📄 README.md
```

---

## How It Works

### Step 1 — Data Ingestion
Load source files into a relational database using Talend jobs.

### Step 2 — Dimensional Modeling
Design and load a star schema (dimension tables + fact table) into the database.

### Step 3 — Dashboard
Import tables into Power BI and build a dashboard from a direct database connection.
