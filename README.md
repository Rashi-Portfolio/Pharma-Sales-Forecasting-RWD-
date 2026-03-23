# Pharmaceutical Sales Forecasting & Demand Analysis (Real-World Data)
📌 Forecasted pharmaceutical demand using time-series models to uncover seasonality patterns and enable data-driven supply planning.

## Overview
This project demonstrates how time-series analysis and forecasting can be applied to real-world pharmaceutical Point-of-Sale (POS) data to generate actionable insights for demand planning. The analysis focuses on the M01AB drug category (anti-inflammatory and antirheumatic drugs), using historical sales data to model demand patterns and predict future sales.

## Problem Statement
Pharmaceutical demand is influenced by seasonality, variability, and unexpected disruptions. Traditional planning approaches often fail to capture these dynamics, leading to stock imbalances.  
This project explores how predictive modeling can improve demand forecasting and enable more reliable, data-driven supply planning.

## Data & Scope
- Dataset: Real-world pharmacy POS data (subset of ~600K transactions, 2014–2019)  
- Focus: M01AB drug category  
- Granularity: Daily time-series aggregation  

## Approach

### Data Preparation & Quality Handling
- Structured transactional data into time-series format  
- Validated data consistency and distribution  
- Detected anomalies using IQR-based outlier detection  
- Treated extreme outliers (~45 units vs typical 140–180 range) using rolling mean imputation to preserve continuity  

### Exploratory Analysis
- Historical trend analysis using time-series visualization  
- Seasonality analysis using heatmaps and monthly patterns  
- Identified recurring demand cycles and variability bands  

### Forecasting Models
- Naive baseline model for reference  
- Prophet model to capture trend and seasonality  
- Generated 12-month forward demand forecasts  

## Key Insights
- **Stable baseline demand:** ~140–160 units/month  
- **Seasonal uplift:** 20–30% increase, driving peaks to ~180–210 units  
- **Consistent seasonality:** Demand reliably peaks in July–August (e.g., 211 units in Aug 2016)  
- **Anomaly detection:** Extreme drop to ~45 units (~65–70% below expected levels) indicates potential stockouts or disruptions  
- **Forecast reliability:** Prophet predictions remain within ~140–180 units with ±20–30 unit uncertainty  

## Business Implications & Recommendations
- **Baseline planning:** Maintain inventory aligned to ~150 units/month  
- **Peak preparedness:** Scale supply capacity by 25–35% (up to ~200+ units) ahead of mid-year demand surges  
- **Safety buffers:** Maintain ~20–30 units additional buffer to manage variability  
- **Anomaly monitoring:** Implement early warning systems to detect sharp demand deviations  
- **Proactive planning:** Use forecasting outputs for 3–12 month procurement and supply chain optimization  

## Tools & Technologies
Python, Pandas, Matplotlib, Seaborn, Prophet  

## Conclusion
This project highlights how combining structured data preparation, exploratory analysis, and predictive modeling can transform raw transactional data into strategic insights. The approach demonstrates the importance of seasonality-aware forecasting and robust data handling in enabling proactive, data-driven decision-making in pharmaceutical operations.
