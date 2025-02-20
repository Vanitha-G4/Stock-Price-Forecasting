### Stock Price Forecasting using ARIMA
This project demonstrates how to use historical stock price data and apply the ARIMA (Auto-Regressive Integrated Moving Average) model to predict future stock prices. 
The stock data is obtained using yfinance, and we visualize the results using matplotlib. We evaluate the model using Root Mean Squared Error (RMSE).

### Requirements
To run this project, you'll need to install the following Python libraries:

    --yfinance for downloading stock data
    --pandas for data manipulation
    --matplotlib for visualization
    --statsmodels for the ARIMA model
    --sklearn for evaluating the model
    
### You can install the required packages using pip:
  pip install yfinance pandas matplotlib statsmodels scikit-learn
### Steps in the Code
   * Download Stock Price Data: We use the yfinance library to download stock price data for a specific stock symbol. In this example, we use Apple (AAPL), but you can change it to any valid stock symbol.

  * Visualize Stock Price Data: The closing prices of the stock are plotted over time for visual analysis.

  * Autocorrelation and Partial Autocorrelation: We use ACF (AutoCorrelation Function) and PACF (Partial AutoCorrelation Function) plots to help determine the best parameters for the ARIMA model (p, d, q).

 * Prepare the Data: We clean the data by dropping any NaN values and then split it into training and testing datasets. 80% of the data is used for training and the remaining 20% for testing.

 * Fit ARIMA Model: We fit an ARIMA model with specified parameters (p=5, d=1, q=0) to the training data.

 * Make Predictions: The trained ARIMA model is used to forecast future stock prices, and we visualize the predicted data alongside the actual test data.

 * Evaluate the Model: We use RMSE (Root Mean Squared Error) to evaluate how well our model performed in predicting stock prices.

 * Visualization of Actual vs Predicted Data: The actual test data and predicted forecast are plotted for comparison.
