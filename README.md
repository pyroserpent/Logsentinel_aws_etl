# 🚀 AWS Cloud-Based ETL Automation | Data Engineering & Analytics

## 📌 Project Overview
This project showcases my **cloud engineering** and **data analytics** skills by implementing an end-to-end **AWS-based ETL pipeline**. It automates log ingestion, transformation, and querying using **AWS Lambda, Glue, Athena, and CloudWatch**, demonstrating expertise in:

- **Cloud Data Engineering** 🏗️ (AWS Lambda, Glue, Athena, S3)
- **ETL/ELT Pipeline Automation** 🔄 (Extract, Transform, Load)
- **SQL-based Log Analysis** 📊 (Athena Querying)
- **Cloud Monitoring & Alerting** 🚨 (CloudWatch Alarms & Metrics)
- **Infrastructure as Code (IaC)** 🏗️ (IAM Roles, S3 Storage, Logging)

---

## 🏗️ **Cloud Architecture**
```
┌───────────────────────────┐       ┌──────────────────────────┐
│   AWS Lambda (Ingestion)  │  →    │       AWS S3 (Raw Logs)  │
└───────────────────────────┘       └──────────────────────────┘
             │                                 │
             ▼                                 ▼
┌───────────────────────────┐       ┌──────────────────────────┐
│  AWS Glue (ETL Pipeline)  │  →    │   AWS S3 (Processed Logs)│
└───────────────────────────┘       └──────────────────────────┘
             │
             ▼
┌───────────────────────────┐
│    AWS Athena (Querying)  │
└───────────────────────────┘
             │
             ▼
┌───────────────────────────┐
│ AWS CloudWatch (Alerts)  │
└───────────────────────────┘
```

---

## ⚡ **Technology Stack & AWS Services**

✅ **AWS Lambda** → Ingests logs into **S3 (`raw_logs/`)**
✅ **AWS Glue** → Transforms logs and writes to **S3 (`processed_logs/`)**
✅ **AWS Athena** → Enables SQL-based querying of logs in **S3 (`processed_logs/`)**
✅ **AWS CloudWatch** → Monitors logs and triggers alerts for anomalies
✅ **AWS S3** → Stores raw and processed log data
✅ **AWS IAM** → Manages security roles and permissions
✅ **Python (Boto3, PySpark, SQLAlchemy)** → Core ETL scripting & data transformation

---

## 📂 **Project Structure**
```
logsentinel-aws-etl/
│── lambda/                  # AWS Lambda function code
│   ├── log_ingest.py        # Lambda function for S3 ingestion
│── glue/                    # AWS Glue ETL scripts
│   ├── transform.py         # Glue script for processing logs
│── athena/                  # Athena queries
│   ├── queries.sql          # Sample queries for analysis
│── cloudwatch/              # CloudWatch setup scripts
│   ├── cloudwatch_alarm.json # JSON config for alerts
│── data/                    # Sample data (optional)
│── README.md                # Project documentation
│── requirements.txt         # Python dependencies (if any)
│── .gitignore               # Ignore unnecessary files
```

---

## 🚀 **Key Features & Use Cases**

✅ **Log Ingestion Automation** → AWS Lambda captures logs and uploads them to **S3 (`raw_logs/`)**.
✅ **ETL Pipeline Execution** → AWS Glue **cleans, transforms, and processes** logs into structured data.
✅ **SQL-Based Log Analysis** → AWS Athena enables **real-time querying** of logs for analytics.
✅ **Cloud Monitoring & Alerts** → AWS CloudWatch detects anomalies and **sends alerts** for errors.
✅ **Scalable, Serverless Design** → Fully **automated, scalable, and cost-effective cloud-based ETL pipeline**.

---

## 📊 **Athena SQL Queries (Log Analysis Examples)**

**📝 Query 1: Show All Logs**
```sql
SELECT * FROM processed_logs_table LIMIT 10;
```
✅ **Displays the first 10 logs**.

**📝 Query 2: Show Only Errors**
```sql
SELECT * FROM processed_logs_table WHERE level = 'ERROR';
```
✅ **Filters logs where `level = 'ERROR'`**.

**📝 Query 3: Count Logs by Log Level**
```sql
SELECT level, COUNT(*) AS log_count FROM processed_logs_table GROUP BY level;
```
✅ **Counts log occurrences by severity (`INFO`, `ERROR`, `WARNING`, etc.)**.

---

## 🔧 **Setup & Deployment Guide**

### 1️⃣ **Deploy AWS Lambda for Log Ingestion**
1. Upload `log_ingest.py` to **AWS Lambda**.
2. Assign IAM role with S3 write permissions.
3. Test by sending sample log events.

### 2️⃣ **Deploy AWS Glue ETL Job**
1. Upload `transform.py` to **AWS Glue**.
2. Schedule Glue job for periodic execution.
3. Verify processed logs in **S3 (`processed_logs/`)**.

### 3️⃣ **Run SQL Queries in AWS Athena**
1. Create an Athena table from **processed_logs/**.
2. Use `queries.sql` to analyze logs.

### 4️⃣ **Set Up CloudWatch Alerts for Anomalies**
1. Apply **`cloudwatch_alarm.json`** to configure log-based alerts.
2. Get notifications when errors exceed threshold.

---

## 🎯 **Why This Project is Valuable for Employers**
This project demonstrates my ability to:
✅ **Build scalable, cloud-native ETL solutions** using AWS.
✅ **Automate data pipelines** for real-time analytics.
✅ **Write optimized SQL queries** for big data processing.
✅ **Implement cloud monitoring & alerting** to detect system failures.
✅ **Work with AWS IAM, S3, Lambda, Glue, and Athena** professionally.

---

## 🤝 **Let's Connect!**
If you're looking for a **Data Engineer | Cloud Engineer | Data Analyst**, let’s talk!
📩 **[Email](zacafnan@gmail.com)** | 💼 **[LinkedIn](https://www.linkedin.com/in/ziaul-chowdhury-dataandcomputerscience)** | 🌍 **[GitHub](https://github.com/pyroserpent)**
