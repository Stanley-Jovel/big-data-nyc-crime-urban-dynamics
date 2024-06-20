# Mapping Urban Dynamics: Crime, Property, Subway Ridership, and Business in New York City

## Overview

This project investigates the relationships between crime rates, property values, subway ridership, and business perceptions in New York City. By integrating multiple datasets, we aim to provide valuable insights for pedestrians, homeowners, policymakers, and urban planners.

See [project paper here](/BDAD_Project_Report.pdf)

## Data Sources

- NYPD Complaint Data: Incident reports from the NYPD 911 system.
- Google Local Data: Business reviews and metadata from Google Maps.
- NYC Property Valuation and Assessment Data: Detailed property valuation and assessment information.
- MTA Subway Hourly Ridership Data: Hourly ridership data for NYC subway stations.

## Technologies Used

- Apache Zeppelin: For interactive data analysis and visualization.
- Hive & Presto: For data querying and integration.
- Spark SQL & Spark DataFrames: For data processing and analysis.
- Tableau: For creating visualizations and dashboards.

## Key Findings

1. Crime and Businesses: Higher crime rates correlate with businesses that have high foot traffic and cash transactions, such as restaurants and shops.
2. Crime and Customer Sentiment: Mixed correlations between crime rates and business reviews, varying by neighborhood.
3. Crime and Subway Ridership: Positive correlation between ridership and crime complaints, particularly in high-traffic areas.
4. Crime and Property Values: Weak negative correlation between crime rates and property values, with variations across different boroughs.

## Implementation

### Data Ingestion

Datasets were imported into HDFS using Spark jobs and SparkSQL for pre-processing. Missing values, such as zip codes, were filled using latitude and longitude mappings.

### Data Processing

Data cleaning and profiling were performed in Zeppelin notebooks. Common pre-processing steps included:

- Loading raw data into DataFrames
- Standardizing data formats
- Handling missing values
- Validating data integrity

### Data Analysis

Datasets were merged based on zip codes to generate statistical insights. Spark SQL and Hive were used for querying data, and Tableau was used for visualizations.

## Results

Detailed analyses were conducted to explore the impact of crime on businesses, subway ridership, and property values. Significant patterns and correlations were identified, providing actionable insights for improving public safety, real estate decisions, and urban planning strategies.

## Acknowledgements

We thank New York University for providing resources and support, including a free student license for Tableau and access to the NYU HPC Dataproc cluster. Special thanks to Professor Yang Tang for his guidance.

For more detailed information, please refer to the [project paper](/BDAD_Project_Report.pdf) and analysis notebooks in this repository.
