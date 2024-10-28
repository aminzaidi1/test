# Assignment: Working with Managed No-SQL Databases

## Objective

The objective of this assignment is to introduce you to managed database services in Azure and Google Cloud Platform (GCP). You will learn how to start, stop, and monitor database-related services, including BigQuery and MySQL.

## Dataset

The dataset used for this assignment is a healthcare dataset with the following columns:

| PatientID | Name           | Age | Gender | DiagnosisCode | VisitDate  | Hospital                | TreatmentPlan          | FollowUpDate |
|-----------|----------------|-----|--------|---------------|------------|-------------------------|------------------------|---------------|
| 1         | John Doe      | 45  | M      | M54.5         | 2024-09-10 | Stony Brook Hospital     | Physical Therapy        | 2024-09-20    |
| 2         | Jane Smith    | 29  | F      | E11.9         | 2024-08-15 | Stony Brook Hospital     | Insulin                | 2024-09-15    |
| 3         | Bob Johnson    | 65  | M      | I10           | 2024-10-01 | Long Island Clinic       | Hypertension Medication | 2024-11-01    |
| 4         | Alice Williams  | 50  | F      | J45.909       | 2024-07-22 | Southampton Hospital     | Bronchodilators        | 2024-08-22    |
| 5         | Michael Brown   | 37  | M      | G43.909       | 2024-06-12 | Stony Brook Hospital     | Triptans               |               |
| 6         | Susan Davis    | 54  | F      | I25.10        | 2024-05-10 | Stony Brook Hospital     | Statins                | 2024-06-10    |

## 1. Google BigQuery (GCP)

### Steps to Upload Data
1. Navigate to BigQuery in the Google Cloud Console.
2. Create a new dataset.
3. Upload the healthcare dataset (CSV) into a table within your dataset.
4. Run the SQL query: 

![GCP-1](images\gcp-1.png)

![Query Result](images\gcp-2.png)

## 2. MongoDB Atlas

### Steps to Insert Data

1.  Go to MongoDB Atlas and create a new database instance.
2.  Insert the healthcare dataset into a collection using the following Python script:

![atlas-1](images\atlas-1.png)

![atlas-db](images\atlas-2.png)

## 3. Redis Cloud

### Steps to Insert Data

1.  Sign up for a free tier account on Redis Cloud.
2.  Insert patient data using the following Python script:

![redis-1](images\atlas-1.png)

![redis-upload](images\atlas-2.png)