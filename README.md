# Time-Series-Forecasting-project
Time Series Sales Forecasting
Project Description
A simple time series forecasting project using Python to predict monthly sales data. The notebook analyzes daily sales data (from time_series_sales_data.csv), resamples it to monthly, builds a SARIMA model using auto_arima, forecasts the next 12 months, and evaluates performance.
Key Features

Data preprocessing (date parsing, monthly resampling)
Automatic SARIMA model selection (with seasonal period m=12)
12-month ahead forecasting with confidence intervals
Model evaluation (MAE, RMSE) on last 12 months as test set
Comparison with non-seasonal ARIMA
Visualization of actual vs forecasted sales

Requirements
Bash pip install pandas numpy matplotlib statsmodels pmdarima scikit-learn
Files

time_series_project.ipynb → Main Jupyter notebook
time_series_sales_data.csv → Dataset (daily sales from 2010)

How to Run

Clone the repo
Install dependencies
Open and run the notebook:Bash jupyter notebook time_series_project.ipynb

Results

Best model: Seasonal ARIMA (SARIMA)
Forecast example (2025):
Jan: ~305.39
Feb: ~314.08
...
Dec: ~310.98

Test set performance:
MAE: ~286.43
RMSE: ~16.92


Notes

Model captures monthly seasonality well.
Can be extended with Prophet, LSTM, or external features (e.g., holidays, promotions).
