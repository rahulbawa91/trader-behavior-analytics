# 📊 Market Sentiment vs Trader Behavior (Hyperliquid)

##  Overview
This project analyzes how **Bitcoin market sentiment (Fear/Greed index)** impacts trader behavior and performance on Hyperliquid.  
The goal is to uncover patterns that can help design **data-driven trading strategies**.

---

##  Methodology

### 🔹 Data Sources
- **Fear/Greed Dataset**: Market sentiment classification (Fear / Greed)
- **Hyperliquid Historical Data**: Trade-level data (PnL, size, side, timestamp, etc.)

### 🔹 Data Preparation
- Cleaned missing values and removed duplicates  
- Standardized column names  
- Converted timestamps to datetime format  
- Aligned both datasets at a **daily level** using date  

### 🔹 Feature Engineering
Key metrics created:
- **Daily PnL per trader**
- **Win rate** (percentage of profitable trades)
- **Average trade size (USD)**
- **Trading frequency** (number of trades per day)
- **Long/Short ratio** (buy vs sell activity)

---

##  Key Insights

### 1. Performance varies with sentiment
- Traders experience **lower average PnL during Fear periods**
- **Higher volatility** in returns during Fear
- Win rates tend to decrease in uncertain conditions

### 2. Behavioral changes in different market regimes
- **Fear Periods:**
  - Increased trading frequency (panic trading)
  - Inconsistent outcomes
- **Greed Periods:**
  - More stable performance
  - Larger position sizes (overconfidence)

### 3. Trader segmentation insights
- **Frequent traders** underperform during Fear due to overtrading  
- **Consistent traders** maintain stable performance across conditions  
- **High-volume traders** are more exposed to volatility swings  

---

##  Strategy Recommendations

### 1. Risk Management Rule
- During **Fear periods**:
  - Reduce position sizes  
  - Avoid overtrading  
- During **Greed periods**:
  - Avoid excessive leverage  

---

### 2. Segment-Based Strategy
- **Consistent traders** → Can trade during volatile Fear periods  
- **Infrequent traders** → Should reduce activity during Fear  

---

### 3. Sentiment-Based Trading Signal
- Use sentiment as a **contrarian indicator**:
  - **Extreme Fear → Potential buying opportunity**
  - **Extreme Greed → Possible market correction**

---

##  Conclusion
Market sentiment significantly influences trader behavior and performance.  
- **Fear → volatility + overtrading**
- **Greed → stability + overconfidence**

Incorporating sentiment into trading decisions can improve **risk management and profitability**.

---

##  Tech Stack
- Python (Pandas, NumPy)
- Data Visualization (Matplotlib, Seaborn)
- Machine Learning (optional: Scikit-learn)

---

##  Future Work
- Build predictive models for trader profitability  
- Cluster traders into behavioral archetypes  
- Develop a Streamlit dashboard for interactive analysis  

---