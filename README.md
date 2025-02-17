# AI-Powered-Demand-Forecasting-System


#### an automated ETL pipeline that predicts future product demand based on historical sales data, external factors, and seasonal trends.

- Extract historical sales data from CSV, a database, or an API.
- Integrate external factors such as:
  - Weather API (temperature, rain)
  - Google Trends API (search interest for the product) - https://pypi.org/project/pytrends/
  - Holiday calendar API (seasonality)
- Store extracted data in PostgreSQL
- Handle missing values, duplicates, and outliers.
- Create useful features:
  - Lag features: Sales from the past 7, 14, 30 days.
  - Rolling averages: Moving averages over different time windows.
  - External influence factors: Weather, holidays.
  - Day of the week, month, seasonality.
- Normalize the data for better model performance.
- Create a Machine Learning Model for Forecasting
  - Prophet (good for time series with seasonality).
  - XGBoost (good for structured data).
  - LSTM (RNN) (deep learning approach).
- Train the model using historical data and evaluate accuracy.
- Automate Predictions and Scheduling (ETL - Loading)
  - Store model predictions in a database.
  - Create a Streamlit dashboard for visualization.
  - Schedule daily runs using Apache Airflow or Prefect.
