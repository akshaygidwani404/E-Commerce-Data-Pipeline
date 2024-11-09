# E-commerce Data Pipeline

![](https://github.com/akshaygidwani404/E-Commerce-Data-Pipeline/blob/main/Images/e-commerce-data-pipeline.png)

This repository contains the code for an E-commerce Data Pipeline built on Databricks using PySpark and SQL. This pipeline processes over 1 million records daily from raw ingestion to curated analytics-ready datasets, implementing a medallion architecture with Bronze, Silver, and Gold layers for efficient data handling and transformation.

## Project Overview
The pipeline processes data from multiple e-commerce data sources, managing it across the following three layers:

**Bronze Layer:** Ingests raw data as-is from source systems.

**Silver Layer:** Cleans and transforms the data, applying necessary joins and business rules.

**Gold Layer:** Curates the data for analysis, building a star schema with fact and dimension tables.
This architecture ensures efficient, scalable processing while preserving the original raw data and providing progressively refined datasets.

## Key Features
- Daily Data Processing: Handles over 1 million records each day.
- Medallion Architecture: Structured in Bronze, Silver, and Gold layers for effective data organization and transformation.
- Slowly Changing Dimensions (SCD) Type 2: Tracks historical changes in dimension tables, preserving data integrity and enabling point-in-time analyses.
- Incremental Loads: Processes only new or updated records to reduce processing time and optimize resource usage.
- Real-Time Insights: Provides timely, curated datasets ready for analysis and visualization.

## Technologies Used
- Databricks: For cloud-based distributed processing and data storage.
- PySpark: For data transformations, joins, and incremental processing.
- SQL: To structure and manage data transformations, especially in the Gold layer.

## Setup and Deployment
1. Clone this repository.
2. Import the notebooks into your Databricks workspace.
3. Ensure access to the necessary data sources and permissions.
4. Execute the notebooks sequentially to process data through each pipeline stage.

## Future Enhancements
- Data Quality Checks: Implement automated checks to ensure data accuracy and completeness.
- Alerting and Monitoring: Add real-time alerts for pipeline performance and data quality issues.
- Additional Sources: Extend pipeline capabilities to handle other e-commerce datasets.
## Contributing
Contributions are welcome! Please open an issue or submit a pull request to contribute.