# 🛍️ ShoppingMART Data Analytics — End-to-End Microsoft Fabric Project

## 📘 Project Overview

**ShoppingMART Analysis** is a comprehensive data analytics solution built using **Microsoft Fabric**, following the **Medallion Architecture (Bronze → Silver → Gold)**.

This project demonstrates the complete lifecycle of modern data analytics — from **data ingestion and transformation using PySpark notebooks** to **pipeline orchestration** and **interactive Power BI visualizations**, all within a unified Fabric environment.

The goal of this project is to analyze **sales performance**, **customer behavior**, **product engagement**, and **sentiment trends** for a retail store chain using both structured and semi-structured data sources.

---

## 🧩 Project Components

| Component                                 | Type             | Description                                                                                 |
| ----------------------------------------- | ---------------- | ------------------------------------------------------------------------------------------- |
| **ShoppingMart_BronzeLayer**              | Lakehouse        | Raw ingestion zone (Bronze). Stores unprocessed structured and semi-structured data.        |
| **Notebook 1 - Initial Process**          | PySpark Notebook | Performs initial cleaning, standardization, and schema alignment.                           |
| **ShoppingMart_dataBronzeLayer Pipeline** | Fabric Pipeline  | Automates data ingestion from multiple sources using parameters.                            |
| **ShoppingMart_SilverLayer**              | Lakehouse        | Cleaned, validated, and structured dataset for analytics.                                   |
| **Notebook 2 - Further Transformations**  | PySpark Notebook | Performs aggregations, joins, and business-level data modeling.                             |
| **ShoppingMart_GoldLayer**                | Lakehouse        | Final analytics layer with KPIs and summarized data.                                        |
| **Master Pipeline (Run_MasterPipeline)**  | Orchestration    | Combines structured + unstructured ingestion and executes all transformations sequentially. |
| **ShoppingMart_Analysis_KPI's**           | Power BI Report  | Final dashboard visualizing sales, stock, sentiment, and engagement insights.               |

---

## 🧠 Key Features

### 🔹 1. Parameterized Pipelines

* Modular, reusable, and dynamic pipelines for different datasets.
* Handles both structured and semi-structured data seamlessly.

### 🔹 2. Delta Lake Integration

* ACID-compliant storage for reliability.
* Supports incremental data updates without full refreshes.

### 🔹 3. Orchestration with Fabric Pipelines

* End-to-end automation through a master pipeline controlling all sub-pipelines and notebooks.
* Ensures sequential execution: *ingestion → cleaning → aggregation → visualization.*

### 🔹 4. PySpark Transformations

Used Spark DataFrame APIs for:

* Null handling
* Data type casting
* Aggregations (sales by category, region, product, etc.)
* Sentiment and review scoring

### 🔹 5. Business-Focused Dashboard

Power BI dashboard integrated within Fabric workspace, featuring:

* Total Revenue and Product Sales KPIs
* Top 5 Products & Customers
* Sales by Category
* Sentiment Distribution (Positive / Neutral / Negative)
* Stock Quantity Insights
* Sales Trend by Month

---

## 📈 Results & Outcomes

1. Achieved automated data pipeline refresh with **zero manual intervention**.
2. Reduced **data latency** between ingestion and reporting.
3. Generated **clear business insights** on sales, inventory, and customer engagement.
4. Demonstrated a **real-world analytics workflow** integrating both data engineering and business intelligence.

---

### 🧾 Tech Stack

**Microsoft Fabric**, **PySpark**, **Delta Lake**, **Power BI**, **Data Factory Pipelines**, **Medallion Architecture**

---

📍 *This project showcases an end-to-end data analytics workflow within Microsoft Fabric — transforming raw data into actionable insights.*
