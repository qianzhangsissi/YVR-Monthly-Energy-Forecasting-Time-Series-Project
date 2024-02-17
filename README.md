# YVR Monthly Energy Forecasting Time Series Project

## Project Overview
This project focuses on forecasting monthly energy usage at Vancouver International Airport (YVR) using historical energy consumption data. The objective is to provide YVR with accurate forecasts that can aid in effective energy planning and budgeting.

## Files in the Repository
- `YVR Monthly Energy Forecasting Time Series Project.ipynb`: Jupyter notebook containing the Python code and detailed analysis of the time series forecasting models.
- `Energy use at YVR.csv`: CSV file containing the dataset used for analysis. The data includes monthly energy usage along with other variables that may affect consumption.

## Data Description
The dataset `Energy use at YVR.csv` includes the following columns:
- `month`: The month of the observation.
- `energy`: The amount of energy used in thousands of kWh.
- Additional columns may include weather data, terminal area, and passenger numbers which can influence energy usage.

## Analysis Summary
The analysis involved:
- Exploratory Data Analysis (EDA) to understand the data's characteristics.
- Fitting various time series forecasting models, including Exponential Smoothing (ETS) and Autoregressive Integrated Moving Average (ARIMA).
- Comparing model performances based on Akaike Information Criterion corrected (AICc) and forecast accuracy measures.
- Residual diagnostics to ensure the adequacy of the selected models.

## Key Findings
- The ARIMA(0,1,1)(0,1,1)[12] model was selected as the final model due to its lower AIC value and higher forecast accuracy compared to other models.
- The model effectively captures the seasonal patterns in energy usage and exhibits well-behaved residuals.

## Usage
To run the Jupyter notebook, ensure you have the following:
- Python 3.x installed.
- Required Python packages installed: pandas, numpy, matplotlib, statsmodels, pmdarima, seaborn, jupyter.

You can install the necessary packages using the following command:
```
pip install pandas numpy matplotlib statsmodels pmdarima seaborn jupyter
```

After installing the dependencies, launch Jupyter Notebook and open the `.ipynb` file to view the analysis.

## Recommendations
The analysis provides a robust model for short-term forecasting. It is recommended to periodically re-evaluate the model performance with new data and adjust the parameters accordingly.
