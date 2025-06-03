# 🏬 Superstore Data Models ETL Pipeline

This project builds an end-to-end ETL (Extract, Transform, Load) pipeline for the WorkSpace Superstore e-commerce dataset. It integrates automated feature engineering using **Featuretools** and cloud-based data warehousing via **Snowflake**, culminating in analytical dashboards created in **Power BI**.
---

## Project Objectives

- Identify high-performing states and products by revenue and profit.
- Determine best-selling and most/least profitable sub-categories.
- Evaluate customer segments and payment preferences.
- Measure shipping efficiency and regional customer spending over time.

---
## Dataset

- **Source**: WorkSpace Superstore (United States)
- Covers: Orders, Customers, Products, Payments, Shipments
---

## Techniques & Tools Used

### ETL Pipeline
- **Extract**: Load CSV data using `pandas`
- **Transform**: Clean and enrich data with `Featuretools` and custom logic
- **Load**: Store into Snowflake using `snowflake-connector-python`

### Data Modeling
- **Star Schema** with `Orders` as fact table
- Dimension tables: `Customer`, `Product`, `Payment`, `Shipment`
- Designed and implemented directly in **Snowflake**

### Feature Engineering
- Deep Feature Synthesis (DFS) via `Featuretools`
- Derived features:
  - `AverageProfitPerProduct`
  - `TotalQuantityPerShipment`
  - `AverageProfitMarginPerCustomer`
  - `NumberOfOrdersPerPayment`
  - `TotalPricePerProduct`
  - and more...

### Visualization
- **Power BI** for dashboards
- Insights on sales, customer segments, product trends, shipping efficiency

---

## Data Governance & Security

- Complies with **GDPR**, **CCPA**, **PDPA**
- Role-based access control in Snowflake (e.g., `ACCOUNTADMIN`, `SECURITYADMIN`)
- Enforced data accuracy, consistency, and completeness standards

---

## Technologies Used

- **Python**, `pandas`, `Featuretools`
- **Snowflake** (data warehousing)
- **Power BI** (dashboarding)
- **Google Colab** (collaborative development)

### Links
- 📊 [Colab Notebook (Feature Engineering)](https://colab.research.google.com/drive/1JS9eJGBSwH4Ox_uoTWNK7cqXT6MwNKlD?usp=sharing)

---

## Conclusion

The pipeline built here demonstrates how modern technologies can be combined to:
- Automate data preparation
- Perform insightful analysis
- Ensure compliance and governance
- Support data-driven business decision-making

> The combination of automation (Featuretools), scalability (Snowflake), and visualization (Power BI) offers a powerful approach for future enterprise data projects.
