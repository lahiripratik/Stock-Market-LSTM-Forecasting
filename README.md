# Stock Market LSTM Forecasting
LSTM stands for Long Short Term Memory Networks. Many theories suggest stock prices tend to depend on their previous values, despite many assumptions of a random walk model.
In this project, I attempted to study the impact of trend of a stock on its future prices. 

I took a lag of 4 prices, which means that I judged the dependance of a stock's price today on four previous closing values. I tried to build a relationship for the same and aimed to predict the coeffecients accurately.

### Preprocessing
Used MinMax scaler to compress the stock price data between 0 and 1 as LSTM is very sensitive to the scale of the data.
Then, divided the data into training and testing batches, in a ratio of 2:1. Cross Validation and Random Seed work better in Regression so not done here.
#### Timesteps : talks about how many previous days does present day price depend on
Previous days are X-Train and Today is Y-Train.

### Training the LSTM Model
Imported Sequential, Dense and LSTM libraries. Ran 100 epochs.
Scaler inverse transform was done on previously transformed data to study RMSE easily.

### Testing the model over the test dataset

### Predicting output for the next 30 days
