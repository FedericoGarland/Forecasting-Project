# Automated Time Series Forecasting for Commodity Prices (R, Power BI)

## Overview
Production-ready time series forecasting solution for commodity prices. Processes and models historical price data to enable scalable, automated forecasting and data-driven commercial planning.

An end-to-end forecasting pipeline was designed and built to evaluate multiple time series models, select the best-performing one for each product and generate 12-month forecasts, delivering business-ready outputs through a Power BI dashboard.

The solution is fully automated, integrating model execution into a Power Query ETL pipeline to ensure consistent and up-to-date forecasting results for decision-making.

Key components include:
- Automated model selection across multiple algorithms (ARIMA, ETS, Holt-Winters, TBATS)
- Hyperparameter tuning for ARIMA models
- Forecast evaluation using cross-validation and test set validation (MAPE)
- Generation of 12-month forecasts with comparable outputs across products
- Integration of forecasting results into Power BI via Power Query ETL
- Interactive dashboard for price monitoring and forward-looking decision-making
- End-to-end automation of the forecasting and reporting workflow

---

## Architecture

### Forecasting Pipeline
Raw Time Series Data → Model Selection (R) → Forecast Generation → Power Query ETL → Power BI Dashboard

---

## Dashboard

![Forecast Dashboard](images/forecast_dashboard.png)

The dashboard allows users to:
- Visualize historical prices and forecasts
- Compare model performance
- Evaluate forecast uncertainty
- Monitor expected price trends for decision-making

---

## Business Problem
Agricultural price volatility makes planning difficult for:

- Producers deciding which crops to grow  
- Businesses planning procurement strategies  
- Consumers optimizing purchasing decisions  

Without reliable forecasting, decisions are reactive rather than proactive.

---

## Solution
A fully automated forecasting pipeline was built to:

- Evaluate multiple time series models per product  
- Select the best model based on forecasting accuracy (MAPE)  
- Generate 12-month forecasts  
- Integrate predictions into a Power BI dashboard  
- Enable continuous updates through ETL automation  

---

## Modeling Approach

### Model Selection
For each product, the pipeline:

1. Iterates through multiple models:
   - ARIMA (with hyperparameter tuning)
   - ETS (Exponential Smoothing)
   - Holt-Winters
   - TBATS  

2. Evaluates performance using:
   - Cross-validation (one-step forecasts)
   - Test set validation (multi-step forecasts)

3. Selects the best model based on lowest MAPE

---

### Forecasting
- Generates future price predictions (12 months)
- Includes confidence intervals for uncertainty estimation
- Produces comparable outputs across products

---

## Pipeline Flow
1. Time series data is loaded into R  
2. Models are trained and evaluated per product  
3. Best model is selected based on accuracy  
4. Forecasts are generated  
5. Results are exported to Power BI via Power Query ETL  
6. Dashboard is refreshed automatically  

---

## Tech Stack
- R (Forecasting, Statistical Modeling)
- Power BI (Visualization, Dashboarding)
- Power Query / M (ETL Integration)
- DAX
- Time Series Forecasting
- Cross-Validation

---

## Key Techniques
- Automated model selection across multiple algorithms  
- Hyperparameter tuning for ARIMA models  
- Forecast evaluation using MAPE  
- Integration of data science workflows into BI pipelines  
- End-to-end automation of forecasting and reporting  

---

## Business Value
This solution enables:

- Proactive planning based on expected price movements  
- Identification of high-volatility products  
- Better procurement and production decisions  
- Scalable forecasting across multiple products  

---

## 🔗 Links
- 🚀 [Project Repository](https://github.com/FedericoGarland/Forecasting-Project)
- 🌐 [Portfolio Website](https://federicogarland.github.io/FedericoGarlandWebsite/)
- 💼 [LinkedIn Profile](https://www.linkedin.com/in/federico-garland/)