# 🛒 E-Commerce End-to-End Business Intelligence Platform

An enterprise-grade Data Warehousing and Business Intelligence solution designed to extract, transform, and model e-commerce transactional data into actionable analytical insights.

## 🏗️ Architecture & Project Structure
The project is structurally organized into dedicated layers to follow best engineering practices:
- 📂 **SSIS_Packages/**: Contains the core ETL framework with multi-layered pipelines (STG, ODS, DWH).
- 📂 **SSAS_Project/**: Multi-dimensional Semantic Layer built using SQL Server Analysis Services for fast querying.
- 📂 **Bi_Reports/**: Interactive Power BI dashboards leveraging the SSAS Cubes.
- 📂 **Scripts/**: Database schema files and staging optimization scripts.
- 📂 **Architecture/**: Data Lineage and Control Flow diagrams.

## ⚡ ETL Lifecycle (SSIS)
The ETL pipeline handles complex corporate transformations using **Microsoft SSIS**:
1. **STG (Staging)**: Raw, non-blocking ingestion of transnational data.
2. **ODS (Operational Data Store)**: Data cleaning, structural synchronization, and constraint checks.
3. **DWH (Data Warehouse)**: Population of the Dimensional Model (Star Schema) via optimized incremental loads.

## 📊 Semantic Modeling (SSAS)
- Star Schema design with optimized Fact and Dimension relationships.
- Pre-aggregated measures and hierarchies for sub-second analytical processing.
