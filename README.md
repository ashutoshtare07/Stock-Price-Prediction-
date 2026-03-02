# Stock-Price-Prediction

In this project, I performed a time series analysis to predict stock prices using an LSTM (Long Short-Term Memory) neural network. The process involved:

Data Acquisition: 
Downloading historical stock data (e.g., TATAGOLD.NS) using the yfinance library.

Data Preprocessing:
Scaling the stock prices using MinMaxScaler to normalize the data, which is crucial for neural networks. I also handled data splitting into training and testing sets, and reshaped the data to create sequences suitable for LSTM input.

Model Building: Constructing a sequential LSTM model using Keras, including multiple LSTM layers and dense layers to learn complex patterns in the time series data.

Model Training: Compiling the model with an Adam optimizer and mean squared error loss, and then training it on the historical data.

Model Evaluation: Making predictions on unseen test data, inverse transforming the predictions to their original scale, and evaluating the model's performance using metrics like Root Mean Squared Error (RMSE). 

Finally, visualizing the actual vs. predicted prices to understand the model's accuracy.
This project provided hands-on experience with fundamental concepts in time series forecasting, deep learning for sequential data, and practical application of machine learning in financial markets.
