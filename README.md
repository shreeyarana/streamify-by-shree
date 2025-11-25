# Streamify: End-to-End Data Engineering Pipeline

This is created by **Shreeya Rana**.

The project demonstrates an end-to-end data pipeline architecture using **Kafka**, **Airflow**, **Spark Streaming**, **dbt**, and **BigQuery**, covering data ingestion, transformation, and analytics.  

---

### 📘 About Me
I’m **Shreeya Rana**, a data enthusiast with interests in:
- **Data Engineering & Analytics**
- **ETL & Data Pipelines**
- **BigQuery, SQL, and Airflow**
- **Real-time Data Streaming (Kafka)**
- **Machine Learning & Predictive Analytics**

This repository showcases these skills.
A data pipeline with Kafka, Spark Streaming, dbt, Docker, Airflow, Terraform, GCP and much more!

## Description

### Objective

The project will stream events generated from a fake music streaming service (like Spotify) and create a data pipeline that consumes the real-time data. The data coming in would be similar to an event of a user listening to a song, navigating on the website, authenticating. The data would be processed in real-time and stored to the data lake periodically (every two minutes). The hourly batch job will then consume this data, apply transformations, and create the desired tables for our dashboard to generate analytics. We will try to analyze metrics like popular songs, active users, user demographics etc.

### Dataset

This project uses the **Eventsim** data generator to simulate user song-play events for a music streaming platform.  

In this repository, the `eventsim` folder is not included to keep the repository lightweight and GitHub-friendly.  

Eventsim typically uses song metadata from the [Million Songs Dataset](http://millionsongdataset.com) to simulate realistic user behavior.  
I have used a [subset](http://millionsongdataset.com/pages/getting-dataset/#subset) of 10000 songs.



### Tools & Technologies

- Cloud - [**Google Cloud Platform**](https://cloud.google.com)
- Infrastructure as Code software - [**Terraform**](https://www.terraform.io)
- Containerization - [**Docker**](https://www.docker.com), [**Docker Compose**](https://docs.docker.com/compose/)
- Stream Processing - [**Kafka**](https://kafka.apache.org), [**Spark Streaming**](https://spark.apache.org/docs/latest/streaming-programming-guide.html)
- Orchestration - [**Airflow**](https://airflow.apache.org)
- Transformation - [**dbt**](https://www.getdbt.com)
- Data Lake - [**Google Cloud Storage**](https://cloud.google.com/storage)
- Data Warehouse - [**BigQuery**](https://cloud.google.com/bigquery)
- Data Visualization - [**Data Studio**](https://datastudio.google.com/overview)
- Language - [**Python**](https://www.python.org)

### Architecture

![streamify-architecture](images/Streamify-Architecture.jpg)

### Final Result

![dashboard](images/dashboard.png)

### How can I make this better?!
- Choose managed Infra
  - Cloud Composer for Airflow
  - Confluent Cloud for Kafka
- Write data quality tests
- Include CI/CD
- Add more visualizations
