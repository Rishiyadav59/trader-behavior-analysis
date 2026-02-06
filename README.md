# Trader Behavior Insights: Sentiment vs. Performance

## 📌 Project Overview
An analysis of how Bitcoin market sentiment (Fear/Greed) influences trader behavior and profitability on the Hyperliquid exchange.

## 🛠️ Setup & Execution
1. Clone this repository.
2. Ensure you have `pandas`, `seaborn`, and `matplotlib` installed.
3. Run the Jupyter Notebook `analysis.ipynb`. The script automatically handles:
   - Timestamp normalization (ms to daily).
   - Inner-merging trade logs with sentiment data.
   - Metric engineering (Win Rate, PnL, Trade Frequency).

## 📊 Methodology
- **Data Cleaning**: Aligned millisecond-level trade data with daily sentiment classification.
- **Segmentation**: Categorized traders into 'High Frequency' vs 'Low Frequency' based on daily trade counts to identify which group is more susceptible to sentiment shifts.

## 💡 Key Insights
- **Performance**: [Insert your finding, e.g., "Win rates dropped by 10% during Extreme Greed, indicating over-trading."]
- **Behavior**: [Insert your finding, e.g., "Trade frequency doubled during Fear days for the high-leverage segment."]

## 🚀 Actionable Strategy Recommendations
1. **The Volatility Buffer**: During "Extreme Fear" (Index < 25), implement a 30% reduction in maximum allowable position size for accounts with high trade frequency.
2. **Greed Filter**: Limit new entry orders for traders with a 3-day declining win rate when sentiment is > 75 (Extreme Greed).# trader-behavior-analysis
