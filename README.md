# Stock_Trend_Prediction_Model

A Machine Learning model that predicts the trend of a stock, developed by me and my two respected mates in college as a semester project.

-The model uses LSTM (Long Short Term Memory) -  a type of Recurrent Neural Network (RNN).

-It begins by taking the stock ticker and start and end date for the time period as input.

-Here, Yahoo Finance API is used to fetch historical data of the stock.

-The dataframe contains many features like Open, High, Low etc. The feature used here to build the model is Adj Close as it is mostly recommended.

-The data set is divided into two sets as usual- training and testing in the ratio 80:20.

-A time frame of 100 days is used to predict the 101st day price. For example, a time frame 1st - 100th day is used to predict the 101st day price, a time frame 2nd - 101st day is used to predict the 102nd day price and so on.

-The LSTM Neural Network model contains 5 layers.

-Model is fitted with early stopping and stochastic gradient descent as well to improve the optimization.

-Next the price for the unseen 30 days in the future is predicted.