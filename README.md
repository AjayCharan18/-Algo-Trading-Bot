
# Algo Trading Bot

This is a fully-featured algorithmic trading system for Indian stocks using yfinance, technical indicators, ML-based predictions, Google Sheets logging, and Telegram notifications. It is designed to be run in Google Colab.

## Features

- **Fetches historical data** from Yahoo Finance for a configurable list of stocks.
- **Calculates technical indicators** (RSI, MACD, SMA, Bollinger Bands, ATR, VWAP, Stochastic).
- **Backtests a trading strategy** (relaxed RSI-based demo for testing).
- **Logs all trades and summary stats** to Google Sheets.
- **Sends trade/summary notifications** to Telegram.
- **Trains a RandomForest ML model** to predict next-day price movement and logs results.
- **Interactive Plotly charts** for each stock.
- **Robust error handling** and logging.

## Setup

1. **Clone this repo or download as ZIP.**
2. **Install requirements** (Colab cell does this, or use pip locally):
3. **Google Sheets API:**
   - Create a Google Service Account and download the JSON credentials.
   - Upload your JSON credentials to Colab or your project directory.
   - Share your Google Sheet with the service account email.

4. **Edit `config` in `algo_trading_bot.py`:**
   - Set `GDRIVE_JSON` to the path of your service account JSON.
   - Set your Telegram Bot token and Chat ID.

5. **Run in Colab or locally:**
   - For Colab: Copy/paste the code, upload your JSON, and run.
   - For local: Ensure all dependencies are installed.

## Usage

- Adjust the list of stocks and strategy as desired.
- All trades, summary, and ML analytics will be logged to your configured Google Sheet.
- Telegram notifications will be sent automatically.

## Files

- `algo_trading_bot.py` — Main script (copy-paste into Colab or run locally)
- `README.md` — This file
- *(Optional)* `requirements.txt` — List of Python dependencies

## License

MIT
