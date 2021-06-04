# Sales Forecast Prediction

This task uses a dataset for a large Austrailian company Austral AB with sales data from a 1009 of stores in 20 fictitious towns.

## Problem Description
In uncertain business times, Austral AB would love to have predictable revenue. The revenue is often the starting point for annual plans and budgets affecting the whole organization. Now after the last expansion 2009, where they expanded from 250 to 1009 stores, and with distributed sales teams the future growth strategy highly rely on revenue forecasting.

With sales forecasting they would be able to:
- Make better business decisions for business planning, budgeting and risk management.
- Efficiently allocate resources for future growth and cash flow management.
- Efficiently mange the sales teams achieve their goals by preventative instead of reactive management.
- Estimate costs and revenue accurately, and therefore ability to predict the companys short- and long-term performance.  

However, they noticed that their current short term forecasting is way off the reality and would therefor like some help to predict number of customers and revenue.

## Objective
To predict the number of customers and the sales figures for the time period that follows directly after the time period covered in the dataset (2012-01-01 - 2012-02-03).

# Data
## Data Files
- Train model: `sales_data.csv` (~ 900.000 entries)
- Produce predictions on `sales_data_forecast.csv` (~ 35.000 entries)
- Predictions `sales_data_forecast.csv` with prediction of `n_cust` and `revenue`
- Revenue prediction model errors for each `store_id`: `results_comparison_revenue.csv`
- Nr of customer prediction model errors for each `store_id`: `results_comparison_ncust.csv`

## Features
- `store_id`: An integer ID for each store
- `date`: The date in year-month-day format (string)
- `is_store_open`: Binary variable indicating if the store is open on this date or not (1 = open)
- `is_sale_period`: Binary variable indicating if the store has an ongoing sale (1 = yes)
- `town`: Name of the (fictitious) town

## Target Variables
- `n_cust`: The number of customers who visited the store on the given date
- `revenue`: The total revenue that was earned by the store on the given date

# Script
- `sales_prediction_main.ipynb` is the main script containing all data wrangling and modelling.

# Folder Structure
- Input and output data files are in `data`.
- Generated visualizations are in `visuals`.

# Reports
- `sales_forecast_report.ipynb` is the development report
- The report is also presented as a slideshow in `sales_forecast_report.slides.html`

# Requirements
Python 3.9
Jupyter Notebook
