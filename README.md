# Stock Price Prediction of Apple Inc. Using Recurrent Neural Network
Closing Price Prediction of Apple Inc. Using LSTM Recurrent Neural Network

# Dataset:
The dataset is taken from yahoo finace's website in CSV format. The dataset consists of Open, High, Low and Closing Prices of Apple Inc. stocks from 1st january 2000 to 30th May 2021 - 5387 rows × 6 columns. 
# Price Indicator:
Stock traders mainly use three indicators for prediction: OHLC average (average of Open, High, Low and Closing Prices), HLC average (average of High, Low and Closing Prices) and Closing price, In this project, Closing price has been used.
# Data Pre-processing:
After filtering the Closing price in the dataset, it becomes one column data. This has been converted into two column time series data, 1st column consisting stock price of time t, and second column of time t+1. All values have been normalized between 0 and 1.
# Model: 
Two sequential LSTM layers have been stacked together and one dense layer is used to build the RNN model using Keras deep learning library. Since this is a regression task, 'linear' activation has been used in final layer.
# Version:
Python 3.8 and latest versions of all libraries including deep learning library Keras and Tensorflow.
# Training:
70% data is used for training. Adam optimizer is used for faster convergence.
After training starts it will look like:

![ttt1](https://github.com/imrishi24/Apple-Stock-Price-Prediction-/blob/main/1.png)

# Test:
Test accuracy metric is root mean square error (RMSE).
# Results:
The Movement of Closing price:

![ttt1](https://github.com/imrishi24/Apple-Stock-Price-Prediction-/blob/main/2.png)

After the training the fitted curve with original stock price, predicetd stock price and validated stock price:

![tt2](https://github.com/imrishi24/Apple-Stock-Price-Prediction-/blob/main/3.png)

# Observation and Conclusion:
Since difference among OHLC average, HLC average and closing value is not significat, so only Closing price is used to build the model and prediction. The training and testing RMSE are: 1.08 and 1.67 respectively which is pretty good to predict future values of stock.

Finally, this work can greatly help the quantitative traders to take decisions.

# For Reference:
https://cppsecrets.com/users/810311410511510497981041141031171141069711464103109971051084699111109/Stock-Price-Prediction-of-Apple-Inc-Using-Recurrent-Neural-Network.php
