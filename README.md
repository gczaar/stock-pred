CD Projekt Stock Price Prediction
Project Overview
This project develops an LSTM-based machine learning model to predict CD Projekt's next-day stock price based on the previous 10 days of closing prices. Utilizing YFinance for historical data, the model captures trends in the stock’s time series data, aiming to deliver reliable price predictions.

Model Workflow
Data Collection: Fetches CD Projekt stock data using YFinance (closing prices only).
Data Preprocessing: Scales data between 0 and 1 with MinMaxScaler to improve LSTM performance.
Sequence Creation: Forms sequences of 10 days for the model to learn past patterns.
Model Architecture:
LSTM Layers: Two LSTM layers with 50 units each for time-series pattern recognition.
Dense Layer: Outputs the predicted stock price.
Model Training: Trained on 80% of data with an 20-epoch limit and validation on remaining 20%.
Evaluation: Assessed using RMSE, with predictions visualized against actual prices.
Results
The model’s predictions closely follow actual trends, as visualized in a line plot, demonstrating its capability in capturing stock price patterns.

Technologies
Libraries: Python, TensorFlow/Keras, YFinance, NumPy, Pandas, Matplotlib
Methods: LSTM layers, MinMaxScaler for normalization, RMSE for evaluation
How to Run
Install dependencies with pip install yfinance tensorflow scikit-learn matplotlib.
Run the script to train the model and generate predictions for the stock price trend visualization.
