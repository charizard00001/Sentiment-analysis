# Stock Sentiment Analysis Using Machine Learning  

## Overview  
Stock Sentiment Analysis combines **sentiment scores from textual data** with **historical stock price features** to predict stock price movements. By leveraging **Natural Language Processing (NLP)** and **Machine Learning (ML)**, this project identifies **buy/sell signals** for stocks like Microsoft (MSFT), Amazon (AMZN), and Tesla (TSLA), helping traders make informed decisions.  

## Features  
- Sentiment analysis of news and social media using NLP techniques.  
- Integration of stock price features with sentiment data for accurate predictions.  
- Predictive models using ML algorithms like Logistic Regression, Random Forest, SVM, and Neural Networks.  
- Backtesting and portfolio evaluation to assess the trading strategy's effectiveness.  
- Visualization of buy/sell signals on stock price charts.  

## Workflow  

### 1. **Data Collection**  
- Scraped news headlines from [Market Insider](https://markets.businessinsider.com/) for stock-related data.  
- Gathered historical stock prices using the `yfinance` library.  

### 2. **Data Preprocessing**  
- **Text Data**:  
  - Preprocessed text (lowercase conversion, punctuation removal, stemming/lemmatization).  
  - Extracted sentiment scores (positive, negative, neutral) using VADER.  
- **Price Data**:  
  - Calculated moving averages, volatility, and other price-based features.  

### 3. **Feature Engineering**  
- Merged sentiment scores with price data to form a comprehensive dataset.  
- Labeled data for binary classification (price increase: `1`, decrease: `0`).  

### 4. **Model Training and Evaluation**  
- **Trained Models**: Logistic Regression, SVM, Random Forest, Neural Network.  
- **Metrics**: Evaluated using accuracy, precision, recall, F1-score, and ROC-AUC.  
- **Hyperparameter Tuning**: Enhanced model performance through optimization.  

### 5. **Prediction and Strategy Implementation**  
- **Buy/Sell Signals**: Generated signals based on model predictions.  
- **Backtesting**: Validated the trading strategy using unseen data.  
- **Portfolio Evaluation**: Calculated metrics like Sharpe Ratio and Maximum Drawdown.  

### 6. **Visualization**  
- Plotted stock prices with buy/sell points for clear strategy assessment.  

---

## Installation  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/charizard00001/Sentiment-analysis.git  
   cd stock-sentiment-analysis  
