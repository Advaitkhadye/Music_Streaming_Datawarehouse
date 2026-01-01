# 🎧 Music Streaming Data Warehouse using PySpark

## About the Project
This project is a hands-on implementation of a **music streaming data warehouse** built using **PySpark** in **Google Colab**.

The main goal of this project is to take raw, unstructured JSON data (similar to real-world streaming app logs) and convert it into a clean, structured format that can be easily analyzed. Instead of focusing only on analysis, this project emphasizes **how data is engineered at scale** — from ingestion to transformation to analytics.

---

##  Dataset
The dataset used in this project is the **Sparkify Music Dataset**, sourced from Kaggle:

🔗 https://www.kaggle.com/code/yukinagae/sparkify-project-churn-prediction

It includes:
- User activity logs in JSON format  
- Song and artist metadata in JSON format  

These datasets simulate real music streaming application data.

---

## What This Project Does
- Loads raw JSON log files and song metadata  
- Cleans and transforms data using **PySpark**  
- Builds a **Star Schema** for analytics  
- Creates fact and dimension tables  
- Runs analytical queries using **Spark SQL**  
- Visualizes user activity and streaming trends  

---

## Data Modeling – Star Schema
The data warehouse follows a **Star Schema** design:

### Fact Table
- **songplays** – records of user song play events  

### Dimension Tables
- **users** – user information  
- **songs** – song details  
- **artists** – artist information  
- **time** – extracted time attributes (hour, day, week, month, year, weekday)

This structure improves query performance and is widely used in analytics systems.

---

## Why Use a Data Warehouse?
Raw application logs are not optimized for analysis. A data warehouse:
- Reduces data redundancy  
- Makes analytical queries faster  
- Organizes data for business intelligence use cases  

This project demonstrates how real analytics systems are designed in practice.

---

## Why PySpark?
PySpark allows distributed processing of large datasets and is commonly used in data engineering roles.

Compared to Pandas, PySpark:
- Handles large volumes of data efficiently  
- Supports distributed transformations and joins  
- Allows SQL-style queries using Spark SQL  

---

## What I Learned
- Processing semi-structured JSON data  
- Building ETL pipelines using PySpark  
- Designing a Star Schema for analytics  
- Handling data quality issues  
- Creating Spark SQL views  
- Extracting business insights from raw logs  

---

## Project Workflow
1. Load raw JSON data  
2. Parse timestamps and extract time features  
3. Create dimension tables  
4. Build the `songplays` fact table  
5. Register tables as Spark SQL views  
6. Run analytical queries  
7. Visualize streaming trends  

---

## Example Insights
- Peak listening hours  
- Most played songs and artists  
- User activity patterns  
- Streaming traffic trends  

---

## Tech Stack
- PySpark  
- Spark SQL  
- Google Colab  
- Pandas  
- Matplotlib  
- Seaborn  
