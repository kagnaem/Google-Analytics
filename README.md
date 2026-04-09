# Global Temperature Analysis with BigQuery and Looker Studio

## Project Overview
This project analyses global temperature data using Google BigQuery for data preparation and querying, and Looker Studio for interactive dashboard visualisation. The project focuses on average temperature patterns across countries, long-term temperature trends, and recent worldwide temperature change.

## Objective
The purpose of this project is to:
- explore historical global temperature data
- prepare reporting-ready tables and views in BigQuery
- compare temperature patterns across countries and regions
- visualise the results in Looker Studio
- communicate insights clearly through charts, tables, and maps

## Tools and Technologies
- Google BigQuery
- SQL
- Looker Studio
- Google Cloud Platform
- Python notebook for data access and exploration

## Data Source and Workspace
- Google Cloud Project: `global-temperature-429612`
- BigQuery Dataset: `GlobalTempGSOD`
- Notebook: [GlobalTempGSOT.ipynb](./GlobalTempGSOT.ipynb)

BigQuery dataset link:
[Open BigQuery Dataset](https://console.cloud.google.com/bigquery?ws=!1m4!1m3!3m2!1sglobal-temperature-429612!2sGlobalTempGSOD)

Looker Studio dashboard:
[Open Dashboard](https://lookerstudio.google.com/u/0/reporting/d3b74624-32d4-4b34-b1aa-13e59c88a68a/page/tEnnC)

## BigQuery Tables and Views
The project uses a combination of tables and views to support trend analysis, date-based aggregation, and geographic reporting.

- `iso-country-codes`
- `tblAVGTemp190s`
- `tblGeoTemp`
- `tbl_DateTime_AvgTemp`
- `tbl_YearlyAvgTemperature`
- `tbl_YearlyMeanTeamp`

These objects help structure the raw temperature data into reusable reporting layers for Looker Studio.

## Dashboard Preview

### 1. Average Temperature Worldwide
![Average Temperature Worldwide](https://github.com/user-attachments/assets/d4d903e7-c41c-484d-8f13-45c86a132893)

This map shows how average temperature varies across countries worldwide and highlights strong regional climate differences.

### 2. Average Temperature by Year and Country
![Average Temperature by Year and Country](https://github.com/user-attachments/assets/993afd1a-85b9-4621-9845-cc51d6dfc1fe)

This dashboard view compares average temperature across selected countries and years and also shows a long-term average temperature trend line.

### 3. Global Temperature Change Within 10 Years
![Global Temperature Change Within 10 Years](https://github.com/user-attachments/assets/ebef0262-0e3b-45bc-8488-7f853dc64129)

This map shows temperature change across countries over a 10-year period and helps identify where warming or cooling is more pronounced.

## Key Insights
- Average temperature differs clearly across countries and regions.
- India appears consistently warmer than the United States and the United Kingdom in the comparison chart.
- The long-term trend suggests recent years are generally warmer than much of the earlier historical series.
- Geographic location strongly influences average temperature.
- Temperature change over the last 10 years appears widespread, but the intensity varies by country.

## Repository Contents
- [README.md](./README.md): project overview and dashboard summary
- [INSIGHTS_REPORT.md](./INSIGHTS_REPORT.md): detailed interpretation of dashboard results
- [GlobalTempGSOT.ipynb](./GlobalTempGSOT.ipynb): notebook used to connect to and inspect BigQuery data

## Conclusion
This project demonstrates an end-to-end analytics workflow using Google BigQuery and Looker Studio. It combines cloud-based querying, data preparation, interactive visualisation, and insight communication in a single portfolio project.
