# PM_Accelerator

In this project I create a weather forecasting ARIMA model given data from World Weather Repository (https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository?resource=download).

Methodology

1. Read in the csv data to create a pandas dataframe with last_updated as the index column (the time that row of data was last updated).
2. Perform data cleaning by dropping the rows with missing values and removing outliers with the interquartile method.
3. EDA: Find correlations between columns and provide visualizations for temperature and precipitation.
4. Split the cleaned dataframe into training and test data and build the ARIMA model on the temperature column.
5. Get model predictions and evaluate its performance with root mean squared error and mean absolute error.

Results

RMSE: 9.015394134633288
MAE: 6.699250035618072

Given that these errors are in the unit of the dependent variable which is temperature, the model's predictions are not bad.
