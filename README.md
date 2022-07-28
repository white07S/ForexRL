# ForexRL
A Deep Reinforcement Learning model for high volume Forex Portfolio Management

![GitHub](https://img.shields.io/github/license/white07S/ForexRL)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/white07S/ForexRL)
![GitHub repo size](https://img.shields.io/github/repo-size/white07S/ForexRL)
![GitHub last commit](https://img.shields.io/github/last-commit/white07S/ForexRL)

# Attributes

| Constraints      | Description |
| ----------- | ----------- |
| Features      | FX market is represented via 512 features in X_train and X_test.     |
| Summary  | 512 features summarizes the price-actions of 10+1 assets in past 10 days.        |
| Return | Hourly log returns of assets during train & test periods are in y_train and y_test. |
| Risk | Calmar, Sortino, Omega ratio(s), etc. (Included but limited)|
  
# GPU Results
 | Constraints | Result |
 | ----------- | -------- |
 | Max. Drawdown |  6.24% | 
 | Sortino Ratio |  10.10x |
 | Sharpe Ratio |  3.15x |  
 | Stability |  91.31% |
 | Tail Ratio | 3.57x | 
 | Value at Risk |  -0.84% |
 
# CPU is not tested

# Install and Run
# Note: Don't forget to unzip the Xtrain tar file
```
pip install -r requirements.txt
```
Pytorch implementation with GPU and CPU version seprately with shared auto encoder

```
python gpu.py
```

Run autoencoder for plots and results
```
python autoencoder.py
```

# Results

**Daily Portfolio Balances**
![DPB](https://github.com/white07S/ForexRL/blob/main/graphs/portfolio_weights.png)
**Annual Cumulative Return**
![](https://github.com/white07S/ForexRL/blob/main/graphs/cumulative_return.png)
**Weekly Portfolio Log Return**
![](https://github.com/white07S/ForexRL/blob/main/graphs/weekly_returns.png)
**Autoencoder Interpretation**
![](https://github.com/white07S/ForexRL/blob/main/graphs/autoencoder.png)

# Caution: Don't use it for live forex market.
