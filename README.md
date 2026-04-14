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

Property_Assessment → Validation_Base → Clean_Data → Data_Quality_Issues → Dashboard

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

Z = (Assessed_Value - Mean) / Standard_Deviation

Records with **|Z| > 3** were flagged for review.

### 5. Exception Reporting
A dedicated **Data_Quality_Issues** layer isolates all records failing one or more validation checks. An **Issue_Reason** column provides clear explanations for each flagged record.

### 6. Dashboard Development
An interactive Excel dashboard was designed to provide real-time insights, including:
- KPI cards summarizing data quality metrics
- Issue distribution by municipality and property class
- Data quality issue breakdown
- Average assessed property values
- Top 10 exception records
- Slicers for dynamic filtering
- A narrative “Key Insights” section

---

## 📊 Dashboard Features

<img width="348" height="355" alt="PT Dashboard" src="https://github.com/user-attachments/assets/dc81b3fa-96d1-4709-8a9a-6616f4f80560" />


### 🔹 Key Performance Indicators (KPIs)
- Total Records
- Valid Records (%)
- Incomplete Records
- Duplicate Municipality Codes
- Records with Issues (%)
- Tax Mismatches
- Invalid Municipality Codes
- Outliers

### 🔹 Visualizations
- **Issues by Municipality**
- **Issues by Property Class**
- **Data Quality Issue Breakdown**
- **Average Assessed Property Value by Class**
- **Top 10 Data Quality Exceptions**

### 🔹 Interactivity
- Slicers for Municipality, Assessment Year, and Property Class
- Dynamic KPI updates upon data refresh

---

## 📈 Key Insights
- **77%** of records are valid, indicating generally strong data quality.
- **Tax mismatches** are the most prevalent issue, affecting **9.4%** of records.
- **Toronto and Ottawa** exhibit the highest concentration of data quality issues.
- **Multi-residential properties** show the highest average assessed values.
- Automated validation significantly reduces manual data quality checks.

---

## 🚀 Impact
- **80% reduction** in manual data validation effort.
- Improved **data accuracy and governance**.
- Enhanced **decision-making** through interactive visualizations.
- Scalable and reusable **ETL framework** for future datasets.

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
🔗 **LinkedIn:** www.linkedin.com/in/abodunrin-oketade-579aa331  

---

⭐ *If you found this project insightful, feel free to star the repository!*
