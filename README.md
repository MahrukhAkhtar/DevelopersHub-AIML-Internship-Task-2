# DevelopersHub-AIML-Internship-Task-2

## Stock Price Prediction

### Project Overview
This project is part of the AI/ML Engineering Internship at DevelopersHub Corporation. It focuses on predicting the future closing price of Apple stock (AAPL) using historical market data and Machine Learning models.

### DataSet
**Yahoo Finance Stock Data (AAPL)**
* The dataset consists of historical stock data for Apple Inc. (AAPL) covering a 2-year period.
* It contains **500 rows** and **5 feature columns** (Open, High, Low, Volume, Close) with a target column (Next_Close).

### Tools Used
* Python
* yfinance (Yahoo Finance API)
* Pandas
* Numpy
* scikit-learn
* Matplotlib

### Machine Learning Models
* Linear Regression
* Random Forest Regressor

### Visualizations
* Actual vs Predicted Closing Price Line Plot (Time-Series Comparison)

### Summary of Findings
* Two different machine learning models were trained and compared: **Linear Regression** outperformed the Random Forest Regressor on this dataset.
* **Linear Regression Performance:** * Mean Absolute Error (MAE): **$1.72**
  * $R^2$ Score: **0.9345** (Excellent model fit)
* **Random Forest Performance:**
  * Mean Absolute Error (MAE): **$2.01**
  * $R^2$ Score: **0.9066**
* The actual vs predicted visualization shows the **red dashed line (predicted)** closely following the **blue line (actual prices)**, indicating that the model effectively captured the overall trend and stock volatility.
* Since this is time-series data, disabling data shuffling (`shuffle=False`) during the train-test split was crucial to prevent data leakage and maintain chronological order.
