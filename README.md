# IPO ATH Tracker

Live candlestick charts for every NSE IPO (mainboard and SME) listed in the last three months, built to spot new listings that hit a high, pulled back, and are climbing back toward it.

**Live site:** https://kevcode-absurd.github.io/ipo-ath-tracker/

## How it works

- `snapshot.json` is rebuilt every weekday after the 3:30 PM IST close: the IPO list (NSE), three months of hourly and daily candles (Upstox), and company details (Yahoo Finance and offer documents).
- In the browser, the page pulls today's 5-minute candles from Upstox's public market data every minute between 9 AM and 4 PM IST, and whenever someone presses Refresh, so prices, distance from the all-time high and today's candles stay current.
- Charts use [TradingView Lightweight Charts](https://www.tradingview.com/lightweight-charts/).

## Filters

- **Back near high**: dipped at least the chosen amount (5–20%) from an earlier high and now within the chosen band (1–10%) of the all-time high.
- **At all-time high**, **Pulled back from high**, **All listings**, plus search, listing window, segment, candle size and sort.

Market data is for information only and may be delayed or incomplete. Not investment advice.
