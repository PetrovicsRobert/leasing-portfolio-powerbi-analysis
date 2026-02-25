# Portfolio Risk & Rent Dashboard

## Overview
This repository contains a Power BI dashboard that provides insights into a real estate portfolio, focusing on rental risk and performance metrics. The dashboard includes visualizations and key metrics to help understand total rent, rent per square meter, high-risk leases, lease expiry, and break options.

To open the interactive dashboard, please navigate to `PetrovicsRobert/leasing-portfolio-powerbi-analysis` and click on `leasing-portfolio-powerbi-analysis.pbix`.

## Data Cleaning and Preparation
The data used in this dashboard underwent a cleaning and preparation process, which included:

- Handling missing values and ensuring rental costs and lease dates are complete.  
- Standardizing area measurements to square meters and converting rents to USD using a fixed exchange rate.  
- Creating calculated columns and measures to classify lease risk, break option risk, and high-risk leases.  
- Ensuring the Region column reflects correct country-to-region assignments for accurate filtering.  

## Features

### Key Performance Indicators (KPIs)
- **Total Properties:** Counts all properties in the current filter context.  
- **Total Rent (USD):** Sum of rental cost in USD.  
- **Rent per sqm (USD):** Total rent divided by total area.  
- **High Risk Lease Count:** Number of leases classified as "High Risk".  
- **% of Rent at Risk:** Proportion of total rent at risk.  

### Interactive Slicers
- **Region → Country → City (hierarchical)**  
- **Building Tenure**  
- **Primary Use**  
- **Lease Risk**  

*Slicers allow dynamic filtering across all visuals for detailed analysis.*

### Charts & Visualizations

**Top Row (Column Charts):**  
- Total Annual Rent by Lease Risk (USD)  
- Total Annual Rent by Break Option Risk (USD)  

**Middle Row (Bar Charts):**  
- Rent per sqm (USD) by Lease Risk  
- Top 5 Cities by Rent per sqm (USD)  

**Bottom Row (Data Table):**  
- Columns: Area (sqm), Rental Cost (USD), Rent per sqm (USD), Lease Risk, Break Option Risk, High Risk Lease  

*All charts and tables are interactive and respond to slicer selections.*

## Insights
- **High Rent Risk Concentration:** Properties with leases expiring within one year or without break options represent the highest financial risk.  
- **Top Cities by Rent per sqm:** Certain cities consistently show higher rental efficiency, indicating areas of higher revenue potential.  
- **Break Option Trends:** Properties with upcoming break options ≤1 year are likely to contribute to future volatility in rent income.  
- **Lease Expiry Distribution:** A significant portion of leases expiring within 1–3 years provides opportunities for renegotiation or risk mitigation strategies.  

## Recommendations
- **Prioritize High-Risk Leases:** Focus monitoring and mitigation efforts on leases flagged as “High Risk”.  
- **Optimize Rent per sqm:** Investigate areas with lower rent per sqm to identify potential for operational or pricing improvements.  
- **Plan for Upcoming Break Options:** Develop strategies to manage revenue fluctuations from properties with near-term break options.  
- **Leverage Regional Insights:** Use region and city trends to guide investment or divestment decisions for higher portfolio stability.  

## Technologies & Tools
- **Power BI:** For interactive dashboard creation.  
- **DAX (Data Analysis Expressions):** For calculated columns and measures.  
- **GitHub:** Version control and project documentation.  

## Notes
- All measures and calculated columns automatically respect slicers and filters for dynamic analysis.  
- Currency conversions assume a **static exchange rate** (1 USD = 0.73 local currency).  
- Top 5 cities visualization dynamically updates based on filtered data.
