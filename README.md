# Electricity Consumption Forecasting

## Project Overview
This project focuses on forecasting electricity demand using time series analysis. By leveraging historical power consumption data and weather conditions, the model aims to predict future electricity usage for better energy planning and resource optimization.

## Dataset
- **Source:** Kaggle
- **Timeframe:** 5-minute intervals (2021-2024)
- **Features:**
  - Power Demand
  - Temperature
  - Humidity
  - Wind Speed
  - Pressure

## Data Preprocessing
- Handled missing values using interpolation and forward-filling.
- Renamed columns for clarity.
- Resampled data from 5-minute intervals to daily frequency.
- Set the timestamp as the index for time series analysis.

## Exploratory Data Analysis
- Seasonal trends observed with peaks in extreme weather conditions.
- Correlation analysis showed:
  - **Positive correlation** with temperature (0.40) and wind speed (0.24).
  - **Negative correlation** with pressure (-0.39).
- Moving averages and trend decomposition used to visualize patterns.

## Model Selection
- Explored multiple forecasting models and found **SARIMA** to be the best fit.
- SARIMA captures seasonality, trends, and dependencies in the data.
- Hyperparameter tuning done using ACF/PACF plots.

## Model Performance
- **Mean Absolute Error (MAE):** 287,249
- **Mean Squared Error (MSE):** 139,283,540,200
- **Root Mean Squared Error (RMSE):** 373,207
- **Mean Absolute Percentage Error (MAPE):** 38.12%
- Model captures general trends but struggles with extreme fluctuations.

## Key Insights & Recommendations
- Frequent power demand spikes and zero values may indicate power outages or data issues.
- Further analysis is needed to identify causes of sudden drops in power demand.
- Incorporating external factors (e.g., economic activity, industrial usage) may improve forecasting accuracy.
- Future work includes hybrid models SARIMA

## How to Use This Repository
1. Clone or download the repository.
2. Open the Jupyter Notebook to explore data preprocessing, EDA, and model training.
3. Install dependencies using `pip install -r requirements.txt`.
4. Run the notebook to train the model and visualize results.

## Contact
For any inquiries, reach out via GitHub Issues or email.
dhwanizala25@gmail.com

---

**Author:** [Dhwani Zala]  
**Date:** April 2025

