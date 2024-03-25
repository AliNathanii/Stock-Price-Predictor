# Stock-Price-Predictor
Utilizes ML (Random Forest) to predict stock price movements based on historical data of the S&amp;P 500 index.

Data Retrieval:

Imported historical stock price data for the S&P 500 index (^GSPC) from Yahoo Finance using the yfinance library.
Limited the data retrieval period from January 1, 2000, to January 1, 2023.

Data Preparation and Exploration:

Plotted the overall trends of the S&P 500 index and its closing prices against time.
Removed irrelevant columns such as "Dividends" and "Stock Splits" from the dataset.
Created a target variable ("Target") representing whether the stock price would increase or decrease the next day.

Model Training and Evaluation:

Split the dataset into training and testing sets.
Trained a RandomForestClassifier model using features such as close price, volume, open, high, and low prices.
Evaluated the model's precision score, indicating the accuracy of predicting stock price movements.

Backtesting and Model Improvement:

Implemented functions for backtesting and improving the model's performance over time.
Incorporated rolling averages and trends as new predictors to enhance the model's predictive power.
Fine-tuned the RandomForestClassifier model parameters for better performance.

Results and Analysis:

Analyzed the model's predictions through backtesting and evaluated its precision score.
Examined the distribution of predicted outcomes and compared them with actual stock price movements.
