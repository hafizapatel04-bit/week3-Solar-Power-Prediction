# week3-Solar-Power-Prediction
Solar Power Analytics project combining generation and weather datasets, cleaning them, engineering features, and producing an interactive Streamlit dashboard. It visualizes power trends, temporal patterns, and correlations to help analyze and understand plant performance.**


# **Week 3 – Solar Power Analysis & Dashboard**

This week focuses on preparing the solar power dataset for modeling and building an interactive analytics dashboard.

## **1. Data Preparation**

* Loaded and cleaned generation + weather datasets.
* Merged them on timestamp.
* Handled missing values and inconsistent timestamps.
* Exported the cleaned dataset as `processed.csv`.

## **2. Exploratory Data Analysis (EDA)**

* Examined distributions of power output, irradiance, module temperature, and humidity.
* Visualized daily and hourly production trends.
* Calculated correlations to identify strong predictors of DC power.
* Detected temporal patterns indicating production drop during low irradiance or high temperature.

## **3. Feature Engineering**

* Extracted hour, weekday, month from timestamps.
* Added rolling means (3/6/12 intervals) for smoothing short-term fluctuations.
* Created lag features to capture temporal dependence.

## **4. Modeling**

* Trained baseline models: Linear Regression, Random Forest.
* Tested advanced models: XGBoost and LSTM (time-series).
* Compared metrics such as RMSE and MAE.
* Identified XGBoost as a strong performer on tabular features.

## **5. Dashboard (Streamlit)**

* Built a fully interactive dashboard showing:

  * Time-series power output
  * Hourly production patterns
  * Rolling mean vs power
  * Correlation matrix
* Hosted using a public ngrok link.

## **6. Deliverables**

* `processed.csv`
* `app.py` (Streamlit dashboard)
* `Week3_EDA.ipynb`
* Model evaluation notebook
* README file

You can extend this next week by optimizing the model, adding forecasting, or deploying the dashboard permanently.
