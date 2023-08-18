# Stock Market LSTM Forecasting
LSTM stands for Long Short Term Memory Networks. Many theories suggest stock prices tend to depend on their previous values, despite many assumptions of a random walk model.
In this project, I attempted to study the impact of trend of a stock on its future prices. 

I took a lag of 4 prices, which means that I judged the dependance of a stock's price today on four previous closing values. I tried to build a relationship for the same and aimed to predict the coeffecients accurately.

### Preprocessing
Used MinMax scaler to compress the stock price data between 0 and 1.
Then, divided the data into training and testing batches, in a ratio of 2:1.
