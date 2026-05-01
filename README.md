# Stock-advisor-bot
# 📊 Stock Advisor Bot

An autonomous AI-powered investment analysis agent built in Python. Every morning it analyzes live market data, generates personalized stock picks powered by Claude AI, and delivers a full briefing to your inbox — complete with risk scores, stop-losses, plain English explanations, and more.

> ⚠️ **This project is for educational and experimental purposes only. Nothing it produces is financial advice.**

---

## What It Does

- Fetches live stock prices and market news across all sectors every morning
- Runs the data through three AI analyst personas (Bullish, Bearish, Neutral) and surfaces only the picks all three agree on
- Sends a daily HTML email with picks, a PDF report, and an MP3 audio summary
- Tracks your portfolio value in real time and updates a local browser dashboard
- Learns from its own mistakes — every week it reviews how its suggestions performed and adjusts future analysis accordingly
- Monitors SEC EDGAR for institutional whale activity on every suggested stock
- Sends pre-market alerts, Friday options expiration warnings, volatility alerts, and Sunday performance recaps

---

## What's in Every Daily Email

| Field | Description |
|---|---|
| Risk Score | 1–10 rating (1 = safest, 10 = most aggressive) |
| Confidence | High / Medium / Low |
| Best Time to Buy | Optimal intraday entry window |
| Stop-Loss Price | Recommended exit point to protect capital |
| Sleep Well Score | How safe is this stock to hold overnight |
| News Sentiment | How today's headlines affect this pick |
| Insider Activity | Recent executive buy/sell activity |
| Analyst Target | Wall Street price target vs. current price |

The email also includes a market mood summary, sector heat map, earnings calendar, watchlist, commodity correlation, and a what-if simulator showing hypothetical returns.

---

## Alert Schedule

| Time | What Gets Sent |
|---|---|
| 7:00 AM daily | Pre-market movers |
| 9:30 AM daily | Full daily briefing + PDF + audio |
| 9:00 AM Friday | Options expiration alert |
| 8:00 AM Sunday | Weekly performance recap |
| Anytime | Volatility alert if any stock moves ±5% |

---

## Setup

### 1. Clone the repo
```bash
git clone https://github.com/agonzalez-droid/stock-advisor-bot.git
cd stock-advisor-bot
