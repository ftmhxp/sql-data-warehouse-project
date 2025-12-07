# Data Warehouse and Analytics Project

This project demonstrates how raw operational data can be transformed into a high-quality analytical layer using **ETL pipelines**, **dimensional modeling**, and **SQL-based transformations**. It follows best practices such as **star schema design**, **clean staging layers**, and **slowly changing dimensions**.
---
## Data Architecture

This project adopts the Medallion Architecture, consisting of the Bronze, Silver, and Gold layers to ensure data reliability, clarity, and usability across all stages of processing.

### Bronze Layer  
Stores raw, unprocessed data exactly as received from source systems. In this project, data is ingested from CSV files and loaded into SQL Server without modifications.
### Silver Layer  
Applies data cleansing, standardization, and validation. This layer resolves inconsistencies, handles missing values, and prepares the data for integration and modeling.
### Gold Layer  
Contains fully modeled, business-ready data organized into a star schema. This layer supports reporting, analytics, and self-service BI.

---
## Project Overview

This project demonstrates the design and implementation of a modern SQL Server–based data warehouse. It includes:

1. **Data Architecture**: Implementing a structured Medallion Architecture with clearly defined Bronze, Silver, and Gold layers.  
2. **ETL Pipelines**: Extracting raw data from source systems, transforming it, and loading it into the appropriate layers.  
3. **Data Modeling**: Building fact and dimension tables optimized for analytical workloads.  
4. **Analytics and Reporting**: Producing SQL-driven reports and creating dashboards to deliver actionable business insights.  

---
## Project Requirements

### Building the Data Warehouse

#### Objective
Develop a scalable, well-structured data warehouse in SQL Server to consolidate sales data from multiple systems and enable efficient analytical reporting.

### Specifications  
- **Data Sources**: Two independent systems (ERP and CRM), both provided as CSV files.  
- **Data Quality**: Identify and resolve quality issues prior to transformation and modeling.  
- **Integration**: Merge both datasets into a unified, consistent data model suitable for analysis.  
- **Scope**: Focus exclusively on the latest available data; historization is not required for this version.  
- **Documentation**: Provide clear, accessible documentation of the data architecture and data model for both technical and business users.  

---

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and share this project with proper attribution.
