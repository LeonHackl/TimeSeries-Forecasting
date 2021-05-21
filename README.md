# Time-Series Forecasting

## Overview
Comparing classic econometric forecasting models like autoregressive-integrated-moving-average (ARIMA) and vector-autoregression (VAR) with modern RandomForest machine learning algorithms regarding the computation of time-series forecasts on the U.S. gross domestic product (GDP). In the first part of this analysis, a general overview of the data is given consisting of different visualizations and hypothesis tests in regards of the order of differencing required to make the data stationary and the autocorrelation of the data. Furthermore, the data is split into two subsets: training and testing data. Whereas the training data is used for model training and hyperparameter optimization and the test set is used for final evaluation and out-of-sample forecasting. For training and evaluation of the ARIMA model, the Box-Jenkins approach will be followed.

#### The Box-Jenkins Method
The Box-Jenkins method refers to the iterative application of the following three steps:
- **Identification:** Using plots of the data, autocorrelations, partial autocorrelations, and other information, a class of simple ARIMA models is selected. This amounts to estimating appropriate values for p, d, and q.

All of the coding related work is done in `Python` using `JupyterLab`. For modelling and computation of the forecasts the `statsmodels` module is used. All computations are done locally on the central-processing-unit (CPU).

## To-Do
- ~Part 1: Data preparation~
- ~Part 2: ARIMA model & forecasting~
- ~Part 3: VAR model & forecasting~
- Part 4: RandomForest algorithm & forecasting
- Part 5: Forecast comparison
