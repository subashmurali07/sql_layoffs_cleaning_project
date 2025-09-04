# 📊 SQL Layoffs Data Project  

This project focuses on cleaning and analyzing a layoffs dataset using **MySQL**. It is divided into two parts: **Data Cleaning** and **Exploratory Data Analysis (EDA)**.  

---

## 🧹 1. Data Cleaning  
In `layoffs_cleaning.sql`, I performed the following steps:  
- Created staging tables for safe transformations  
- Removed duplicates using `ROW_NUMBER()`  
- Standardized company names, industries, and countries  
- Fixed date formats (`TEXT` → `DATE`)  
- Handled null and blank values  
- Removed unnecessary rows and columns  

---

## 🔎 2. Exploratory Data Analysis (EDA)  
In `layoffs_exploratory_analysis.sql`, I explored the cleaned dataset to answer key questions:  
- 📈 Maximum layoffs overall and by company  
- 🏭 Industries and countries most affected  
- 📅 Layoffs by time period (min/max dates, monthly/rolling totals)  
- 💰 Layoffs by company funding stage  
- 🏆 Top companies with the most layoffs per year  

Techniques used:  
- Aggregate functions (`MAX`, `SUM`, `MIN`)  
- `GROUP BY` with `ORDER BY`  
- Window functions (`DENSE_RANK()`, rolling totals)  
- Date functions (`YEAR()`, `SUBSTRING()`)  

---

## ⚙️ How to Use  
1. Import the layoffs dataset into MySQL as a table named **`layoffs`**.  
2. Run queries from **`layoffs_cleaning.sql`** to clean the data.  
3. Run queries from **`layoffs_exploratory_analysis.sql`** to perform analysis.  

---

## 🛠️ Tech Stack  
- SQL (MySQL)  
- Window Functions  
- CTEs  
- Date Functions  

---

✨ This project demonstrates the **end-to-end process** of preparing raw data and gaining insights using SQL.  
