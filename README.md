# Project Title: Building a Delta Lakehouse for Multi-source Data Integration

## Project Overview
In this project, I designed and implemented a Delta Lake-based data lakehouse to integrate and manage diverse data sources efficiently. The project involved creating the following data sources, both batch and real-time, and centralizing them within a unified Delta Lake storage system:

- **The Stores Database (Microsoft SQL Server):** I established a seamless data pipeline to ingest and synchronize data from the Stores database, stored in Microsoft SQL Server, into the Delta Lakehouse. This allowed for real-time access to structured data.

- **E-commerce Transactions (Azure Event Hubs):** I set up data streaming from Azure Event Hubs to Delta Lake, enabling the ingestion of real-time e-commerce transactions data, which was crucial for up-to-date analytics and reporting.

- **E-commerce Website Tracking (Azure Blob Storage):** I implemented a data ingestion process to download website tracking data from Azure Blob Storage, ensuring that valuable user behavior insights were readily available within the Delta Lakehouse.

- **Currency Conversion Data (REST API):** To provide currency conversion capabilities, I established a connection to an external REST API, enabling real-time updates of exchange rates and currency conversion within the Delta Lakehouse.

- **Geo-location Data (HTTP Source):** For geospatial analytics, I designed a mechanism to acquire and integrate geo-location data from an HTTP source, enabling geographic insights in the Delta Lakehouse.

## Project Achievements
- Successfully integrated diverse data sources into a unified Delta Lake storage layer, enabling centralized data management and analysis.
- Implemented robust data pipelines for batch and real-time data ingestion, ensuring data freshness and availability.
- Facilitated real-time analytics and reporting on e-commerce transactions and website tracking data.
- Enhanced data quality and reliability through validation and transformation processes.
- Implemented currency conversion capabilities and enriched analytics with geo-location data.

## Technologies Used
- Delta Lake
- Apache Spark
- Microsoft SQL Server
- Azure Event Hubs
- Azure Blob Storage
- REST API Integration
- HTTP Data Source

## Setting up the project on Azure

1. **Create an Azure Data Factory**:
   Make sure you have an Azure Data Factory instance created in your Azure subscription. If you don't have one, you can create it in the Azure portal.

2. **Set up Azure DevOps**:
   If you don't have an Azure DevOps organization and project, create one. You'll need it for CI/CD.

3. **Connect Azure DevOps to GitHub**:
   In your Azure DevOps project, connect it to your GitHub repository. This allows you to access your ADF pipeline code from Azure DevOps.

4. **Create a Build Pipeline**:
   Set up a build pipeline in Azure DevOps that will compile and package your ADF pipeline code from your GitHub repository. Depending on your ADF project, this might involve tasks like publishing ARM templates, building code, or packaging linked services.

5. **Create a Release Pipeline**:
   Create a release pipeline that defines how your ADF code is deployed to your Azure Data Factory. This typically involves tasks like deploying ARM templates and making any necessary configurations.

6. **Configure CI/CD Triggers**:
   Set up continuous integration and continuous deployment triggers so that your ADF pipelines are automatically updated whenever changes are pushed to your GitHub repository. This ensures that your ADF environment is always up to date with your repository.

7. **Run the Pipeline**:
   Trigger the CI/CD pipeline to run, which will deploy your ADF pipelines to Azure. This can be manually initiated or triggered automatically when changes are pushed to your GitHub repository.

8. **Monitor and Troubleshoot**:
   Monitor the pipeline execution for any errors or issues and troubleshoot them as needed.
