# 🚀 My Food Inspections Data Warehouse & BI Project

🔗 **[View Dashboard](https://app.powerbi.com/groups/me/reports/2b0f49c5-e2d0-4b6c-afe1-128b4303dc6f/7638e95db92838a5585c?experience=power-bi)**

---

## 📝 Project Overview

I built this end-to-end data engineering and BI project using real-world food inspection datasets from **Chicago** and **Dallas** food inspection websites, transforming messy raw data into structured insights with interactive dashboards.

## Dataset

Chicago - [Link]
Dallas - [Link]

### 👨‍💻 What I Did

- Engineered **ETL pipelines** (for data ingestion, cleaning, and modeling)  
- Designed a **dimensional data warehouse** (in Snowflake)  
- Developed **Power BI dashboards** (to analyze food safety risks and inspection trends)

---

## 📂 Datasets Used

| Dataset         | Records  | Highlights                                          |
|-----------------|----------|-----------------------------------------------------|
| **Chicago**     | 290K     | Establishment info, violations, risk levels         |
| **Dallas**      | 79K      | 114 columns, up to 25 violations per inspection     |

---

## 💻 Tech Stack

- **Data Profiling:** Alteryx, YData Profiling
- **ETL & Pipelines:** Azure Data Factory, Databricks, Snowflake, SQL  
- **Modeling:** ER/Studio (for Star Schema design)
- **Cleaning & Scripting:** Python, Regex, SQL  
- **Visualization:** Power BI, DAX

---

## 🔧 My Process

### 🏗️ Architecture

Implemented a **Medallion architecture**:

1. **Bronze:** Raw ingestion via SnowSQL  
2. **Silver:** Data cleaning and staging in Databricks  
3. **Gold:** Dimensional modeling in Snowflake with Azure Data Factory pipelines

---

### 🧹 Data Cleaning Highlights

✅ **Dallas Dataset**  
- Processed wide-format data (114 columns) using Alteryx  
- Parsed nested violation fields and merged into normalized rows  
- Derived Inspection Result, Risk Level, and Total Violation Score  
- Standardized names, removed whitespace with Regex  

✅ **Chicago Dataset**  
- Deduplicated on Inspection ID  
- Flattened violations to 1 row per violation  
- Cleaned and standardized city names, risk levels, ZIP codes

---

## 🗃️ Data Warehouse Design

| Table Type  | Tables Included |
|-------------|-----------------|
| **Dimensions** | DIM_LOCATION, DIM_INSPECTION, DIM_RESTAURANT, DIM_RESULT, DIM_RISK, DIM_VIOLATION |
| **Fact**   | FACT_INSPECTION – one row per violation per restaurant per inspection date |

📌 All pipelines were automated via **Azure Data Factory** for scalable deployment.

---

## 📊 My Power BI Dashboard

Built an interactive dashboard featuring:

- 📆 **Inspection Trends** – temporal analysis  
- 🏚️ **High-Risk Restaurants** – risk scoring and identification  
- ⚠️ **Violation Analysis** – most common violations and categories  
- 🌍 **Geospatial Heatmaps** – location-wise inspection results  
- 🤖 **AI-Powered Insights** – automated business insights for strategy

---

### 🔍 Dashboard Snapshots
<img width="1296" height="714" alt="Home Screen - Chicago_Dallas_Visualizations - Power BI" src="https://github.com/user-attachments/assets/a50a299c-3735-4f8f-9f2e-bf5acbca9577" />



## 🎯 Key Skills Demonstrated

✔️ ETL pipeline design and orchestration  
✔️ Advanced data cleaning and parsing (Regex, Alteryx)  
✔️ Dimensional modeling & DWH development in Snowflake  
✔️ Building KPI dashboards and reports in Power BI  
✔️ End-to-end ownership from data engineering to analytics delivery

---

## 🤝 Let’s Connect

I love solving real-world data challenges. If you’re looking for an intern or entry-level professional in **Data Engineering, Analytics, or BI**, feel free to reach out on [LinkedIn]().
