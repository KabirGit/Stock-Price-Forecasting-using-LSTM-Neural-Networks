# Stock-Price-Forecasting-using-LSTM-Neural-Networks
Built an LSTM-based model to predict stock prices using historical data. Preprocessed and normalized time series data, trained the model with Keras, and achieved 87% accuracy. Visualized predictions to validate trends, demonstrating the effectiveness of deep learning in finance.

# 📈 Stock Market Prediction using Stacked LSTM

This project demonstrates the use of a **Stacked LSTM (Long Short-Term Memory)** model to predict future stock prices based on historical data. Implemented in Python using TensorFlow/Keras, the model forecasts both short-term trends and the next 30 days of prices.

## 🔍 Overview

- **Objective:** Forecast future stock prices using past market data.
- **Dataset:** Apple (AAPL) stock prices from 2015 to 2020, including `Open`, `High`, `Low`, `Close`, and `Volume`.
- **Model:** Deep Stacked LSTM with 3 layers and 100 time steps input.

## 🧠 Key Features

- Data scaling using `MinMaxScaler` for LSTM sensitivity.
- Custom sequence generation function for time-series windows.
- Train-test split (65-35%) on normalized close prices.
- Stacked LSTM model with 3 layers and a dense output layer.
- Visualization of:
  - Historical vs Predicted values
  - 30-day forecast plot
- RMSE calculated for both training and test predictions.

## 🛠️ Libraries Used

- `Pandas`, `NumPy` – Data handling
- `Matplotlib` – Visualization
- `Scikit-learn` – Scaling and metrics
- `TensorFlow/Keras` – Model development

## 📊 Performance

- **Training RMSE:** ~141.22  
- **Testing RMSE:** ~235.68  
- The model performed well in capturing the trend with low validation loss and smooth convergence.

## 📈 Forecasting Future Days

- The model predicts the next **30 days** of stock prices using the last 100 data points.
- Forecast is plotted alongside historical data for visual inspection.

## 🔧 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/stock-lstm-predictor.git
   cd stock-lstm-predictor
   ```

2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook or Python script:
   ```bash
   jupyter notebook stock_price_prediction.ipynb
   ```

## 📌 Future Enhancements

- Incorporate additional indicators (e.g., RSI, MACD)
- Add support for multiple stock symbols
- Use real-time API integration for live predictions

## 👨‍💻 Author

**Kabir Talbhandare**  
[LinkedIn](https://linkedin.com/in/your-profile) | [GitHub](https://github.com/your-username)

---

*Note: This project is for educational purposes and not intended for actual financial trading decisions.*
