# ML_StockPrice_Prediction

Stock Price Prediction for TATA STEEL

This project provides an end-to-end workflow for predicting TATA STEEL's stock price using ARIMA and Ridge Regression models. The code covers data preparation, time series decomposition, stationarity testing, modeling, evaluation, and future forecasting. It uses both traditional time series analysis (ARIMA) and machine learning regression (Ridge, Linear Regression).

Features
- Download historical stock data for TATA STEEL using Yahoo Finance.
- Data preprocessing: cleaning, date conversion, feature extraction.
- Visualization:
  - Line, candlestick charts
  - Interactive Plotly graphs
  - Year-wise and decomposition analysis
- Stationarity tests: Augmented Dickey-Fuller (ADF), differencing.
- Modeling:
  - ARIMA model for time series
  - Ridge Regression and Linear Regression for feature-based modeling
  - Model evaluation: MAE, RMSE, R^2, residual distribution analysis.
- Forecasting: Predicts stock prices for the next 6 and 12 months.
- Comprehensive plotting and results visualization.

Requirements
- Python 3.7+
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- statsmodels
- scikit-learn
- yfinance

Install using pip:

bash
pip install pandas numpy matplotlib seaborn plotly statsmodels scikit-learn yfinance

Usage
1.	Fetch data:
- The script downloads TATA STEEL historical stock price data from Yahoo Finance.
- Optionally imports CSV from local/Google Drive sources.
2.	Run the script:
- Execute the Python script directly:

bash
python stock_price_prediction_tata_steel_2.py
- It is designed to run in Jupyter/Colab and as a standalone script.
3.	View Results:
- Visualizations and result plots will display directly via matplotlib and Plotly.
- Model predictions and future forecast plots are shown for both ARIMA and Ridge Regression.

Input Data
- TATA STEEL stock data (automatically downloaded via yfinance).
- Optional: Use your own CSV by editing the file path in the script.

Output
- Plots: Time series, decomposition, prediction overlays, residual analysis.
- Metrics: MAE, RMSE, R² for both training and testing periods.
- Forecasts: Stock price predictions for the next 6 and 12 months.

How it Works
- Stationarity: The series is checked and made stationary for ARIMA by differencing.
- Model Selection: Uses ACF/PACF plots for ARIMA (p,d,q) selection.
- Regression: Uses Ridge and Linear Regression as alternative approaches.
- Forecast: Generates future business-day dates and predicts future values using the best model.
- isualization: All steps visualized for easy interpretation.

Limitations
- Future performance of stocks is not predictable and this script is for educational purposes only.
- Model tuning not exhaustive: parameters can be optimized further.
- Requires a stable internet connection for data download.

Acknowledgement
- Yahoo Finance for stock data (yfinance)
- Open source community for modeling and visualization libraries

Contact
For questions or improvements, please open an issue or contact the author.

