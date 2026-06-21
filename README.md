# PTAX Dollar Exchange Rate - Data Lakehouse & Volatility Analytics

This repository contains the data engineering and analytics layer of an end-to-end data pipeline. The project captures nested data from the Central Bank of Brazil's API, processes it in a Big Data environment via **Databricks (Apache Spark)** using the Medallion architecture, and consumes the final layer in an executive dashboard in **Power BI Desktop**.

## 🏗️ Data Pipeline Architecture

```text
[Central Bank API] ──> [Bronze: Raw JSON] ──> [Silver: Clean & Cast] ──> [Gold: Window Functions] ──> [Power BI (Star Schema)]
