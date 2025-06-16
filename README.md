# Financial Analysis Assistant

This project was inspired by [Neural Nine’s YouTube tutorial](https://www.youtube.com/watch?v=9y9YYhCuLro&list=PL7yh-TELLS1G9mmnBN3ZSY8hYgJ5kBOg-&index=38&t=2665s).

## Overview

**Financial Analysis Assistant** is an intelligent chatbot designed to deliver real-time stock analysis and financial insights. Built with **Python**, **Streamlit**, **OpenAI’s GPT-3.5 model**, and popular financial libraries, this tool helps users interactively explore market data and technical indicators through a user-friendly web interface.

## Key Features

- **Real-Time Stock Data**: Access the latest stock prices and visualize performance trends over time.
- **Technical Analysis Tools**: Calculate key indicators like SMA, EMA, RSI, and MACD.
- **Visual Charting**: Generate time series plots for stock prices covering the past year.
- **Conversational Interface**: Ask financial questions naturally and get insightful responses via a chatbot interface.
- **Web-Based Access**: Easily use the assistant from any device through a Streamlit-powered frontend.

## How It Works?

The assistant uses GPT-3.5 to interpret user queries and provide intelligent responses. It supports specific function calls to execute various stock-related tasks. Here’s a high-level workflow:

1. **User Input**: Enter your query through the Streamlit app.
2. **Model Interpretation**: GPT-3.5 processes the query, recognizing function-based intents.
3. **Data Processing**: The system fetches relevant financial data using libraries like `yfinance`.
4. **Analysis Execution**: Technical indicators are computed, and visualizations are generated.
5. **Response Output**: Results are displayed in an intuitive format, supporting an ongoing chat-style conversation.

## Getting Started

Follow these steps to run the project locally:

1. Clone this repository to your local system.
2. Install the dependencies using:

```bash
   pip install -r requirements.txt
```
3. Replace 'YOUR_API_KEY' in the code with your actual OpenAI API key.
4. Launch the app using:

```bash
   streamlit run main.py
```

5. Begin exploring stocks and financial data through the chatbot interface.

## Supported Functions
The assistant currently supports the following stock analysis tools:
- `getStockPrice`: Retrieve the latest price for a specified stock ticker.
- `calculateSMA`: Compute the Simple Moving Average over a chosen window.
- `calculateEMA`: Compute the Exponential Moving Average.
- `calculateRSI`: Calculate the Relative Strength Index.
- `calculateMACD`: Get the MACD and signal line values.
- `plotStockPrice`: Display a one-year stock price chart.
