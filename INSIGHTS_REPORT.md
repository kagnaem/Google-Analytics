# Global Temperature Insights Report

## Project Overview
This report summarises insights from the global temperature dashboard built with Google BigQuery and Looker Studio. The dashboard explores average temperature by country, long-term temperature trends, and global temperature change over a 10-year period.

## 1. Average Temperature by Year and Country

### Result
This view compares average temperature for selected countries across several years and includes a long-term average temperature trend line.

### Interpretation and Key Insights
- India shows the highest average temperature among the countries displayed.
- The United States sits in the middle range across the selected years.
- The United Kingdom has the lowest average temperature among the three compared countries.
- The differences between countries remain clear across the selected years, showing stable climate contrasts by location.
- The trend line suggests that more recent years are generally above the long-run average.

## 2. Average Temperature Worldwide

### Result
This world map visualises average temperature levels across countries.

### Interpretation and Key Insights
- Average temperature varies strongly across world regions.
- Warmer countries tend to cluster around tropical and lower-latitude zones.
- Cooler temperatures are more visible in higher-latitude regions.
- Geography appears to be a major driver of global temperature variation.
- The map provides an intuitive overview of how unevenly average temperature is distributed worldwide.

## 3. Global Temperature Change Worldwide Within 10 Years

### Result
This map displays temperature change (`temp_delta`) across countries over a 10-year period.

### Interpretation and Key Insights
- Many countries show positive temperature change, indicating warming over the selected period.
- The magnitude of change is uneven, which suggests that climate impacts vary by region.
- Some northern and polar-adjacent regions appear to show stronger increases.
- A smaller number of countries show weaker change or cooling relative to others.
- The map supports the view that temperature change is global in scale, but not uniform in intensity.

## Overall Findings
- Global temperature patterns differ clearly by geography.
- Historical trend analysis suggests a warming tendency in more recent years.
- The dashboard combines country comparison, world mapping, and time trends to provide a broad view of global temperature behaviour.
- BigQuery enabled structured preparation of analysis-ready tables and views for reporting.
- Looker Studio made it possible to communicate the results through interactive visual analytics.

## Conclusion
This project provides a complete example of cloud-based analytics using Google BigQuery and Looker Studio. It shows how raw climate data can be transformed into meaningful reporting outputs that help readers understand both long-term patterns and recent global temperature change.
