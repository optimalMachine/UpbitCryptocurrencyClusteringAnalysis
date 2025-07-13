# 🚀 Upbit Cryptocurrency Clustering Analysis

## 📋 Project Overview

This project analyzes cryptocurrencies on **Upbit Exchange** using **machine learning clustering techniques** to group coins with similar characteristics and help construct **efficient investment portfolios**.

### 🎯 Main Objectives
- 📊 Analyze cryptocurrency market patterns
- 🔍 Discover coin groups with similar characteristics
- 💼 Suggest portfolio compositions for diversification
- 📈 Develop risk-return based investment strategies

## 🛠️ Key Features

### 1. **Data Collection** 📥
- Real-time data collection via Upbit API
- 6-month (180 days) analysis using 4-hour candlesticks
- Data quality validation and continuity checks

### 2. **Feature Analysis** 📊
- **Return Metrics**: Mean returns, Sharpe ratio, Calmar ratio
- **Risk Metrics**: Volatility, Maximum Drawdown (MDD), Skewness, Kurtosis
- **Market Characteristics**: Positive return periods ratio, Session performance
- **Period Analysis**: Intraday/Weekly volatility, Monthly trends

### 3. **Clustering Analysis** 🎨
- Coin grouping using K-means algorithm
- Optimal cluster determination via Elbow Method and Silhouette Score
- Visualization through PCA (Principal Component Analysis)

### 4. **Visualization** 📈
- 9 detailed analysis charts
- Cluster-based feature heatmaps
- Risk-return scatter plots
- Correlation matrices

### 5. **Portfolio Recommendations** 💡
- Optimal coin selection from each cluster
- Top performers based on Sharpe ratio
- Diversification strategy suggestions

## 🚀 How to Use

### 1. Run on Google Colab
```python
# Required libraries will be installed automatically
!pip install pandas numpy matplotlib seaborn scikit-learn requests

# Run the code
# Copy and execute the entire code
```

### 2. Select Analysis Options
```
Select analysis option:
1. Analyze all coins (time-consuming)
2. Analyze top N coins only
3. Analyze major coins only (recommended) ← Recommended for beginners
```

### 3. Review Results
- 📊 Check coin groups by cluster
- 📈 Analyze visualization charts
- 💼 Review recommended portfolio
- 💾 Save results as CSV files

## 📊 Example Output

### Clustering Analysis Results
```
📊 Clustering Analysis Results:
============================================================
Optimal number of clusters: 4 (Silhouette Score: 0.421)

🔍 Coin Groups by Cluster:
============================================================
Cluster 0 (8 coins):
  Coins: BTC, ETH, BCH, LTC, ETC, NEO, QTUM, XLM
  - Average 4H return: 0.0234%
  - Average volatility: 1.2345%
  - Average Sharpe ratio: 0.8234
```

### Recommended Portfolio
```
🎲 Sample Portfolio Composition (10 coins):
  1. BTC (Sharpe ratio: 0.892, Volatility: 1.23%)
  2. ETH (Sharpe ratio: 0.845, Volatility: 1.45%)
  3. ADA (Sharpe ratio: 0.734, Volatility: 1.89%)
  ...
```

## 📁 Output Files

The program generates 3 CSV files after execution:

1. **`upbit_clustering_result_YYYYMMDD_HHMMSS.csv`**
   - Cluster assignment information for each coin

2. **`upbit_coin_features_YYYYMMDD_HHMMSS.csv`**
   - Detailed feature data for all coins

3. **`upbit_recommended_portfolio_YYYYMMDD_HHMMSS.csv`**
   - Recommended portfolio composition

## 📈 Chart Explanations

### 1. Elbow Method
- Chart for finding optimal cluster number
- "Elbow" point indicates optimal clusters

### 2. Silhouette Score
- Clustering quality evaluation
- Closer to 1 means better clustering

### 3. PCA Cluster Visualization
- High-dimensional data reduced to 2D
- Same color = same cluster

### 4. Feature Heatmap
- Coin features represented by colors
- Red: high values, Blue: low values

### 5. Cluster Mean Features
- Quick overview of each cluster's characteristics

### 6. Risk-Return Scatter Plot
- X-axis: Volatility (Risk)
- Y-axis: Mean Returns
- Top-left is ideal (low risk, high return)

### 7. Returns Distribution Boxplot
- Compare return distributions by cluster
- Box centerline: median

### 8. Correlation Matrix
- Price movement correlation between coins
- Closer to 1 means similar movements

### 9. Cluster Size Distribution
- Number and percentage of coins in each cluster

## ⚠️ Important Notes

1. **API Limits**: Upbit API has rate limits
2. **Execution Time**: Full analysis takes 30-60 minutes
3. **Network**: Stable internet connection required
4. **Data Interpretation**: Based on historical data, doesn't guarantee future returns

## 🔧 Tech Stack

- **Python 3.x**
- **Pandas**: Data processing
- **NumPy**: Numerical computations
- **Scikit-learn**: Machine learning (K-means, PCA)
- **Matplotlib/Seaborn**: Data visualization
- **Requests**: API communication

## 💡 Usage Tips

### For Beginners
1. Start with "3. Analyze major coins only" option
2. Build portfolio with coins from different clusters
3. Include BTC, ETH for stability

### For Advanced Users
1. Analyze all coins to find hidden gems
2. Use feature CSV data for further analysis
3. Develop hedging strategies considering cluster correlations

---

**⚡ Disclaimer**: This tool is not investment advice, and all investment decisions are at your own risk. Cryptocurrencies are high-risk assets with high volatility.
