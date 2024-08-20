**Tokyo Olympic Data Analytics | End-To-End Azure Data Engineering Project**


Overview
This project demonstrates an end-to-end data engineering pipeline on Azure for analyzing data related to the Tokyo Olympic Games. The architecture leverages various Azure services to ingest, store, transform, analyze, and visualize data, providing insights through interactive dashboards.
![Architecture](https://github.com/user-attachments/assets/e8f9ad7a-02ae-4953-bfa5-284811f038b6)

Architecture
1. Data Source
Description: The data source represents the raw data related to the Tokyo Olympic Games, which  include 11,000 athelets,with 47 disciplines, along with 743 Teams taking part in the 2021(2020) Tokyo Olympics.This dataset contains the details of the Athletes, Coaches, Teams participating as well as the Entries by gender. It contains their names, countries represented, discipline, gender of competitors, name of the coaches.
Source(Kaggle):[2021 Olympics in Tokyo](https://www.kaggle.com/datasets/arjunprasadsarkhel/2021-olympics-in-tokyo)

3. Data Ingestion
Service: Azure Data Factory
Description: Azure Data Factory is used for orchestrating and automating the data movement from the source into Azure. It facilitates the ETL (Extract, Transform, Load) processes.
Steps:
Connect to various data sources.
Copy the raw data to a centralized data storage.
4. Raw Data Store
Service: Azure Data Lake Gen 2
Description: The raw data is stored in Azure Data Lake Gen 2, a scalable and secure data lake solution for high-volume data storage. The data is stored in its original format for future processing.
5. Data Transformation
Service: Azure Databricks
Description: Azure Databricks is utilized to transform and process the raw data. It enables large-scale data processing using Apache Spark and allows for advanced analytics, machine learning, and real-time streaming.
Steps:
Cleanse and normalize the raw data.
Perform aggregations, computations, and other transformations.
6. Transformed Data Store
Service: Azure Data Lake Gen 2
Description: The transformed data is stored back into Azure Data Lake Gen 2 for further analysis. This allows for separation of raw and processed data.
7. Data Analytics
Service: Azure Synapse Analytics
Description: Azure Synapse Analytics is used to query and analyze the transformed data. It offers an integrated experience for data preparation, management, and serving data for business intelligence.
Steps:
Load transformed data from Azure Data Lake.
Run complex queries and generate insights.
8. Dashboarding and Reporting
Services:
Power BI
Looker Studio
Tableau
Description: The final insights and analytics are visualized using interactive dashboards. These dashboards are created using Power BI, Looker Studio, and Tableau to provide stakeholders with a comprehensive view of the analyzed data.
Features:
Customizable dashboards with real-time data.
Various visualization options to represent the data effectively.
Technologies Used
Azure Data Factory: Data ingestion and ETL processes.
Azure Data Lake Gen 2: Scalable storage for raw and transformed data.
Azure Databricks: Data processing and transformation.
Azure Synapse Analytics: Data analysis and querying.
Power BI, Looker Studio, Tableau: Data visualization and dashboarding.
How to Run the Project
Prerequisites:

Azure Subscription
Access to the necessary data sources (Olympic data)
Azure Databricks, Data Lake, Synapse Analytics, and Data Factory services enabled.
Steps:

Set up Azure Data Factory to ingest data from your data sources into Azure Data Lake Gen 2.
Use Azure Databricks to transform and process the ingested data.
Store the processed data back into Azure Data Lake Gen 2.
Query the processed data using Azure Synapse Analytics to derive insights.
Create dashboards using Power BI, Looker Studio, or Tableau to visualize the data.
Conclusion
This project illustrates how to build a scalable and efficient data engineering pipeline on Azure, leveraging its various services to handle large-scale data from ingestion to visualization. The architecture is modular and can be adapted to various other data engineering use cases beyond Olympic data analytics.

# Tokyo-olympic-azure-data-engineering-project
