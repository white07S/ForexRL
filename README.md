# ForexRL
A Deep Reinforcement Learning model for high volume Forex Portfolio Management

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
