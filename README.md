# Trader Performance vs Market Sentiment Analysis
### Candidate: Chakradhar Rao
### Role: Data Science / Analytics Intern
### Team: Web3 Trading Analytics

---

## 📌 Project Overview

This project analyzes how trader behavior and profitability on Hyperliquid align with Bitcoin market sentiment regimes (Fear, Greed, Extreme Greed, Neutral).

The objective is to uncover regime-based behavioral patterns, evaluate performance dispersion across sentiment conditions, and derive actionable strategy recommendations that improve risk-adjusted returns.

---

## 📂 Project Structure

chakradhar_rao_ds_assign/
├── notebook_1.ipynb         # Data cleaning & feature engineering  
├── notebook_2.ipynb         # Behavioral analysis & ML modeling  
├── csv_files/               # Processed datasets  
│   ├── daily_trader_metrics.csv  
│   └── trader_risk_profile.csv  
├── outputs/                 # Generated charts & visual outputs  
│   ├── pnl_by_sentiment.png  
│   ├── trade_count_by_sentiment.png  
│   ├── long_ratio_by_sentiment.png  
│   └── ml_feature_importance.png  
├── ds_report.pdf            # Executive summary report  
└── README.md                # Setup & documentation  

---

## 🛠 Methodology

### Data Engineering
- Timestamp normalization (Unix → datetime)
- Daily alignment of trades with sentiment data
- Clean merge validation (no missing sentiment labels)
- Event-driven regime analysis (6 high-volume dates)

### Feature Engineering
- Daily PnL
- Trade count
- Total volume (USD)
- Average trade size
- Win rate
- Long bias ratio
- Fee intensity

### Segmentation
- High Activity vs Low Activity traders
- Volatility-based trader profiling

### Statistical Testing
- Independent t-test between Fear and Greed regimes
- Risk-adjusted return comparison (mean / std PnL)

### Predictive Modeling
- Random Forest classifier
- Binary profitability prediction (daily PnL > 0)
- Feature importance analysis

---

## 🔥 Key Insights

1. Fear regimes produced the highest average and risk-adjusted profitability.
2. Greed regimes increased activity but reduced execution efficiency.
3. Low-activity traders significantly underperformed during Extreme Greed.
4. Profitability is strongly regime-dependent and behavior-sensitive.

---

## 🚀 Strategy Implications

- Fear Regime Acceleration Strategy  
- Greed Regime Risk Throttle  
- Sentiment-Aware Execution Controls  

---

## ▶️ How to Run

1. Open notebooks in Google Colab.
2. Upload the original CSV datasets.
3. Run `notebook_1.ipynb` to generate processed data.
4. Run `notebook_2.ipynb` for analysis, segmentation, and ML modeling.
5. All charts will be saved automatically in the `outputs/` directory.

---

## 📌 Notes

- Dataset is event-driven (6 major trading dates).
- Results should be interpreted as exploratory due to limited event samples.
- All steps are fully reproducible.
