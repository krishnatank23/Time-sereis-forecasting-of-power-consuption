Tetuan City Power Consumption Forecasting

This project focuses on forecasting power consumption across three zones of Tetuan City using historical energy, weather, and environmental data. The aim is to analyze consumption patterns, understand the impact of weather, and build models to predict future power demand. The insights can help in energy planning, load management, and sustainability initiatives.

📂 Dataset

The project uses the Tetuan City Power Consumption dataset, which includes:

DateTime – Timestamp of readings

Zone 1, Zone 2, Zone 3 – Power consumption per zone

Temperature, Humidity, Wind Speed – Weather data

Diffuse Flows & General Diffuse Flows – Environmental factors

The data is resampled hourly and cleaned to handle missing timestamps.

🔍 Exploratory Data Analysis (EDA)

Trend Analysis: Visualized power consumption per zone over time

Weather Impact: Studied correlations between temperature, humidity, wind, and consumption

Scatterplots & Heatmaps: Compared zones and examined feature correlations

Decomposition: Analyzed seasonal, trend, and residual components

🛠️ Methodology
Data Preprocessing

Parsed DateTime and resampled hourly

Handled missing values

Normalized and scaled features

Feature Engineering

Calculated hourly weather statistics (mean, max, min)

Aggregated zone-wise consumption

Differenced series for stationarity

Stationarity & Autocorrelation

ADF Test for stationarity

ACF & PACF plots to identify patterns

Modeling

Time Series Models: ARIMA, SARIMA

Machine Learning Models: Random Forest, XGBoost

Deep Learning Models: LSTM using PyTorch

Evaluation Metrics

RMSE – Root Mean Squared Error

MAE – Mean Absolute Error

MAPE – Mean Absolute Percentage Error

R² Score – Coefficient of determination

📊 Key Findings

Temperature and humidity significantly affect energy consumption

Zone 1 shows more seasonal fluctuations than Zones 2 and 3

SARIMA and XGBoost performed well for short-term forecasts

LSTM models captured complex temporal dependencies

🖥️ Tech Stack

Languages & Libraries: Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels, XGBoost, PyTorch

Tools: Google Colab / Jupyter Notebook

Visualizations: Heatmaps, scatter plots, and time series trends# Time-sereis-forecasting-of-power-consuption
