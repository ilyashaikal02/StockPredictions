# StockPredictions

Abstract

There are a few ways of predicting stock prices. From blind guessing to machine learning, many techniques have been tested to try to achieve decent results. Capturing the complexity of the market in a model is a daunting task but it can be broken down in a number of approaches.

Since predicting the exact percent increase of a stock the next day is difficult, i can instead try instead to predict the direction of the movement. Alternatively, i can look at the trends and seasonality in the data and try to predict with some level of confidence where the price would like in an arbitrary number of days.

The logistic models which try to predict the direction of the next day’s movement yielded poor results. Hardly any of the predictor variable were significant, and the classification accuracies were around 52% which is hardly better than guessing. Panel Regression as well as the autoregressive models using ARIMA attempt to predict closing prices of stocks using one stock at a time. Panel Regression attempts to build one model for any number of stocks across the same time periods. Doing this also yielded poor and sporadic results when predicting per stock. On the other hand, the auto-regressive models that predict subsequent values of a stock time series were of greater use. This required finding a suitable combination of parameters to fit the data closely.

Dataset : 

This dataset provides free end of day data for all stocks currently in the Dow Jones Industrial Average. For each of the 30 components of the index, there is one CSV file named by the stock's symbol (e.g. AAPL for Apple). Each file provides historically adjusted market-wide data (daily, max. 5 years back). 

- 30 Companies
- 36, 851 Observations
- Range: 2/21/2014 - 2/20/2019 

URL: https://www.kaggle.com/datasets/timoboz/stock-data-dow-jones?select=DIS.csv

