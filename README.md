# Global Temperature Analysis with BigQuery and Looker Studio

## Project Overview
This project explores global temperature patterns using Google BigQuery for data preparation and Looker Studio for interactive visualisation. The analysis focuses on three questions:

- How does average temperature differ across countries?
- How has average temperature changed over time?
- Which parts of the world show stronger recent temperature change?

## Project Objective
The goal of this project is to transform raw temperature data into analysis-ready BigQuery tables and views, then use Looker Studio to communicate findings through maps, trend lines, and country comparisons.

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

## BigQuery Data Preparation
The dashboard is supported by a set of tables and views created in BigQuery to organise the data for time-based, country-based, and geographic analysis.

### Tables and Views
- `iso-country-codes`
- `tblAVGTemp190s`
- `tblGeoTemp`
- `tbl_DateTime_AvgTemp`
- `tbl_YearlyAvgTemperature`
- `tbl_YearlyMeanTeamp`

These objects were used to structure the temperature data into reusable reporting layers for Looker Studio.

## Dashboard Views

### 1. Average Temperature by Year and Country
![Average Temperature by Year and Country](https://github.com/user-attachments/assets/993afd1a-85b9-4621-9845-cc51d6dfc1fe)

This dashboard view combines:
- a country comparison chart for India, the United States, and the United Kingdom
- a long-term average temperature trend line with an average reference line

**What this shows**
- India remains the warmest of the three compared countries.
- The United States sits in the middle range.
- The United Kingdom remains the coolest of the three.
- The long-term trend suggests more recent years are often above the historical average.

### 2. Average Temperature Worldwide
![Average Temperature Worldwide](https://github.com/user-attachments/assets/d4d903e7-c41c-484d-8f13-45c86a132893)

This choropleth map shows how average temperature varies across countries worldwide.

**What this shows**
- Average temperature differs significantly by geography.
- Warmer temperatures appear more strongly in lower-latitude and tropical regions.
- Cooler average temperatures are more visible in higher-latitude regions.

### 3. Global Temperature Change Within 10 Years
![Global Temperature Change Within 10 Years](https://github.com/user-attachments/assets/ebef0262-0e3b-45bc-8488-7f853dc64129)

This map highlights temperature change by country over the selected 10-year period.

**What this shows**
- Temperature change is global in scale, but uneven in intensity.
- Many countries show warming over the selected period.
- Some regions appear to change more strongly than others.

## Key Findings
- Temperature patterns differ clearly across countries and world regions.
- India appears consistently warmer than the United States and the United Kingdom in the country comparison chart.
- The long-term average temperature trend suggests a broader warming pattern in more recent years.
- Geography is a major factor in average temperature variation.
- Recent temperature change appears widespread, although the size of change differs by country.

## Repository Contents
- [README.md](./README.md): project overview, dashboard summary, and key findings
- [INSIGHTS_REPORT.md](./INSIGHTS_REPORT.md): detailed interpretation of the dashboard results
- [GlobalTempGSOT.ipynb](./GlobalTempGSOT.ipynb): notebook used to connect to and inspect BigQuery data

## Conclusion
This project demonstrates an end-to-end analytics workflow using Google BigQuery and Looker Studio. It shows how raw global temperature data can be transformed into reporting-ready tables, visualised through interactive dashboards, and interpreted in a clear portfolio-ready format.
