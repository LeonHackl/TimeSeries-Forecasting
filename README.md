# Time-Series Forecasting

## Overview
Comparison of classic econometric forecasting models like autoregressive-integrated-moving-average models (ARIMA) and vector-autoregressions (VAR) regarding the computation of time-series forecasts of the U.S. gross domestic product (GDP). In the first part of this analysis, a general overview of the data is given, consisting of different visualizations and hypothesis tests in regards of the order of differencing required to make the data stationary and the autocorrelation of the data. Furthermore, the data is split into two subsets: training and testing data. Whereas the training data is used for model training and hyperparameter optimization and the test set is used for final evaluation and out-of-sample forecasting. For training and evaluation of the models, the Box-Jenkins approach will be followed.

#### The Box-Jenkins Method
The Box-Jenkins method refers to the iterative application of the following three steps:
- **Identification:** Using plots of the data, autocorrelations, partial autocorrelations, and other information, a class of simple ARIMA models is selected. This amounts to estimating appropriate values for p, d, and q.
- **Estimation:** The parameters of the selected model are estimated using maximum likelihood
techniques as outlined in Box-Jenkins (1976).
- **Diagnostic Checking:** The fitted model is checked for inadequacies by considering the autocorrelations of the residual series (the series of residual, or error, values).

All of the coding related work is done in `Python` using `JupyterLab`. For modelling and computation of the forecasts the `statsmodels` module is used. All computations are done locally on the central-processing-unit (CPU).
