# Pharmaceutical Sales Forecasting & Demand Analysis (Real-World Data)
📌 This project builds a pharmaceutical sales forecasting model using real-world data, focusing on the M01AB drug category (anti-inflammatory and antirheumatic drugs). Using a subset of transactional data (2014–2019) from a pharmacy Point-of-Sale system, the analysis applies time-series techniques, outlier treatment, and Naive vs Prophet models to predict 12-month demand and uncover seasonality patterns for improved supply planning.

## Objective
To evaluate how different forecasting approaches can improve demand prediction and support data-driven decision-making in pharmaceutical supply planning and inventory management.

## Approach

### Data Preparation
- Aggregated transactional data to monthly time-series format  
- Validated data consistency and structure  
- Identified and treated anomalies using IQR-based outlier detection  

### Outlier Handling
- Detected outliers using Interquartile Range (IQR) method  
- Replaced anomalies using centered rolling mean (window = 3)  
- Preserved time-series continuity while improving data stability  

### Exploratory Analysis
- Historical trend analysis using line charts  
- Seasonality analysis using heatmaps and monthly patterns  
- Identified recurring demand cycles and peak periods  

### Forecasting Models
- **Naive Model:** Baseline assumption using previous observations  
- **Prophet Model:** Captures trend and seasonality for improved forecasting  

## Key Insights
- Baseline demand: ~140-160 units/month  
- Peak demand: ~180-210 units, especially in July–August  
- Seasonal uplift: ~20-30% above baseline  
- Forecast range: ~140-180 units with ±20-30 units uncertainty  
- Identified anomaly (~45 units) indicating potential stockout or disruption  

## Business Impact
- Enables more accurate inventory and procurement planning  
- Supports proactive supply chain decision-making  
- Reduces risk of stockouts and excess inventory  
- Provides a scalable approach for forecasting across drug categories  

## Tools & Technologies
Python, Pandas, Matplotlib, Prophet

## Conclusion
This project demonstrates how combining data preprocessing, exploratory analysis, and time-series forecasting can transform raw sales data into actionable insights. The results highlight the importance of seasonality-aware forecasting and robust data handling in driving effective pharmaceutical demand planning. 
