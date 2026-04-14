# 🏡 Property Tax & Assessment Data Quality Dashboard

## 📌 Project Overview
This project presents an end-to-end **data quality and validation solution** for municipal property tax and assessment datasets. Leveraging **Power Query**, **Excel**, and **interactive dashboarding**, the solution automates the detection of data inconsistencies, enhances governance, and supports evidence-based decision-making.

The dashboard enables stakeholders to monitor data integrity, identify anomalies, and prioritize remediation efforts through intuitive visualizations and exception reporting.

---

## 🎯 Problem Statement
Municipal property assessment data is often prone to quality issues such as:
- Duplicate roll numbers
- Invalid municipality or property class codes
- Tax calculation mismatches
- Missing or incomplete records
- Statistical outliers in assessed property values

Manual validation of these large datasets is time-consuming and error-prone. This project addresses these challenges by implementing an **automated and scalable data quality framework**.

---

## 🛠️ Tools & Technologies
- **Microsoft Excel**
- **Power Query (ETL & Data Transformation)**
- **Pivot Tables & Pivot Charts**
- **Data Validation Techniques**
- **Statistical Analysis (Z-score for Outlier Detection)**
- **Interactive Dashboard Design**

---

## 🔄 Methodology

### 1. Data Preparation
- Structured raw datasets into Excel tables.
- Imported data into Power Query for transformation and validation.

### 2. Data Transformation & Integration
- Merged reference tables for municipalities, property classes, and tax rates.
- Implemented a layered ETL architecture:

### 3. Data Quality Validation Checks
The following validation rules were implemented:

| Validation | Description |
|-----------|-------------|
| Municipality_Code_Check | Verifies municipality codes against reference data |
| Municipality_Name_Check | Ensures consistency between code and name |
| Property_Class_Check | Validates property classifications |
| Tax_Check | Confirms assessed tax calculations |
| Duplicate_Check | Identifies duplicate roll numbers |
| Postal_Code_Check | Validates postal code format |
| Sale_Date_Check | Ensures valid and logical dates |
| Completeness_Check | Detects missing or null values |
| Outlier_Check | Identifies anomalous assessed values using Z-score |

### 4. Outlier Detection
Outliers were identified using the Z-score formula:
