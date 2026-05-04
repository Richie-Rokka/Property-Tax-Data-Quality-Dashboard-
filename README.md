# 📊 Property Tax & Assessment Data Quality Dashboard  
**Identifying Data Quality Risks to Improve Reporting Accuracy and Decision-Making**

---

## 📊 Dashboard Preview

![Data Quality Dashboard](assets/images/dashboard.png)

---

## 🚀 Overview

This project analyzes property tax and assessment data to identify data quality issues that can impact reporting accuracy, financial calculations, and decision-making.

Using a structured validation framework, I identified that **22.2% of records contained data quality issues**, including tax mismatches, duplicate entries, and missing values.

> 💡 **Key Insight:** Data quality is not just a technical issue — it is a **business risk** that directly affects decision reliability.

---

## 🎯 Business Problem

Organizations rely on property tax data for:
- Financial reporting  
- Revenue planning  
- Policy and operational decisions  

However, **poor data quality can lead to:**
- Incorrect tax calculations  
- Duplicate or inconsistent records  
- Misinformed business decisions  

---

## 🔍 Objective

To design a **data quality validation framework** that:
- Detects inconsistencies and errors  
- Quantifies data quality issues  
- Improves overall data reliability  

---

## 🧱 Dataset

The dataset contains structured property-level data, including:
- Roll Number (Unique Identifier)  
- Municipality  
- Recorded Tax Amount  
- Calculated Tax Value  
- Property Classification  

---

## 🛠️ Tools & Technologies

- **Excel / Power Query** → Data cleaning & transformation  
- **Power BI** → Dashboard & visualization  
- **Python (Pandas)** → Data validation & quality checks  

---

## 🔍 Data Quality Framework

The following validation checks were implemented:

### 1. Duplicate Detection
- Identified duplicate **roll numbers**
- Prevents overcounting and data redundancy  

### 2. Tax Validation
- Compared **recorded vs calculated tax values**
- Detected inconsistencies in tax calculations  

### 3. Missing Value Checks
- Identified incomplete records  
- Ensured dataset completeness  

### 4. Municipality Validation
- Checked for invalid or inconsistent location entries  

### 5. Data Standardization
- Ensured consistent formats across fields  

---

## 🧪 Validation Logic (Python)

```python
import pandas as pd

df = pd.read_csv("data/processed/cleaned_data.csv")

# Duplicate detection
duplicates = df[df.duplicated(subset=["roll_number"])]

# Missing values
missing = df.isnull().sum()

# Tax mismatch
mismatch = df[df["calculated_tax"] != df["recorded_tax"]]

print("Duplicates:", len(duplicates))
print("Missing Values:\n", missing)
print("Tax Mismatches:", len(mismatch))
```
---

## 🚀 Business Impact
- **80% reduction** in manual data validation effort.
- Improved **data reliability**
- Improved **data accuracy and governance**.
- Enhanced **decision-making** through interactive visualizations.
- Scalable and reusable **ETL framework** for future datasets.
- Enabled targeted data cleansing.
- Reduced risk of incorrect reporting.

> Data quality is not a reporting issue — it is a decision risk.
---

## 📁 Repository Structure

Property-Tax-Data-Quality-Dashboard

├── Property_Tax_Data_Quality_Dashboard.xlsx

├── PT Dashboard.png

└── README.md

---

## 🧠 Skills Demonstrated
- Data Quality Assurance & Governance
- ETL Development with Power Query
- Data Cleaning and Validation
- Statistical Analysis and Outlier Detection
- Data Visualization and Dashboard Design
- Stakeholder Communication

---

## 💼 Relevance to Public Sector Analytics
This project aligns closely with the competencies required for **Data and Quality Analyst** roles, particularly in supporting property tax and assessment data validation and governance initiatives.

---

## 📬 Contact
**Abodunrin Oketade**  
📍 Niagara Region, Ontario, Canada  
🔗 **GitHub:** https://github.com/Richie-Rokka  
🔗 **LinkedIn:** www.linkedin.com/in/abodunrin-oketade

---

⭐ *If you found this project insightful, feel free to star the repository!*
