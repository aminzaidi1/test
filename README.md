# HHA504: Managed No-SQL Databases in Atlas MongoDB, Redis, and GCP BigQuery

## Table of Contents

-   Introduction
-   MongoDB Atlas Setup
    -   Configuration
    -   Connection Details
    -   Monitoring
-   Data Uploads to MongoDB
-   Redis Setup
    -   Configuration
    -   Connection Details
    -   Data Uploads to Redis
-   GCP BigQuery Exploration
    -   Dataset Creation
    -   Query Execution
    -   Cost Monitoring
-   Conclusion

## Introduction

This document outlines my experience with managed No-SQL database services using MongoDB Atlas, Redis, and Google Cloud Platform (GCP) BigQuery. I set up and monitored these databases and conducted data analysis using BigQuery.

## MongoDB Atlas Setup

### Configuration

I created a cluster in **MongoDB Atlas** with the following configuration:

-   **Cluster Name**: hha-non-sql-cluster
-   **Cloud Provider**: AWS
-   **Region**: US East

### Connection Details

-   **Connection String**:
    
    bash
    
    Copy code
    
    `mongodb+srv://admin_super:your_password@hha-non-sql-cluster.mongodb.net/test` 
    
-   **Database Name**: healthcare_db
-   **Collection Name**: patients

  
_Connection details for MongoDB Atlas._

### Monitoring

In MongoDB Atlas, I monitored performance metrics such as CPU usage, memory consumption, and connection count.

![MongoDB Atlas Monitoring](images/atlas-1.png)  
_Monitoring metrics in MongoDB Atlas._

## Data Uploads to MongoDB

Data uploads to MongoDB were performed using the `pymongo` library in Python:

![MongoDB Atlas Monitoring](images/atlas-2.png)  

I prepared a CSV file with patient data to be uploaded into the MongoDB collection.

## Redis Setup

### Configuration

I set up **Redis** to manage in-memory data:

-   **Database Name**: healthcare_redis

### Connection Details

-   **Host**: your_redis_host
-   **Port**: your_redis_port
-   **Password**: your_redis_password

  
_Connection details for Redis._

### Data Uploads to Redis

Data uploads to Redis were executed with the following Python script:


![redis python](images/redis-2.png)  


This script allowed me to upload patient records into Redis efficiently.

## GCP BigQuery Exploration

### Dataset Creation

Moving on to **GCP**, I explored BigQuery by creating a dataset named `healthcare_dataset` and loading a CSV file into a table called `patients_table`.

  
_Creating the dataset and loading data in BigQuery._

### Query Execution

I executed a sample query to retrieve patient information:


![GCP Monitoring](images/gcp-2.png)  


  
_Query results from BigQuery._

![GCP Results](images/gcp-	.png)  


### Cost Monitoring

I tracked costs using the Billing Dashboard, noting that 3.2MB of data was processed under the free tier of 10MB.

## Conclusion

In conclusion, MongoDB Atlas, Redis, and GCP BigQuery provide powerful tools for managing No-SQL databases and conducting data analysis. Each platform offers unique features that cater to different needs, making them suitable for various data management tasks. MongoDB Atlas excels in ease of setup and monitoring, Redis is great for fast, in-memory data management, and GCP BigQuery shines in data analysis capabilities. The choice between these platforms largely depends on specific project requirements and user preferences.
