# Global Temperature Insights Report

## Project Overview
This report summarises insights from the global temperature dashboard built with Google BigQuery and Looker Studio. The dashboard presents three complementary views: country-level comparison, worldwide average temperature mapping, and global temperature change over a recent 10-year period.

The project also includes [qry_DateTime_AvgTemp.sql](./sql/qry_DateTime_AvgTemp.sql), one of the SQL queries used to build the BigQuery tables and views behind the dashboard. This query prepares year-based temperature records, creates a `DATETIME` field for reporting, and calculates temperature change relative to a country baseline.

## 1. Average Temperature by Year and Country

### Result
This view combines a bar chart comparing average temperature for India, the United States, and the United Kingdom across selected years with a long-term average temperature trend line.

### Interpretation and Key Insights
- India is consistently the warmest of the three countries shown in the comparison chart.
- The United States remains in the middle range across the selected years.
- The United Kingdom is the coolest of the three countries shown.
- The long-term trend line fluctuates over time, but recent values tend to sit above the average reference line more often.
- This view is useful because it combines both country comparison and time-trend context in one dashboard section.

## 2. Average Temperature Worldwide

### Result
This choropleth world map displays average temperature levels across countries.

### Interpretation and Key Insights
- Average temperature varies clearly across world regions.
- Warmer average temperatures appear more strongly in lower-latitude and tropical areas.
- Cooler average temperatures are more visible in higher-latitude areas.
- The map shows that location is a major factor in average temperature patterns.
- This view helps readers quickly compare temperature levels on a global scale.

## 3. Global Temperature Change Worldwide Within 10 Years

### Result
This map shows temperature change (`temp_delta`) by country over the selected 10-year period, with a date filter allowing time-based exploration.

### Interpretation and Key Insights
- Temperature change is visible across many parts of the world.
- Many countries appear to show warming during the selected period.
- The level of change is uneven, suggesting that some regions are changing more rapidly than others.
- Some cooler-toned areas indicate weaker change or relative cooling compared with the strongest warming regions.
- The date filter strengthens the dashboard by allowing the user to focus on recent periods rather than only a full historical range.

## Overall Findings
- Global temperature patterns differ strongly by country and region.
- India appears consistently warmer than the United States and the United Kingdom in the comparison chart.
- The long-term trend view suggests a broader warming tendency in more recent years.
- The worldwide temperature map confirms strong geographic differences in average temperature.
- The 10-year change map indicates that recent temperature change is widespread, but not uniform.

## Conclusion
This project provides a clear example of how SQL, BigQuery, and Looker Studio can be used together to turn climate data into a meaningful analytics story. It combines query-driven table creation, visual analysis, and insight communication in a format that is easy for readers to follow on GitHub.
