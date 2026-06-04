# 📈 Day Trading Academy

> A complete, interactive day trading education platform — from absolute zero to deploying a live Pine Script strategy on TradingView. Built as a single HTML file with no dependencies beyond a CDN.

![Day Trading Academy](https://img.shields.io/badge/Course-16%20Modules-blue) ![Quizzes](https://img.shields.io/badge/Quizzes-80%20Questions-purple) ![License](https://img.shields.io/badge/License-MIT-green) ![HTML](https://img.shields.io/badge/Built%20with-HTML%2FCSS%2FJS-orange)

---

## 🖥️ Live Demo

Open `index.html` in any modern browser — no server, no install, no account needed.

---

## 📚 What's Inside

A fully interactive dashboard covering **16 modules** with **90+ slides**, **live canvas charts**, **80 quiz questions**, and a **complete Pine Script trading strategy** ready to deploy on TradingView.

### Course Modules

| # | Module | Topics |
|---|--------|--------|
| 1 | **Market Fundamentals** | Stock market mechanics, order types, market hours, PDT rule |
| 2 | **Candlestick Charts** | OHLC anatomy, bullish/bearish candles, timeframes, multi-TF analysis |
| 3 | **Candlestick Patterns** | Doji, Hammer, Engulfing, Morning/Evening Star, 3 Soldiers — drawn on Canvas |
| 4 | **Support & Resistance** | Level identification, role reversal, zones, dynamic S/R (EMAs) |
| 5 | **Technical Indicators** | EMA/SMA, RSI, MACD, Bollinger Bands, VWAP, Volume — all with live charts |
| 6 | **Chart Patterns** | Head & Shoulders, Double Top/Bottom, Triangles, Flags, Cup & Handle |
| 7 | **Confluences & Trade Setups** | Multi-TF analysis, 5 setup types, complete AAPL trade example with P&L |
| 8 | **Risk Management** | Position sizing formula, 1% rule, equity curve comparison, drawdown math |
| 9 | **Options Basics** | Calls/Puts, ITM/ATM/OTM, payoff diagrams, live options chain |
| 10 | **Options Greeks** | Delta, Gamma, Theta, Vega, Rho — interactive curves + IV Crush explained |
| 11 | **Options Strategies** | Covered Call, Bull/Bear Spreads, Iron Condor, Straddle, Strangle |
| 12 | **Volatility** | HV vs IV, VIX chart with zones, IV Rank, volatility skew |
| 13 | **Market Microstructure** | Bid/Ask spread, Market Makers, Level 2 mock order book, tape reading |
| 14 | **Trading Psychology** | Emotion cycle chart, FOMO, revenge trading, trading journal template |
| 15 | **TradingView Guide** | Interface walkthrough, drawing tools, indicators, alerts, Pine Script basics |
| 16 | **Live Trading Playbook** | Complete Pine Script v2, position sizing calculator, pre-market routine, 90-day live plan |

---

## ✨ Features

- **🕯️ Live Canvas Charts** — Candlestick charts with EMAs, S/R levels, pattern labels, and trade setup zones (entry/SL/TP) all rendered from scratch using Canvas API
- **📊 Chart.js Visualizations** — RSI, MACD, Bollinger Bands, equity curves, emotion cycle, VIX with colored zones
- **📝 80-Question Quiz System** — Per-module quizzes with instant feedback, explanations, and score tracking
- **🧒 ELI10 Mode** — Every concept explained in simple language for beginners (toggle top-right)
- **💾 Progress Saved** — LocalStorage saves your progress across sessions automatically
- **🧮 Interactive Position Sizing Calculator** — Input account/risk/entry/stop → get exact share count, dollar risk, and price targets
- **📋 Copy-Ready Pine Script** — Complete 150-line production strategy with one-click copy button
- **📱 Single HTML File** — Zero setup, works offline, no build step

---

## 🚀 Pine Script Strategy (DTA Pro v2.0)

The capstone module includes a complete, production-ready **Pine Script v5** strategy for TradingView:

**Strategy logic:**
- EMA(9) crosses EMA(21) — trend shift signal
- RSI(14) filter — not overbought/oversold
- Volume filter — must exceed 1.5× 20-period average
- EMA(50) trend bias — long only above it, short only below
- Session filter — trades only 9:30–4:00 PM ET

**Risk management built-in:**
- ATR-based stop loss (1.5× ATR) — adapts to volatility automatically
- 2:1 R:R take profit hardcoded
- Live info table on chart — position, P&L, win rate, RSI, ATR
- Auto-drawn entry/stop/target lines for every open trade

**To use:** Copy the script → open TradingView → Pine Editor → Paste → Add to chart.

---

## 🛠️ Tech Stack

| Technology | Used For |
|-----------|----------|
| Vanilla HTML/CSS/JS | Entire app — no framework |
| Canvas API | Candlestick charts, payoff diagrams, Greek curves, VIX chart |
| [Chart.js 4.4](https://www.chartjs.org/) | Equity curves, emotion cycle (via CDN) |
| LocalStorage | Progress persistence |
| CSS Variables | Dark trading theme |

**No build step. No npm. No framework. Just open `index.html`.**

---

## 📂 Project Structure

```
trading-dashboard/
└── index.html          # The entire app — all HTML, CSS, JS in one file
```

---

## 🖥️ How to Run Locally

```bash
# Option 1: Just double-click index.html in Finder

# Option 2: Serve with Python (avoids any file:// quirks)
cd trading-dashboard
python3 -m http.server 8080
# Then open http://localhost:8080

# Option 3: Serve with Node.js
npx serve .
```

---

## 🌐 Deploy to GitHub Pages (Free Hosting)

1. Fork or clone this repo
2. Go to your repo on GitHub → **Settings** → **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Select **main** branch, **/ (root)** folder → **Save**
5. Your site will be live at `https://YOUR-USERNAME.github.io/REPO-NAME/`

---

## 📖 Learning Path

The course is designed to be completed in order, but each module is self-contained:

```
Beginner Path (Weeks 1–2):
  Modules 1 → 2 → 3 → 4 → 8 (Risk Management first!)

Intermediate Path (Weeks 3–4):
  Modules 5 → 6 → 7 → 13 → 14

Options Track (Weeks 5–6):
  Modules 9 → 10 → 11 → 12

Live Trading Prep (Week 7+):
  Modules 15 → 16
```

**Recommended:** Complete all quizzes before moving to live trading. A pass rate of 80%+ across all modules indicates readiness.

---

## 🎯 Capstone Strategy — Quick Start

After completing the course:

1. **Open TradingView** (free account at tradingview.com)
2. Click **Pine Editor** at the bottom of the screen
3. Click **New blank indicator**
4. Go to **Module 16 → Slide 3** in this dashboard
5. Click **📋 Copy v2** button to copy the strategy
6. Paste into Pine Editor → click **Add to chart**
7. Open the **Strategy Tester** tab to see backtest results
8. Set **Trade Direction** to "Long Only" for your first month

**Recommended starting settings:**
- Chart: 15-minute or 1-hour
- Instrument: SPY, QQQ, AAPL, MSFT (liquid, trending)
- Paper trade for 4+ weeks before using real money

---

## ⚠️ Disclaimer

This project is for **educational purposes only**. Nothing in this course constitutes financial advice. Trading involves substantial risk of loss. Past performance (including backtested strategy results) does not guarantee future results. Only trade with money you can afford to lose. Always consult a licensed financial advisor before making investment decisions.

---

## 🤝 Contributing

Contributions are welcome! Here are some ideas:

- Add more candlestick pattern examples
- Add more options strategy payoff diagrams
- Translate to other languages
- Add more quiz questions
- Improve mobile responsiveness
- Add a dark/light theme toggle

**To contribute:**
1. Fork the repo
2. Create a branch: `git checkout -b feature/your-feature-name`
3. Make your changes to `index.html`
4. Commit: `git commit -m "Add: your feature description"`
5. Push: `git push origin feature/your-feature-name`
6. Open a Pull Request

---

## 📄 License

MIT License — free to use, modify, and distribute. See [LICENSE](LICENSE) for details.

---

## ⭐ If This Helped You

Give it a star on GitHub! It helps others find the project.

---

*Built with ❤️ for anyone who ever wanted to learn trading but didn't know where to start.*
