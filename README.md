## # 🚀 Sales Analytics Pipeline using AWS, Snowflake, dbt & Power BI
## 📌 Project Overview
This project demonstrates an end-to-end modern data pipeline built using **AWS S3, Snowflake, dbt, and Power BI**.

The pipeline ingests raw sales data, transforms it using dbt into structured layers, and visualizes business insights through an interactive dashboard.
## 🎯 Business Problem
Raw sales data is often:
- Unstructured and inconsistent  
- Difficult to analyze directly  
- Not optimized for reporting  

This project solves the problem by creating a **scalable analytics pipeline** for better decision-making.
## 🏗️ Architecture
csv_files---->AWS s3--->Snowflake--->dbt staging---->dbt mart----> Power BI

## ⚙️ Tech Stack

- ☁️ AWS S3 – Data storage  
- ❄️ Snowflake – Cloud Data Warehouse  
- 🔁 dbt – Data transformation  
- 📊 Power BI – Data visualization  

---

## 🔄 Data Pipeline Workflow

1. Raw data (CSV) stored in AWS S3  
2. Loaded into Snowflake (RAW layer)  
3. Transformed using dbt:
   - **Staging layer** → data cleaning  
   - **Intermediate layer** → joins & transformations  
   - **Mart layer** → business-ready tables  
4. Connected to Power BI for dashboard creation  

models/
│
├── staging/
│ ├── stg_list_of_orders.sql
│ ├── stg_sales_target.sql
│ ├── stg_order_details.sql
│
├── intermediate/
│ ├── int_orders_details.sql
│
├── marts/
│ ├── sales_report.sql
│
└── sources.yml

## 📊 Dashboard Overview
## 📈 Key Insights

- 💰 Total Sales: ₹431.5K  
- 📊 Total Profit: ₹23.96K  
- 📉 Sales trend decreasing over months  
- 🏆 Clothing category generates highest profit  
- 📍 Top-performing states identified  
- 🎯 Gap observed between actual sales and targets  

## 🚀 Key Features

- End-to-end modern data pipeline  
- Modular dbt transformations  
- Scalable cloud data architecture  
- Interactive and dynamic dashboard  
- Business-driven insights  

---

## 🧠 Key Learnings

- Building ELT pipelines using Snowflake & dbt  
- Data modeling using staging, intermediate, and marts  
- Handling data quality issues  
- Creating business dashboards in Power BI  
- Designing clean and professional visualizations  

---

## 🔥 Future Improvements

- Add incremental models in dbt  
- Automate pipeline using Airflow  
- Implement data quality tests  
- Deploy dashboard for real-time analytics  
