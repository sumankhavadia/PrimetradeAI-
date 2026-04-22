# Hyperliquid × Fear & Greed Index — Trader Performance Analysis
### PrimeTrade.ai Data Science Intern Assignment

## Objective
Analyze how Bitcoin market sentiment (Fear/Greed) relates to trader 
behavior and performance on Hyperliquid perpetuals exchange.

## Setup & How to Run
1. Clone this repo
2. Install dependencies: `pip install pandas numpy matplotlib seaborn jupyter reportlab`
3. Place the two CSV datasets inside the `/data` folder
4. Run `Primetradeai_assignment.ipynb` top to bottom (Kernel → Restart & Run All)

## Dataset
- `fear_greed.csv` — Bitcoin Fear & Greed Index (2018–2025)
- `hyperliquid_trades.csv` — 211,175 trade executions (2024–2025)

## Key Findings
1. **Extreme Greed = highest accuracy** — Win rate peaks at 46.8% vs 
   36.8% in Extreme Fear
2. **Fear = largest position sizes** — Sophisticated traders size up 
   during panic, avg $7,818 vs $3,113 in Extreme Greed
3. **All regimes are profitable** — Total PnL positive across every 
   sentiment zone; strategy adaptation matters more than avoidance

## Strategy Recommendations
- **Greed:** Trend-follow, ride momentum, use trailing stops
- **Fear:** Contrarian longs with tight stops and oversized conviction bets
- **Neutral:** Reduce frequency, wait for clear sentiment signals

## Output Charts
| Figure | Description |
|--------|-------------|
| fig1 | Performance Dashboard — PnL, Win Rate, Volume by Sentiment |
| fig2 | Temporal Analysis — Daily PnL, F&G Evolution, Rolling Win Rate |
| fig3 | Asset & Trader Deep Dive — Top Coins, BUY/SELL Bias, Leaderboard |
| fig4 | Correlation Analysis — Scatter & Pearson Matrix |