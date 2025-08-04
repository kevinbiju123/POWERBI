# ☁️ End-to-End Power BI Project – Azure SQL Integration FOR SHIRT.PBIX

This project showcases a complete business intelligence pipeline using **Azure SQL Database** as the data source and **Power BI** for reporting and visualization. The solution tracks product performance by brand, using cloud-based data cleaning, DAX calculations, and advanced visuals from Power BI AppSource.

---

## 🧩 Problem Statement

The business lacked a centralized, cloud-based system to manage brand-level performance data. There was no visibility into key metrics like discount percentage, profit margin, cost pricing, or brand variety. Decision-makers needed an interactive dashboard hosted on the cloud for easier access and collaboration.

---

## 💡 Solution

We built a scalable and cloud-connected Power BI dashboard that integrates:
- Cloud-hosted Azure SQL Database for storage and querying
- Power BI Desktop for DAX-based data modeling
- AppSource visuals for impactful storytelling
- Power BI Service for secure sharing and publishing

---

## 🔧 Steps Performed

### 1. 🔐 **Azure Setup**
- Created a free Azure account.
- Deployed **Azure SQL Database** and provisioned server credentials.

### 2. 📤 **Data Upload to Azure SQL**
- Uploaded local sales/product data to the Azure SQL environment.
- Verified successful import using SSMS or Azure Data Studio.

### 3. 🧼 **Data Cleaning in Azure SQL**
- Removed nulls, corrected data types, and filtered unwanted records using SQL.

### 4. 🔗 **Connecting Power BI to Azure SQL**
- Connected to Azure SQL via:
  - **Database credentials**
  - **Microsoft account authentication**

### 5. 🧹 **Data Cleaning in Power BI**
- Applied additional cleanup in **Power Query Editor**:
  - Renamed columns
  - Formatted data types
  - Removed duplicates

### 6. 📐 **DAX Calculations**
Created the following DAX measures:
```DAX
-- Discount %
Discount % = DIVIDE([Discount], [Sales], 0)

-- Profit %
Profit % = DIVIDE([Profit], [Sales], 0)

-- Cost Price
Cost Price = [Sales] - [Profit]
