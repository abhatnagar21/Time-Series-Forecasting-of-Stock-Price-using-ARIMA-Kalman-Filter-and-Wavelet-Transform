Stock Price Prediction using Time Series Models
📌 Project Overview
This project implements time series forecasting for stock prices using multiple models, including:
✅ Simple Moving Averages (SMA)
✅ Exponential Smoothing
✅ ARIMA (Auto-Tuned)
✅ Kalman Filter
✅ Wavelet Transform

The goal is to improve prediction accuracy by applying different models and optimizing them.

📂 Dataset
The stock data is read from a CSV file instead of being downloaded from Yahoo Finance.

🔹 Expected CSV Format:
Date	Close	High	Low	Open	Volume
2022-01-03	178.8	179.7	174.6	174.7	104487900
2022-01-04	176.6	179.7	176.0	179.4	99310400
📌 Ensure the dataset contains at least these columns:

Date (Set as index)
Close (Main feature for predictions)
Open, High, Low, Volume (Additional features)
📊 Models Used
1️⃣ Simple Moving Averages (SMA)
SMA_20: 20-day moving average
SMA_50: 50-day moving average
2️⃣ Exponential Smoothing
Captures trends and seasonality.
Implemented using statsmodels.tsa.holtwinters.ExponentialSmoothing
3️⃣ ARIMA (Auto-Tuned)
Automatically finds the best (p, d, q) values.
Uses pmdarima.auto_arima
4️⃣ Kalman Filter
Smooths noisy stock price data to improve predictions.
5️⃣ Wavelet Transform
Removes noise from stock data before applying models.
🚀 How to Run
1️⃣ Install Dependencies
bash
Copy
Edit
pip install pandas numpy matplotlib statsmodels pmdarima sklearn yfinance pywt pykalman
2️⃣ Run the Python Script
bash
Copy
Edit
python stock_prediction.py
📌 Key Features
✅ Reads stock data from a CSV file
✅ Preprocesses data (removes NaNs, normalizes, smooths)
✅ Applies multiple forecasting models
✅ Plots actual vs predicted stock prices

📈 Sample Prediction Plot

💡 Future Improvements
Tune hyperparameters for better accuracy
Add deep learning models (LSTMs, Transformer models)
Incorporate news sentiment analysis
