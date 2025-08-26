# **NAITradingBot**

**NAITradingBot - Neural Artificial Intelligence Trading Bot** is an automated cryptocurrency trading agent designed to interact with the Binance API and execute trades based on advanced machine learning strategies, including LSTM with attention mechanisms and multiple technical indicators (RSI, MACD, EMA, SMA, breakout/breakdown logic).

The bot has been tested in both Testnet and Mainnet environments and supports real-time execution with live market data through Binance WebSocket streams.

🚀 Features

✅ Binance API Integration – Secure connection with Binance Testnet & Mainnet.

✅ Automated Trading – Executes buy/sell orders based on AI-driven signals.

✅ Multi-Strategy Support – Uses indicators such as RSI, EMA, SMA, MACD, and breakout strategies.

✅ Deep Learning Model – LSTM + Attention mechanism for predictive decision-making.

✅ Scalping / HFT Mode – Capable of executing multiple trades per minute with small profit margins.

✅ Risk Management – Custom stop-loss, dynamic position sizing (in progress).

✅ Logging & Analytics – Trade logs, balance tracking, and performance evaluation.

🛠️ Installation
Requirements

Python 3.9+

Binance API

Required libraries:

```Python
pip install numpy
pip install pandas
pip install tensorflow
pip install keras
pip install nest-asyncio
pip install requests
```

Specific version libraries:

```Python
pip install python-binance==1.0.19
pip install websockets==12.0
```

⚙️ Configuration

Change your keys in this code part 

# For Testnet
```Python
# Binance Testnet API keys
api_key = 'XXXXX'
api_secret = 'XXXXX'

client = Client(api_key, api_secret, testnet=True)
```

Create a new API Key & Secret from Binance API Management.

Enable Spot & Margin Trading.

Do NOT enable withdrawals. 

# For Mainnet
```Python
# Binance Mainnet API keys
api_key = 'XXXXX'
api_secret = 'XXXXX'

client = Client(api_key, api_secret)
```

▶️ Usage

Run the bot with:

python main.py


Example trade log:

```
Buy order executed at Price 4395.81 USDT | 0.0022 ETH | Total: 9.67 USDT | 2025-08-12 16:12:38

Sell order executed at Price 4405.34 USDT | 0.0022 ETH | Total: 9.68 USDT | 2025-08-12 16:28:03
```

📊 Example Results (Mainnet Test – ETH/USDT, 12 Aug 2025)

Number of round-trips: 38

Total Profit: +0.230456 USDT

ROI: 0.0621%

Win rate: 63.2%

Best trade: +0.09735 USDT

Worst trade: -0.040876 USDT

🧠 Roadmap

 Add multi-agent reinforcement learning models (PPO, DQN).

 Implement portfolio management (multi-pair trading).

 Deploy on cloud (AWS / GCP / DigitalOcean).

 Dashboard for visualization of live trades.

⚠️ Disclaimer

This project is for educational and research purposes only.
Trading cryptocurrencies involves significant risk. The authors/contributors are not responsible for any financial losses.
Use at your own risk.


## Authors

- [@nderimajdari](https://github.com/nderimajdari)

