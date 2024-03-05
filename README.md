# Stock Price Prediction with Random Forest Classifier

## Overview

This mini project aims to predict whether the stock market will go up or down based on historical S&P 500 data using a Random Forest Classifier. The project involves data fetching, preprocessing, model training, prediction, and backtesting.

## Files

- **stock_price_prediction.ipynb**: Jupyter Notebook containing the complete code for the project.
- **README.md**: Summary file explaining the project overview and structure.

## Steps

1. **Data Retrieval:**
   - Historical S&P 500 data is fetched using the yfinance library.

2. **Data Preprocessing:**
   - The datetime index is reformatted to display only the date.
   - Unnecessary columns (Dividends, Stock Splits) are removed.
   - A target variable ("Target") is created, indicating whether the stock will go up or down based on the closing prices.

3. **Model Training:**
   - A RandomForestClassifier is initialized and trained on the training set.
   - The features used for prediction include "Close," "Volume," "Open," "High," and "Low."

4. **Backtesting:**
   - The model is backtested over multiple years, stepping through the data one year at a time.
   - Predictions are made for each backtesting period using the trained model.
   - Precision scores are calculated for each backtesting period.

5. **Results Visualization:**
   - Predicted values and precision scores are visualized, and the count of predicted values for each class is displayed.

## Usage

1. Open and run the Jupyter Notebook file: **stock_price_prediction.ipynb**.
2. Follow the step-by-step instructions in the notebook to understand the data processing, model training, and backtesting process.

## Dependencies

- yfinance
- pandas
- scikit-learn

## Improvements

- Further hyperparameter tuning and feature engineering can be explored to enhance model accuracy.
- Experiment with different machine learning algorithms for comparison.
