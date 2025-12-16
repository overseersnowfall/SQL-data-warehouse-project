# SQL Server Data Warehouse (Guided Learning Project)

## Overview
This repository contains my implementation of a **SQL Server Data Warehouse**
built as part of a guided learning project.

The goal of this project was to understand how a modern data warehouse is
designed and implemented using **SQL Server**, following the **medallion
architecture (Bronze, Silver, Gold)**.

This repository focuses **only on the data warehouse layer**.
Analytics and BI reporting are **not included**.

---

## Project Scope

This project covers:

- Designing a data warehouse architecture using Bronze, Silver, and Gold layers
- Creating schemas to represent each layer
- Loading raw ERP and CRM data from CSV files
- Performing data cleansing and transformations
- Building fact and dimension tables for analytical use
- Applying data warehouse best practices in SQL Server

---

## Data Architecture

The warehouse follows the **Medallion Architecture** pattern:

- **Bronze Layer**
  - Raw data ingested from ERP and CRM CSV files
  - Minimal transformation
  - Append-only tables

- **Silver Layer**
  - Cleaned and standardized data
  - Data quality checks
  - Type casting and normalization

- **Gold Layer**
  - Business-ready data
  - Star schema design
  - Fact and dimension tables optimized for analytics

---

## Data Sources

- **ERP System** (CSV exports)
  - Orders
  - Products
  - Sales transactions

- **CRM System** (CSV exports)
  - Customers
  - Customer attributes

---

## Technologies Used

- SQL Server
- SQL Server Management Studio (SSMS)
- T-SQL
- CSV files as source data
- Draw.io (for architecture and data models)

---

## Repository Structure

sql-server-data-warehouse/
│
├── datasets/ # Raw ERP and CRM CSV files
│
├── docs/ # Architecture and data model documentation
│ ├── data_architecture.drawio
│ ├── data_models.drawio
| ├── data_flow.drawio # Draw.io file for the data flow diagram
| ├── data_catalog.md
│ └── naming-conventions.md # Consistent naming guidelines for tables, columns, and files
│
├── scripts/
│ ├── bronze/ # Raw data ingestion scripts
│ ├── silver/ # Data cleansing and transformation scripts
│ └── gold/ # Fact and dimension table scripts
│
├── README.md
├── LEARNING_SUMMARY.md
├── LICENSE
└── .gitignore


---

## Acknowledgements

This project was completed as a **guided learning implementation** based on the
**SQL Server Data Warehouse Project** by **Data with Baraa**.

The original project concept, architecture, datasets, and SQL logic were
designed by Data with Baraa. This repository represents my own hands-on
implementation for learning and practice purposes.

Original project and tutorial:
- GitHub: https://github.com/DataWithBaraa/sql-data-warehouse-project
- YouTube: https://www.youtube.com/@datawithbaraa

---

## License

This project is licensed under the **MIT License**.
The original work and concept are credited to Data with Baraa.

