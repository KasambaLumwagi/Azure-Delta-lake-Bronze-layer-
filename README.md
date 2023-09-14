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
