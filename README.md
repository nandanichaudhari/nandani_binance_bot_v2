# Nandani Binance Bot v2 (Educational)

**Purpose:** Educational CLI-based Binance USDT-M Futures order bot skeleton.
**Important:** Use this only for learning. Do not use real funds without testing on testnet.

## Structure
```
nandani_binance_bot_v2/
├── src/
│   ├── __init__.py
│   ├── utils.py
│   ├── market_orders.py
│   ├── limit_orders.py
│   └── advanced/
│       ├── oco.py
│       └── twap.py
├── bot.log
└── README.md
```

## Quick Setup (VS Code)
1. Open VS Code and open this project folder (`nandani_binance_bot_v2`).
2. Create and activate a virtual environment:
   - `python -m venv .venv`
   - Linux/macOS: `source .venv/bin/activate`
   - Windows (PowerShell): `.venv\Scripts\Activate.ps1`
3. Install dependencies:
   - `pip install requests`
4. Set environment variables for API keys (or create a `.env` and load them securely):
   - `export BINANCE_API_KEY="your_api_key"`
   - `export BINANCE_API_SECRET="your_api_secret"`
   - To use testnet, set `BINANCE_BASE_URL` to Binance Futures testnet base URL.
5. Examples:
   - Market order: `python src/market_orders.py BTCUSDT BUY 0.001`
   - Limit order: `python src/limit_orders.py BTCUSDT SELL 0.001 55000`

## Notes
- This code demonstrates API signing, order placement, and simple strategies.
- Always test on testnet. Treat API keys carefully.
