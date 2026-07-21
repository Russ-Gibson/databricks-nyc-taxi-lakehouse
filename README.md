# NYC Taxi Lakehouse – Databricks SQL ETL Pipeline

## Overview

This project demonstrates a production-style Lakehouse architecture implemented in Databricks using SQL and Delta tables.

The solution follows Medallion architecture principles by separating ingestion, transformation, and analytics into independent layers.

## Architecture

Source Dataset:
samples.nyctaxi.trips
``
Flow:

Bronze → Raw ingestion
Silver → Data cleansing and transformation
Gold → Aggregated business metrics

---

## Technologies

* Databricks Free Edition
* Databricks SQL
* Delta Tables
* SQL Transformations
* Medallion Architecture

---

## Project Structure

01_bronze_ingestion
02_silver_clean_transform
03_gold_business_metrics
04_gold_daily_metrics
05_pipeline_configuration
06_data_quality_validation

---

## Features

### Bronze

* Raw ingestion
* Audit timestamp
* Source lineage

### Silver

* Data quality filtering
* Deduplication

### Gold

* KPI calculations
* Daily trend reporting

### Metadata Layer

* Pipeline configuration table

### Validation

* Quality checks

### Audit Logging

Tracks every pipeline execution, including:

- Pipeline Name
- Layer
- Runtime
- Rows Read
- Rows Written
- Success/Failure Status
- Error Message
- Execution Timestamp

---

## Example Metrics

* Average Fare
* Revenue Trends
* Trip Counts
* Distance Analytics

---

## Future Improvements

* Incremental MERGE loading
* Scheduling
* CI/CD deployment
* Power BI dashboard

## Author

Russell Gibson
