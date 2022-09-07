# **youtube analysis project ETL Pipeline**
An end-to-end ETL Pipeline for Building Data Warehouse and Analytics Platform
## **Table of Contents**
* Architecture Diagram
* References
* License

### **Architecture Diagram**
![Architecture](https://user-images.githubusercontent.com/72258715/188996088-12d48529-8ece-4369-bfca-c83686716c5e.png)
**ETL Flow**
* Data is captured from Kaggle API
* Data collected from the API is uploaded to raw area Amazon s3 bucket
* Lambda function is triggered which reads data from raw area  and apply transformations and move data to the cleansed bucket
* AWS Glue will be used for data integration
* Amazon Athena will be used for querying data
* Finally we will use qicksight for dashboarding and insights
