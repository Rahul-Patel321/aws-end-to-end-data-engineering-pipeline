# AWS End-to-End Data Engineering Pipeline

![AWS](https://img.shields.io/badge/AWS-Cloud-orange)
![PySpark](https://img.shields.io/badge/PySpark-BigData-red)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![Redshift](https://img.shields.io/badge/Amazon-Redshift-red)
![Athena](https://img.shields.io/badge/AWS-Athena-blue)
![PowerBI](https://img.shields.io/badge/Power-BI-yellow)

## Project Overview

This project demonstrates a production-ready AWS Data Engineering Pipeline designed to ingest, process, transform, and analyze large-scale transactional datasets using AWS cloud services.

The solution follows a modern Medallion Architecture (Bronze, Silver, Gold) and automates the complete ETL workflow using AWS Glue, PySpark, Amazon Redshift, Amazon Athena, AWS Step Functions, and Power BI.

The primary objective is to convert raw business data into analytics-ready datasets that support reporting and business intelligence.

---

## Architecture

```
                  CSV Dataset
                       │
                       ▼
                  Amazon S3
                       │
                       ▼
             AWS Glue Crawler
                       │
                       ▼
              Glue Data Catalog
                       │
                       ▼
              AWS Glue ETL Jobs
                  (PySpark)
                       │
          ┌────────────┴────────────┐
          ▼                         ▼
   Processed S3              Amazon Redshift
          │                         │
          ▼                         ▼
     Amazon Athena          Power BI Dashboard
```

---

## Tech Stack

- Amazon S3
- AWS Glue
- AWS Glue Crawlers
- AWS Glue Data Catalog
- Amazon Redshift
- Amazon Athena
- AWS Lambda
- AWS Step Functions
- Python
- PySpark
- SQL
- Power BI

---

## Dataset

Brazilian E-Commerce Public Dataset by Olist

Tables include:

- Customers
- Orders
- Order Items
- Products
- Sellers
- Payments
- Reviews
- Geolocation

---

## Project Workflow

1. Upload raw CSV files to Amazon S3.
2. AWS Glue Crawlers automatically discover schemas.
3. AWS Glue Catalog stores metadata.
4. AWS Glue ETL jobs transform raw datasets using PySpark.
5. Curated datasets are loaded into Amazon Redshift.
6. Amazon Athena enables serverless SQL querying.
7. Power BI dashboards provide business insights.

---

## Features

- End-to-End ETL Pipeline
- AWS Cloud Native Architecture
- Medallion Data Architecture
- Automated Data Ingestion
- Data Cleansing
- Data Transformation
- Dimensional Data Modeling
- Data Quality Validation
- Logging
- Monitoring
- Power BI Reporting

---

## Folder Structure

```
architecture/
data/
glue_jobs/
sql/
lambda/
step_functions/
dashboards/
docs/
```

---

## Future Enhancements

- Incremental Loading
- Change Data Capture (CDC)
- Apache Iceberg
- Terraform Deployment
- GitHub Actions CI/CD
- Real-Time Streaming using Kafka

---

## Author

Rahul Patel

Senior Data Engineer

LinkedIn:
https://www.linkedin.com/in/rahul-patel-data-engineer/

Portfolio:
https://rahul-patel321.github.io/RahulPatelAnalyst.github.io/
