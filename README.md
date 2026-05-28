# sql-data-warehouse-project
Building a modern data warehouse system with SQL server,including ETL processes, data modelling and analytics
# FinFlow Data Warehouse & Analytics Engineering Project

## Overview

FinFlow is an end-to-end Data Warehouse and Analytics Engineering project that simulates a modern financial transaction platform.

The project demonstrates how transactional OLTP data is transformed into analytics-ready OLAP warehouse structures using ETL pipelines and Medallion Architecture principles.

This project focuses on:

* Data Warehousing
* ETL Pipelines
* OLTP vs OLAP Systems
* Medallion Architecture
* Star Schema Modeling
* Fact & Dimension Tables
* SQL Analytics
* Data Engineering Concepts
* Business Intelligence Workflows

---

# Architecture

```text
FinFlow Application (OLTP)
        ↓
Raw Transactional Data
        ↓
Bronze Layer (Raw Ingestion)
        ↓
Silver Layer (Cleaned & Validated Data)
        ↓
Gold Layer (Business Analytics)
        ↓
Dashboards & Analytical Queries
```

---

# Tech Stack

## Database & Warehousing

* SQL Server
* SQL Server Management Studio (SSMS)

## Data Modeling

* Star Schema
* Fact Tables
* Dimension Tables

## ETL & Transformation

* SQL-based ETL Pipelines
* CTAS (Create Table As Select)
* Data Cleaning & Transformation

## Analytics

* Advanced SQL
* Window Functions
* Aggregations
* Ranking Functions
* Analytical Queries

---

# Project Goals

The goal of this project is to simulate how modern companies process operational transaction data and convert it into analytical warehouse systems for reporting and business insights.

The project demonstrates:

* Separation of Concerns
* Layered Data Architecture
* Warehouse Design
* ETL Pipeline Design
* Data Transformation Workflows
* Analytical Query Optimization

---

# OLTP System

The OLTP layer simulates the operational transaction system of FinFlow.

It contains normalized transactional tables such as:

* Users
* Accounts
* Transactions
* Payments
* Devices

The OLTP system is optimized for:

* Fast inserts
* Real-time updates
* Transaction processing
* ACID consistency

---

# Medallion Architecture

## Bronze Layer

Raw ingested operational data.

Characteristics:

* Minimal transformation
* Historical preservation
* Raw source ingestion
* Append-heavy datasets

Example Tables:

* bronze_transactions
* bronze_users

---

## Silver Layer

Cleaned and validated analytical foundation layer.

Transformations include:

* Data cleaning
* Standardization
* Deduplication
* Validation
* Joining datasets

Example Tables:

* silver_transactions
* silver_users

---

## Gold Layer

Business-ready analytical datasets optimized for reporting and insights.

Example Metrics:

* Monthly Revenue
* Transaction Volume
* User Activity
* Fraud Analytics

Example Tables:

* gold_monthly_revenue
* gold_user_activity
* gold_fraud_metrics

---

# Data Warehouse Design

The warehouse follows a Star Schema architecture.

## Fact Tables

Contain measurable business events.

Examples:

* fact_transactions

## Dimension Tables

Contain descriptive business attributes.

Examples:

* dim_users
* dim_date
* dim_region

---

# ETL Pipeline

The ETL process includes:

## Extract

Extracting raw data from OLTP tables.

## Transform

Applying:

* Cleaning
* Aggregations
* Business Logic
* Standardization
* Denormalization

## Load

Loading transformed datasets into warehouse layers.

---

# Analytical Features

The project includes advanced SQL concepts such as:

* Window Functions
* CTEs
* Recursive CTEs
* Ranking Functions
* Running Totals
* Rolling Aggregations
* Partitioning
* Indexing
* Views
* Materialized-style Aggregations

---

# Learning Outcomes

Through this project I learned:

* Database Architecture
* Data Warehousing Concepts
* ETL Design
* Medallion Architecture
* OLTP vs OLAP Systems
* SQL Optimization
* Warehouse Modeling
* Analytical SQL
* Indexing Internals
* Separation of Concerns Principle

---

# Future Improvements

Potential future enhancements:

* Kafka Streaming Pipelines
* Airflow Orchestration
* Power BI Dashboards
* Incremental ETL
* Partitioned Warehouse Tables
* Columnstore Indexing
* Real-time Analytics Pipelines

---

# Project Status

🚧 Currently In Development

This project is being actively built while learning modern Data Engineering and Warehouse Architecture concepts.

---

# Author

Abhinav Bora
