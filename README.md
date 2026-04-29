# SQL Data Warehouse Project

Built a data warehouse in SQL Server using the Medallion Architecture (Bronze → Silver → Gold), going from raw CSV files to a clean star schema ready for analytics. The goal was to get hands-on with warehouse design patterns end-to-end — ingestion, transformation, modeling, and querying.

---

## Architecture

Three-layer Medallion Architecture:

| Layer | What it does |
|-------|-------------|
| **Bronze** | Raw CSV data loaded as-is into SQL Server — no transformations |
| **Silver** | Cleansing, standardization, and normalization |
| **Gold** | Star schema (fact + dimension tables) ready for reporting |

---

## What's in here

**ETL pipelines** — scripts to ingest, clean, and model data across all three layers

**Data modeling** — fact and dimension tables built for analytical queries across customer, product, and sales domains

**Analytics** — SQL queries for customer behavior, product performance, and sales trends

**Source data** — two CSV files merged into a single unified model

---

## Stack

- SQL Server Express
- SQL Server Management Studio (SSMS)

---

## Repo structure

```
├── datasets/          # Source CSV files
├── scripts/
│   ├── bronze/        # Raw ingestion
│   ├── silver/        # Cleaning + transformation
│   └── gold/          # Star schema models
└── tests/             # Data quality checks
```
