# Customer Churn Analysis

An end-to-end analysis of 7,043 telecom customers to identify churn drivers, 
flag at-risk customers, and recommend retention strategies. Built across Excel, 
SQL, and Python to demonstrate how each tool handles the same analytical problem 
differently.

---

## Project Overview

| Tool | Role | Key Skills |
|------|------|-----------|
| **Excel** | Quick exploration, stakeholder-ready visuals | PivotTables, conditional formatting, calculated columns |
| **MySQL** | Structured querying, risk segmentation | `GROUP BY`, `CASE` with multiple `WHEN`, `JOIN`, window functions |
| **Python** | Reproducible pipeline, automation, export | pandas, matplotlib, `pd.crosstab()`, boolean indexing |

---

## Dataset

**Source:** [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
[Linkedin](https://www.linkedin.com/in/marshal-favour/)
[GitHub](https://github.com/ejikejohn)
**Size:** 7,043 rows × 21 columns  
**Target Variable:** `Churn` (Yes/No)

| Key Column | Description |
|-----------|-------------|
| `customer_id` | Unique identifier |
| `contract` | Month-to-month / One year / Two year |
| `tenure` | Months as customer |
| `monthly_charges` | Monthly bill amount |
| `churn` | Whether customer left |

---

## Key Findings

| Insight | Evidence | Action |
|---------|----------|--------|
| Month-to-month customers churn at **43%** | Pivot table / SQL aggregation | Push contract upgrades |
| Two-year contracts churn at **3%** | Same as above | Incentivize longer commitments |
| New customers (≤12 months) are highest risk | Tenure binning in SQL + Python | Onboarding intervention |
| **847 current customers match churn profile** | Boolean filtering in Python | Targeted retention campaign |
| **$127K–$169K revenue** at risk | Revenue projection from flagged segment | 10% discount offer to at-risk group |

---

## Repository Structure
<img width="681" height="355" alt="image" src="https://github.com/user-attachments/assets/c23d0ca3-c8c9-4898-8023-1ff52fd7bfb9" />
<img width="664" height="241" alt="image" src="https://github.com/user-attachments/assets/09f239e9-a008-44a6-b20a-2e5b78e3c986" />

---

## How to Run This Project

### Excel
1. Open `excel/churn_exploration.xlsx`
2. Explore pivot tables and conditional formatting
3. Modify `ChurnBinary` helper column to test new segments

### SQL
1. Install MySQL Server and MySQL Workbench
2. Run `sql/01_create_table.sql` to build the database
3. Import the CSV via Table Data Import Wizard
4. Execute queries 02–05 sequentially

### Python
```bash
pip install pandas matplotlib seaborn

---

## How to Run This Project

### Excel
1. Open `excel/churn_exploration.xlsx`
2. Explore pivot tables and conditional formatting
3. Modify `ChurnBinary` helper column to test new segments

### SQL
1. Install MySQL Server and MySQL Workbench
2. Run `sql/01_create_table.sql` to build the database
3. Import the CSV via Table Data Import Wizard
4. Execute queries 02–05 sequentially

### Python
```bash
pip install pandas matplotlib seaborn
python python/churn_pipeline.py
<img width="707" height="303" alt="image" src="https://github.com/user-attachments/assets/cb2908d0-a354-49a4-bc2c-1ff892aa8598" />
<img width="688" height="203" alt="image" src="https://github.com/user-attachments/assets/77a57cd4-375d-480f-be31-071599ad5a26" />

[Linkedin](https://www.linkedin.com/in/marshal-favour/)
[GitHub](https://github.com/ejikejohn)
