# Time Series Analysis for Temperature Prediction
## Project Overview
This project focuses on predicting temperature trends in Delhi using time series analysis. The analysis leverages various statistical models, including ARMA, ARIMA, SARIMA, and Facebook Prophet, to enhance prediction accuracy. The project also explores the impact of additional factors such as humidity, windspeed, and mean pressure on temperature forecasting.

## Dataset
* Name: DailyDelhiClimate
* Source: [[Link to dataset]](https://www.kaggle.com/datasets/sumanthvrao/daily-climate-time-series-data)
* Description: The dataset contains daily climate data from Delhi, including temperature, humidity, windspeed, and pressure.
## Methodology
### 1. Data Preprocessing
**Loading Data**:  Imported and cleaned the dataset.\
**Resampling**: Converted daily data to weekly frequency.
### 2. Model Development
**ARMA Model**: Applied ARMA model with parameters optimized using ACF and PACF plots.\
**ARIMA & SARIMA Models**: Used auto_arima for parameter tuning.\
**Facebook Prophet**: Integrated additional features like humidity, windspeed, and mean pressure for multivariate forecasting.
### 3. Model Evaluation
**Metrics Used**: Mean Absolute Error (MAE), Akaike Information Criterion (AIC).\
**Best Model**: ARMA(2,6) with the lowest AIC, achieving the best performance.
### 4. Forecasting
**Forecast Horizon**: Next two months.\
**Visualization**: Plotted forecasted temperatures alongside historical data.
### Results
**Best Model**: ARMA(2,6) with the lowest AIC.\
**Performance**: Achieved an MAE of 5.35.\
**Forecasting**: Successfully predicted temperatures for the next two months using the best-fit model.
### Additional Analysis
**Multivariate Analysis**: Enhanced forecast accuracy by including humidity, windspeed, and mean pressure using Facebook Prophet.

### Requirements
Python 3.x\
Libraries: pandas, numpy, matplotlib, statsmodels, fbprophet, pmdarima
