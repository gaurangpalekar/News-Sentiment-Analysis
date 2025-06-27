# News-Sentiment-Analysis
NIFTY 50 Price Prediction using News Sentiment
A full-stack application that predicts the next day's NIFTY 50 closing price based on news headlines using sentiment analysis and LSTM modeling.

Overview
Financial markets are heavily influenced by investor sentiment. This project attempts to quantify sentiment from financial news headlines and use it to forecast NIFTY 50 index prices for the next day using a deep learning approach.

Tech Stack
Frontend: HTML/CSS

Backend: Flask

Machine Learning: LSTM with TensorFlow/Keras

Sentiment Analysis: VADER (Valence Aware Dictionary and sEntiment Reasoner)

Model Workflow
java
Copy
Edit
News Headline → Sentiment Score (VADER) → LSTM Model → Price Prediction
Input: Last 10 days of NIFTY 50 closing prices and sentiment scores

Model: 2 LSTM layers + Dense layer

Output: Predicted next-day closing price

Dataset and Features
Data Sources: NIFTY 50 closing prices and financial news headlines

Features Used:

VADER sentiment score

Closing price (time-series)

Missing Values: Handled using forward fill

Windowing: 10-day lookback used for each prediction

Application Flow
User inputs a news headline on the frontend.

Backend uses VADER to assign a sentiment score.

LSTM model predicts the next day's NIFTY 50 price.

Prediction is displayed to the user.

Challenges Faced
Accurate alignment of news and price data

Managing small dataset size

Preventing overfitting in time-series data

Full-stack deployment integration

Future Improvements
Add technical indicators (e.g., RSI, volume)

Replace VADER with transformer-based models like BERT for improved sentiment accuracy

Containerize with Docker and deploy on cloud platforms

Project Outcome
Successfully built and deployed an end-to-end ML pipeline for stock price prediction based on news sentiment. Great learning experience in both NLP modeling and full-stack development.
