# 🧹 Data Cleaning & Pre-processing for an Internal Audit

This project simulates a real-world **internal audit data cleaning process** commonly undertaken in large organizations. The dataset consists of over **1,000 rows** and **9 columns** collected from multiple departments, mimicking the inconsistencies and formatting issues often encountered during audits.

## 🧾 Objective

To clean and standardize a messy internal audit dataset to make it suitable for accurate analysis and reporting. This includes:

- Normalizing inconsistent entries
- Handling missing or invalid data
- Correcting data types
- Ensuring audit-related fields are in usable format

---

## 🗂️ Dataset Overview

The dataset includes the following columns:
- `Employee_ID`
- `Department`
- `Location`
- `Risk_Score`
- `Audit_Finding`
- `Finding_Date`
- `Resolved`
- `Control_Weakness`
- `Comments`

This project tackles a wide range of typical data quality issues that arise in internal audit processes including:

- **Inconsistent text labels** (e.g., `RetailBank` vs `Retail Banking`, `Y` vs `Yes`)
- **Unusable numerical data** (e.g., `"unknown"` in `Risk_Score`)
- **Inconsistent boolean indicators** (`F`, `FALSE`, `T`, `TRUE`)
- **Unformatted date values**

---

## 🧼 Cleaning Steps

### ✅ Normalizing `Department`
Standardized entries like `RetailBank` → `Retail Banking`.

### ✅ Cleaning `Risk_Score`
- Replaced `'unknown'` and blank values with `NaN`
- Converted to float with 2 decimal places

### ✅ Standardizing `Audit_Finding`
Mapped `'Y'`, `'N'`, `'Yes'`, and `'No'` into a unified format.

### ✅ Converting `Finding_Date`
Converted to proper `datetime` type for time-based operations.

### ✅ Normalizing `Resolved`
Unified various truthy/falsy labels (`TRUE`, `FALSE`, `F`, `T`) into `'Yes'` and `'No'`.

---

## 🔍 Key Learnings

- Demonstrated practical **data cleaning** and **pre-processing** techniques using Python and Pandas.
- Highlighted how messy audit data can be systematically refined for further analysis.
- Cleaned and normalized **1,010 rows across 9 columns**, ensuring the dataset is ready for use in dashboards, reports, or machine learning models.

---

## 📁 Technologies Used

- **Python 3.x**
- **Pandas**
- **NumPy**
- **Matplotlib** (for exploratory visuals)
- **Dateutil** (for robust date parsing)

---
