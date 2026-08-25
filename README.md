# Fraud Detection System

A cloud-native **Fraud Detection System** developed to identify high-risk financial transactions using Big Data technologies and machine learning.

The project processes **1,000,000 synthetic transactions** using **AWS S3, Databricks, Apache Spark, and PySpark**. A Medallion Architecture is used to manage the data workflow from raw data ingestion through processing and analysis.

## Technologies Used

* **AWS S3** – Cloud data lake and data storage
* **Databricks / Apache Spark** – Distributed data processing
* **PySpark** – Data preprocessing and feature engineering
* **Gradient-Boosted Trees (GBT)** – Machine learning classification
* **StandardScaler & VectorAssembler** – ML pipeline preprocessing
* **Power BI** – Fraud analytics and dashboard visualisation
* **Parquet** – Efficient columnar data storage

## Key Features

* Processing of 1 million synthetic transactions
* Temporal and behavioural feature engineering
* Fraud-risk prediction using Gradient-Boosted Trees
* Handling of highly imbalanced fraud data
* Evaluation using **AUPRC** alongside accuracy
* Power BI dashboard for fraud-risk analysis
* Cloud-native Medallion Architecture
* Security, privacy, fairness, and human-accountability considerations

## Model Performance

The GBT model achieved:

* **Accuracy:** 94.2%
* **AUPRC:** 0.2979

AUPRC was selected as an important evaluation metric because fraud represents a minority class, making accuracy alone insufficient for evaluating fraud detection performance.

## Project Architecture

**AWS S3 → Databricks/Apache Spark → PySpark Feature Engineering → GBT Machine Learning Pipeline → Power BI Dashboard**

The architecture follows a Medallion approach, moving data from the Bronze layer through processing in the Silver layer to business visualisation in the Gold layer.

## Future Improvements

Future development could include Spark Structured Streaming for real-time fraud intervention, Delta Lake for ACID transactions, automated hyperparameter tuning, and SHAP-based model explainability.
