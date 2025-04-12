# Apple-Stock-predictions-using-SimpleRNN-LSTM
This project involves building deep learning models using SimpleRNN and LSTM to predict Apple’s stock prices, focusing on its adjusted closing price. Given the sequential nature of stock market data, the goal is to capture temporal dependencies and forecast stock price movements for 1, 5, and 10-day intervals.

# Skills Demonstrated
* Python Programming
* Data Cleaning & EDA
* Data Visualization (Matplotlib, Seaborn)
* Deep Learning (SimpleRNN, LSTM with TensorFlow/Keras)
* Time-Series Forecasting

# Domain
Finance / Financial Services / Stock Market Analytics

# Models Used
1) SimpleRNN
2) LSTM (Long Short-Term Memory)
# Both models are trained to learn from the previous 60 days to predict:
The next day's price
Prices over the next 5 days
Prices over the next 10 days

# Workflow
1) # Problem Understanding
--> Time-series problem focused on stock trend prediction.

2) # Data Preprocessing
--> Converted Date to datetime format and set as index.
--> Handled missing values using forward fill.
--> Scaled target feature using MinMaxScaler.

3) # Sequence Generation
--> Created 60-day sliding window sequences to train models.

4) # Model Development
--> Defined SimpleRNN and LSTM architectures.
--> Used Dropout layers to prevent overfitting.
--> Compiled models with Adam optimizer and MSE loss.

5) # Training
--> Used EarlyStopping and ModelCheckpoint callbacks.
--> Compared training and validation loss.

6) # Evaluation
--> Inverse-transformed predictions to original scale.
--> Calculated MSE and visualized predicted vs. actual prices.
