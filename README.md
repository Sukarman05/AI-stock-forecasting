# AI-stock-forecasting
Overview
In today’s fast-moving stock market, traders and investors rely on both historical data and real-time market sentiment to make informed decisions. This project bridges that gap by using machine learning and sentiment analysis to predict stock price movements based on historical stock data and social media sentiment from Reddit.
By leveraging the Reddit API, we collect discussions from relevant stock market communities like r/wallstreetbets and r/stocks. Then, using natural language processing (NLP) and deep learning, we integrate sentiment trends into a hybrid predictive model. The results are presented in a user-friendly dashboard built with Streamlit, allowing traders to explore trends and make better investment decisions.

How It Works
=> Data Collection
Stock Prices: We fetch historical stock price data (Open, High, Low, Close, Volume) using Yahoo Finance (yfinance).

Reddit Sentiment: Using the Reddit API (praw), we scrape posts and comments from stock-related subreddits, filtering discussions based on stock symbols and company names.

=> Data Preprocessing
Stock Data: Cleaned, normalized, and structured for time-series forecasting using MinMaxScaler.

Reddit Text Data: Processed using NLP techniques—removing noise, tokenizing, and analyzing sentiment using VADER or a custom-trained model.

=> Feature Engineering
Technical Indicators: Moving Averages, RSI, and other key market signals.

Sentiment Features: Daily sentiment scores and trends aligned with stock prices.

=> Model Development
We use a hybrid model combining:
-> LSTM (Long Short-Term Memory) – A deep learning model designed for time-series forecasting.
-> Sentiment Integration – Sentiment scores are added as features to influence stock price predictions.

The model is trained on historical data and tested on unseen data to measure accuracy.

=> Predictions & Visualization
The trained model forecasts future stock prices based on past price movements and sentiment trends.

Results are displayed in an interactive Streamlit dashboard with:
> Stock price charts
> Sentiment trends
> Predicted vs. actual prices

How It Works – Step by Step
1️> Setup – Authenticate Reddit API and configure Streamlit.
2️> Data Collection – Fetch stock prices & scrape relevant Reddit discussions.
3️> Data Processing – Clean, align, and structure stock & sentiment data.
4️> Model Training – Train a hybrid LSTM model with sentiment features.
5️> Predictions – Generate forecasts using the latest data.
6️> Visualization – Launch the Streamlit app for real-time exploration.

Conclusion
This project blends quantitative finance and social media analysis to create an innovative stock prediction tool. By harnessing Reddit discussions and historical market trends, we offer real-time insights that can help investors stay ahead of the curve. The Streamlit dashboard makes the entire process accessible, allowing traders to explore the complex relationship between market sentiment and stock performance in a simple, visual format.


