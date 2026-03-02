
This project demonstrates how to predict stock prices using a Long Short-Term Memory (LSTM) neural network, a type of recurrent neural network well-suited for sequence prediction problems.

<h2>Project Highlights:</h2>

<h3>Data Acquisition:</h3>
Utilized the yfinance library to fetch historical stock data for a specified ticker symbol (e.g., TATAGOLD.NS).

<h3>Data Preprocessing:</h3>

Scaling: Applied MinMaxScaler from sklearn.preprocessing to normalize stock closing prices, which is essential for stable and efficient neural network training.

Train-Test Split: Divided the dataset into training and testing sets (80% training, 20% testing) to evaluate model performance on unseen data.

Sequence Creation: Implemented a custom function to create input sequences (e.g., 60 previous days' prices) and corresponding target values for the LSTM model.

Reshaping for LSTM: Reshaped the input data to the required 3D format (samples, timesteps, features) for LSTM layers.

<h3>Model Architecture (Keras/TensorFlow):</h3>
Constructed a Sequential LSTM model.

Included multiple LSTM layers (return_sequences=True for intermediate layers, return_sequences=False for the last LSTM layer).

Added Dense layers for output projection.

<h3>Model Training:</h3>

Compiled the model using the adam optimizer and mean_squared_error as the loss function, standard choices for regression tasks.

Trained the model efficiently over several epochs (epochs=10) with a batch size of 1.

<h3>Model Evaluation:</h3>

Root Mean Squared Error (RMSE): 0.5030766305086154

Made predictions on the X_test dataset.

Inverse transformed the scaled predictions and actual test values back to their original price scale for interpretability.

Calculated the Root Mean Squared Error (RMSE) to quantify the difference between predicted and actual prices.
A lower RMSE indicates higher prediction accuracy.

<h3>Visualization:</h3>
Plotted the actual stock prices against the model's predicted prices to visually assess the model's performance and identify trends or discrepancies.






<h2>👨‍💻 Author</h2>

Ashutosh Tare | Aspiring ML Engineer | Data Science Enthusiast
