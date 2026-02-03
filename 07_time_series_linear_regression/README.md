# Daily Climate - Time Series Forecasting of Daily Temperature
The project demonstrates the process of forecasting time series using regression methods  
The main objective is to show how to combine trends, seasonality, and lag characteristics to create an interpretable and reliable baseline model for time-dependent data

---

## Project Overview

The dataset contains daily weather observations from Delhi, including:

- Mean temperature
- Humidity
- Wind speed
- Atmospheric pressure

The target variable is:

- meantemp - daily mean temperature

The project focuses on one-step-ahead forecasting, where the goal is to predict the next day’s temperature using past information

### Modeling Approach

The project follows a step-by-step modeling strategy:

- Baseline model using the last observed value
- Trend model using a time index
- Trend + seasonality model using Fourier features
- Trend + seasonality + lag model, capturing short-term autocorrelation
- Optional experiment with exogenous weather variables

All models are evaluated using Mean Absolute Error (MAE) on a validation set, and the best model is tested once on a separate test dataset

---

## Files Included

- **07_time_series_linear_regression.ipynb** - main Jupyter Notebook 
- **DailyDelhiClimateTrain.csv** - training dataset
- **DailyDelhiClimateTest.csv** - test dataset
- **README.md** - project description

- ---

## Technologies Used

- **Python 3**  
- **pandas** - data manipulation
- **NumPy**
- **scikit-learn** - linear regression, pipelines, metrics
- **statsmodels** - residual autocorrelation analysis
- **matplotlib** - visualization
- **Jupyter Notebook / JupyterLab**

---

## Results

- Adding trend and yearly seasonality significantly improves performance over the baseline
- Lag features provide the largest performance gain by capturing short-term temperature dependence
- The best model combines:
  - time index (trend)
  - Fourier features (yearly seasonality)
  - lag features (autocorrelation)
- Residual analysis shows no strong remaining autocorrelation, indicating a well-fitted model

---

## How to Run

1. Open `07_time_series_linear_regression.ipynb` in Jupyter Notebook or JupyterLab  
2. Make sure all required libraries are installed
3. Place `DailyDelhiClimateTrain.csv` and `DailyDelhiClimateTest.csv` in the same directory
4. Run the cells from top to bottom  
