# CryptAI: Sentiment-Driven Crypto Trading Engine

## Overview

CryptAI is a sentiment-driven cryptocurrency trading engine that combines real-time market data, social sentiment analysis, and technical indicators to automate trading decisions.

The platform continuously monitors cryptocurrency markets through exchange WebSockets while simultaneously analyzing sentiment from news and Reddit sources. Based on these signals, CryptAI dynamically selects trading strategies and executes paper trades through Alpaca.

Built as a distributed microservice architecture, the system focuses on low-latency data processing, real-time monitoring, and scalable strategy execution.

---

## Demo Video
https://github.com/mehtar38/CryptoStar/blob/main/CryptAI.mp4

## Features

### Real-Time Market Data Processing

* Live cryptocurrency market data ingestion using WebSocket connections
* Concurrent exchange integrations with Binance and KuCoin
* Real-time price, volume, and market movement tracking

### Sentiment-Based Trading

* Reddit sentiment analysis
* News sentiment analysis
* Dynamic strategy selection based on market sentiment signals
* Automated signal generation pipeline

### Technical Analysis Engine

* Relative Strength Index (RSI)
* Exponential Moving Average (EMA)
* Simple Moving Average (SMA)
* Multi-factor trading decision framework

### Automated Trade Execution

* Paper trading through Alpaca
* Real-time order placement and management
* Portfolio tracking and performance monitoring

### Real-Time Dashboard

* Live portfolio monitoring
* Market data visualization
* Trading activity tracking
* Strategy performance insights

### High-Performance Architecture

* FastAPI-based microservices
* Redis caching for low-latency operations
* PostgreSQL persistence layer
* Event-driven market processing

---

## Tech Stack

### Backend

* Python
* FastAPI
* WebSockets
* Alpaca Trading API

### Data & Storage

* PostgreSQL
* Redis

### Frontend

* React
* JavaScript
* CSS

### Market & Sentiment Sources

* Binance API
* KuCoin API
* Reddit Data Sources
* News Data Sources

---

## Trading Workflow

1. Market data is streamed from Binance and KuCoin.
2. News and Reddit content are collected for sentiment analysis.
3. Sentiment scores are generated in real time.
4. Technical indicators (RSI, EMA, SMA) are calculated.
5. Strategy selection is performed using sentiment and technical signals.
6. Trade decisions are executed through Alpaca paper trading.
7. Results are stored in PostgreSQL and cached using Redis(still in development).
8. Portfolio and trade activity are displayed on the React dashboard.

---

## Installation

### Prerequisites

* Python 3.10+
* PostgreSQL
* Redis
* Node.js
* Alpaca API Credentials

### Backend Setup

```bash
git clone https://github.com/mehtar38/CryptoStar

cd backend
univorn main:app --reload

```

### Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

### Start Services

```bash
docker-compose up -d
```

---

## Future Improvements

* Additional exchange integrations
* Enhanced sentiment models using LLMs
* Strategy backtesting framework
* Portfolio optimization algorithms
* Risk-adjusted position sizing
* Production trading support

---

## Contributors

Developed as part of a sponsored project by **San Van High Technologies** by:
- Mitali Deshmukh
- Prina Gudhka
- Revathi Priyan
- Rutvi Mehta

**Duration:** January 2025 – May 2025

---

## Disclaimer

This project is intended for educational and research purposes. Current implementation focuses on paper trading and strategy evaluation. Cryptocurrency trading involves significant financial risk.
