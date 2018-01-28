# Tackling the Risk

Assumptions

1. Final data taken for training is univariate.
2. There are no outliers or missing values in the data.
3. The data is continuous time-series.

Exact Model Used, Parameters and Techniques

There is a definite relation between the losses and total number of cases in individual divisions and quarters. A new feature is created by dividing the total loss by total number of cases, whic gives mean loss. Now, Total number of cases for the subsequent year is calculated by estimating using the Total number of cases in the training data. Now, using the training data, final mean loss is calculated, which is multiplied with the estimated number of cases for each individual division, giving total loss.

The data is forst made stationary through 3 consecutive log transofrmation. ARIMA model is used, with autoregressive lag of 4 and a moving average of 0. the data is differenciated 1 time.

The above p,d,q parameters are calculated using a combination of GridSearch and AC and PAC plots.

Theoretical Results used and Citations

Box, G; Jenkins, G. (1970). Time Series Analysis: Forecasting and Control. San Francisco: Holden-Day.
Hamilton, J.D. (1994). Time Series Analysis. Taylor & Francis US.


