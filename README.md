# Sales-Data-Warehouse-Analytics-Case-Study
Designed a SQL-based Sales Data Warehouse from CRM and ERP datasets, using Medallion Architecture and performed advanced analytics including revenue trends, customer segmentation, product performance, and trend analysis to generate actionable business insights.
# 📊 Sales Data Warehouse & Analytics Case Study

## Project Overview

This project demonstrates the end-to-end design of a modern **Sales Data Warehouse** using **SQL** and **Medallion Architecture (Bronze, Silver, Gold)**. CRM and ERP datasets were integrated, transformed into analytics-ready structures, and analyzed to generate actionable business insights for decision-making.

The project covers the complete data lifecycle—from raw data ingestion and cleansing to dimensional modeling and advanced reporting.

---

## Business Problem

Organizations often store sales, customer, and product data across disconnected systems like CRM and ERP, making reliable reporting difficult.

This project solves that by building a centralized data warehouse to:

* Consolidate fragmented sales data
* Improve data quality and consistency
* Enable scalable business reporting
* Support data-driven decisions

---

## Architecture Overview

### Bronze Layer — Raw Data

* Ingested raw CRM and ERP CSV data into staging tables
* Preserved source data for traceability and recovery
* Supported batch ingestion

### Silver Layer — Data Cleaning

Performed data transformation and cleansing:

* Removed duplicates
* Standardized gender, marital status, and country values
* Fixed invalid dates and missing sales values
* Handled null and inconsistent records

### Gold Layer — Analytics Layer

Designed a **Star Schema** optimized for reporting.

**Fact Table**

* `fact_sales`

**Dimension Tables**

* `dim_customers`
* `dim_products`

This structure enabled fast aggregations and analytical reporting.

---

## Tech Stack

* Microsoft SQL Server
* SQL (DDL, DML, ETL)
* Data Warehousing
* Star Schema Modeling
* Stored Procedures
* Analytical Reporting

---

## SQL Concepts Used

* CTEs
* Views
* Stored Procedures
* Aggregate Functions
* Window Functions
* `ROW_NUMBER()`
* `RANK()`
* `LEAD()` / `LAG()`
* Running Totals
* Year-over-Year Analysis

---

## Analytical Focus

### Customer Analytics

Analyzed:

* Total spend
* Order frequency
* Average order value
* Customer lifespan
* Recency

Customer segments:

* VIP Customers
* Regular Customers
* New Customers

### Product Analytics

Measured:

* Revenue contribution
* Product demand
* Customer reach
* Profitability

Product segments:

* High Performers
* Mid-Range
* Low Performers

---

## Key Business Insights

### Overall Performance

Sales analysis (2010–2014) showed:

* **₹29M+ total sales**
* **60,000+ units sold**
* **27,000+ unique orders**
* **295 products**
* **18,000+ customers**
* Average selling price: **₹486**

---

### Customer Insights

* Customer base heavily concentrated in the **United States**
* Top revenue-generating customers: **Nicola Nara** and **Caitlin Henderson**
* Maximum customer lifespan reached **28 years**

This highlights strong long-term retention among high-value customers.

---

### Product Insights

* Largest product category: **Components**
* Highest revenue category: **Bikes (₹28M+)**
* Bikes contributed **96.46%** of total revenue
* Best-performing subcategory: **Road Bikes (₹14M+)**

This indicates heavy revenue concentration in a single category.

---

### Sales Trends

* **2010:** Lowest sales, only 14 customers
* **2013:** Peak sales year with **₹16M+ revenue** and **17,000+ customers**

---

## Strategic Findings

* High dependency on the **Bikes** category creates revenue concentration risk
* Sales heavily concentrated in the **US market**
* A small VIP customer segment generates disproportionately high revenue

These insights suggest opportunities for revenue diversification, geographic expansion, and targeted retention strategies.

---

## Business Impact

This project demonstrates how modern data warehousing helps organizations:

* Centralize enterprise data
* Improve reporting efficiency
* Identify top-performing products and customers
* Detect business risks
* Support strategic growth through analytics
