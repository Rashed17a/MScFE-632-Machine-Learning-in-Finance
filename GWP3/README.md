# 📙 GWP 3 — Deep Learning: LSTM-Based Portfolio Optimization

> **MScFE 632 Machine Learning in Finance | WorldQuant University**
> Cohort: 25/05 | Group Work Project 3

---

## 🎯 Project Objective

This project applies **deep learning** — specifically **Long Short-Term Memory (LSTM) networks** — combined with **Random Forest signals** and **reinforcement learning principles** to build an intelligent, adaptive portfolio optimization system. The model learns from historical return patterns to generate trading signals and dynamically allocate portfolio weights.

---

## 🗂️ Folder Contents

| File | Type | Description |
|------|------|-------------|
| `GWP3_Team_Member_A.ipynb` | 📓 Notebook | Technical implementation — Team Member A |
| `GWP3_Team_Member_B.ipynb` | 📓 Notebook | Technical implementation — Team Member B |
| `Guideline.pdf` | 📋 PDF | Project guideline from WQU |

---

## 🔬 Methodology

**1. Data Acquisition & Feature Engineering**
- Historical price data for S&P 500 stocks (2018–2024)
- Log returns computation
- Rolling features: return, volatility (rolling std), mean, Sharpe proxy
- Random Forest trading signals as auxiliary input features

**2. Random Forest Signal Generation**
- Trained Random Forest classifier on lagged features to predict next-period direction
- Signals used as additional features to augment LSTM training

**3. LSTM Portfolio Model**
- Sequence-based input window (10 timesteps)
- LSTM architecture with hidden_dim=128, fully connected output layer
- Softmax activation for portfolio weights (long-only constraint)
- Custom reinforcement learning environment: `FeaturePortfolioEnv`
- Reward function: portfolio return per step

**4. Hyperparameter Optimization (Team A)**
- Bayesian Optimization with `scikit-optimize` (BayesSearchCV)
- Optimized SVM and Random Forest models for market regime tasks
- Convergence plots and performance vs. hyperparameter visualization

**5. Backtesting**
- Walk-forward evaluation on held-out test period
- Compared LSTM portfolio vs. equal-weight benchmark
- Performance metrics: Sharpe Ratio, Cumulative Return, Max Drawdown

---

## 📊 Key Results

- LSTM portfolio dynamically adjusted weights based on regime and momentum signals
- Random Forest signals improved directional accuracy over naive baseline
- Bayesian hyperparameter optimization reduced training time while improving F1-score
- Feature engineering (Sharpe proxy, rolling vol) provided strong predictive signal

---

## 🛠️ Libraries Used

```python
# Team Member A
pandas, numpy, matplotlib, seaborn
sklearn (RandomForestClassifier, SVC, TimeSeriesSplit)
scikit-optimize (BayesSearchCV, skopt.plots)

# Team Member B
pandas, numpy, matplotlib
torch (nn.LSTM, nn.Linear, Softmax)
torch.optim (Adam)
sklearn (RandomForestClassifier, StandardScaler)
```

---

## 🔗 Quick Links

| Resource | Link |
|----------|------|
| 📓 Notebook Team A | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1MOdphNcDbjouzm-BxD5uD0LkAiuPgLO7) |
| 📓 Notebook Team B | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1NUYzzry_ynyH0CHHs0z0ukquzfArSzA2) |
| 📋 Guideline | [Google Drive](https://drive.google.com/file/d/1ELr2Q7HOLT4VjStrOaF9Usi0Lsv6EpJY/view) |

---

*Part of MScFE 632 — Machine Learning in Finance | WorldQuant University*
