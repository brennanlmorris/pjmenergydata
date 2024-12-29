# Energy Consumption Analysis Project

## Overview
This project analyzes hourly energy consumption data from American Electric Power (AEP) spanning from December 2004 to January 2018. The analysis explores patterns in energy consumption across different time scales including hourly, seasonal, and yearly trends.

## Data Description
- Source: AEP hourly energy consumption data
- Time period: 2004-2018
- Variables: 
  - Datetime: Hourly timestamps
  - AEP_MW: Energy consumption in megawatts
- Total observations: 121,273

## Analysis Steps

### 1. Initial Data Processing
- Converted timestamp data to datetime format
- Created hourly, monthly, and seasonal aggregations
- Calculated basic statistics including mean, standard deviation, min, and max values

### 2. Hourly Pattern Analysis
- Created visualizations of average consumption by hour of day
- Identified peak and off-peak usage hours
- Found significant differences between peak (7am-11pm) and off-peak hours

### 3. Seasonal Analysis
- Conducted one-way ANOVA test showing significant differences between seasons (F-statistic: 4183.76, p-value < 0.001)
- Performed Tukey's HSD test to identify specific seasonal differences
- Key finding: Winter and Summer show highest consumption, with Spring having lowest average consumption

### 4. Time Series Decomposition
- Decomposed data into trend, seasonal, and residual components
- Identified downward trend in consumption over the study period
- Observed consistent seasonal patterns in usage

### 5. Year-over-Year Analysis
- Calculated yearly averages and percentage changes
- Key findings:
  - Highest consumption: 2007 (16,645.52 MW average)
  - Lowest consumption: 2017 (14,483.74 MW average)
  - Notable decrease in 2009 (-7.76%), possibly due to financial crisis
  - Recent uptick in 2018 (+5.57%)

## Technologies Used
- Python
- Libraries: pandas, numpy, matplotlib, seaborn, scipy, statsmodels
- Statistical tests: ANOVA, Tukey's HSD
