# Azure-Olympics2020-Analytics

This project aims to analyze data from the Tokyo 2020 Olympics using various Azure services. The goal is to create a robust data engineering pipeline that ingests, stores, transforms, and visualizes the data to generate actionable insights.

## Dataset
- Athletes: Details of athletes participating in the Tokyo 2020 Olympics.
- Coaches: Information about coaches.
- Entries by Gender: Statistics on the number of entries categorized by gender.
- Teams: Data on participating teams.
- Medal Counts: Medal counts for each country.

## Technology used:
- Azure Data Factory: For orchestrating data ingestion workflows.
- Azure Data Lake Storage Gen2: For scalable and secure data storage.
- Azure Databricks: For data transformation and preparation.
- Azure Synapse: For advanced analytics and data warehousing.
- Power BI: For data visualization and dashboard creation.

## Key Steps:

- Data Ingestion: Set up pipelines in Azure Data Factory to automate the extraction of raw data and load it into Azure Data Lake Storage Gen2. This setup ensured a reliable and scalable method to handle large volumes of different datasets, including athletes' details, coaches' information, team statistics, and medal counts.
- Data Transformation: Once the data was ingested, I utilized Azure Databricks for data transformation. By writing custom notebooks in Databricks and leveraging Apache Spark, I processed the raw data, cleaning and reshaping it to meet analytical needs. This step included handling missing values, normalizing data formats, and performing aggregations and calculations to prepare the data for deeper analysis.
- Database Creation: Created an SQL database in Azure Synapse Analytics from the transformed data. This involved defining schema structures, setting up tables, and populating them with the cleaned data. By doing so, I enabled efficient querying and analysis, making the data accessible for complex analytical operations and insights generation.
- Visualization: Integrated the Synapse SQL database with Power BI using Azure Connectors to design interactive dashboards that visualize key insights from the Tokyo 2020 Olympics data, including medal counts and country performances, and gender-based participation analysis.
