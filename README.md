# **Simple Data Engineering Project with E-Commerce Dummy Dataset using PySpark**

---

## **Aim & Description**
This project demonstrates a basic data engineering pipeline using **PySpark** to process medium-sized e-commerce datasets.  
The goal is to extract meaningful insights by cleaning, transforming, joining, and analyzing customer and order data on a **distributed environment using Google Cloud Platform (GCP)**.

---

## **Input Files (Size)**
- **customers_500mb.csv** (~544MB)  
- **orders.csv** (~450MB)
- https://drive.google.com/drive/folders/1TtE_SqPl4K6iQ9CT2A88m5qTUsjPNNaz?usp=sharing

---

## **Source of Data**
The dataset is a dummy e-commerce dataset generated by **Mr. Mayank** from the **Big Data Engineering Course on Udemy**.

---

## **Tools**
- **PySpark**  
- **Google Cloud Storage (GCS)**  
- **Google Cloud Dataproc**  
- **JupyterLab** (via Dataproc Notebooks)

---

## **Pipeline Overview**

1. **Data Ingestion (Read)**  
   Read CSV files from GCS into PySpark DataFrames using a **manually defined schema** for better performance.

2. **Data Cleaning and Transformation**  
   - Handle **date format** and **null values**  
   - Extract `year`, `month`, `dayofmonth`, and `dayname`  
   - Use `groupBy`, `filter`, `aggregate`, `orderBy`, `join`, etc., for basic analysis

3. **Data Output**  
   Save the results in **Parquet format** to GCS for further analysis or reporting.

---

## **Output Folders**
- **recent_inactive_customers**  
- **customers_processed**  
- **customers_orders**
- https://drive.google.com/drive/folders/1TtE_SqPl4K6iQ9CT2A88m5qTUsjPNNaz?usp=sharing

---

> 📝 **Note**:  
> The entire pipeline was developed using **PySpark in JupyterLab**, running on a **Google Cloud Dataproc cluster (non-autoscaling mode)**.  
> The project was implemented using the **free tier credits provided by Google Cloud Platform (GCP)**.  
> Cluster setup details can be found in the screenshot folder (**Config Cluster**).
