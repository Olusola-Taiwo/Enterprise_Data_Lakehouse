📦 Modern Sales Data Lakehouse Project
🏗️ Architecture



📘 Project Overview
This project implements a modern Data Lakehouse using Databricks, designed to consolidate ERP and CRM customer‑transaction data into a governed, analytics‑ready environment.
It follows the Bronze → Silver → Gold refinement pattern, with Unity Catalog providing governance, lineage, and access control.

📋 Project Requirements
Data Sources: ERP & CRM CSV datasets

Bronze Layer: Raw ingestion with schema preservation

Silver Layer: Cleansing, standardisation, deduplication, date parsing, phone normalisation

Integration: Unified customer model combining ERP + CRM

Gold Layer: Dimensional model (FactSales, DimCustomer) for BI

Governance: Unity Catalog for metadata, lineage, RBAC

Analytics: SQL Warehouse for dashboards and reporting

📁 Repository Structure
Code
data-warehouse-project/
│
├── datasets/                     # Raw ERP & CRM CSV files
│
├── docs/                         # Architecture, data models, catalog, naming conventions
│   ├── data_architecture.drawio
│   ├── data_models.drawio
│   ├── data_catalog.md
│   └── naming-conventions.md
│
├── scripts/
│   ├── bronze/                   # Raw ingestion scripts
│   ├── silver/                   # Cleansing & integration scripts
│   └── gold/                     # Dimensional model scripts
│
├── tests/                        # Data quality & validation tests
│
├── README.md                     # Project overview
├── LICENSE
└── requirements.txt              # Dependencies
