# 📗 GWP 2 — Supervised Learning: Market Regime Classification with SVM

> **MScFE 632 Machine Learning in Finance | WorldQuant University**
> Cohort: 25/05 | Group Work Project 2

---

## 🎯 Project Objective

This project applies **Support Vector Machines (SVM)** and supervised classification techniques to identify and predict **financial market regimes** (bull / bear / neutral) based on historical price data and engineered financial features. The model is trained and evaluated on real market data with a full backtesting framework.

---

## 🗂️ Folder Contents

| File | Type | Description |
|------|------|-------------|
| `GWP2_Team_Member_A.ipynb` | 📓 Notebook | Technical implementation — Team Member A |
| `GWP2_Team_Member_B.ipynb` | 📓 Notebook | Technical implementation — Team Member B |
| `Final_Report.pdf` | 📄 PDF | Written non-technical report |
| `Guideline.pdf` | 📋 PDF | Project guideline from WQU |
| `dataset.csv` | 📊 CSV | Financial market dataset |

---

## 🔬 Methodology

**1. Data Acquisition & Feature Engineering**
- Historical price data for S&P 500 index and individual stocks
- Engineered features: returns, volatility (rolling std), momentum (12M return), credit spreads, VIX, Yield Spread Lag
- Labeled market regimes: Bull (>5% return), Bear (<-5%), Neutral

**2. Model Training**
- **Support Vector Machine (SVM)** with RBF and linear kernels
- Hyperparameter tuning: C, gamma via Grid Search with cross-validation
- TimeSeriesSplit for proper financial time-series validation (no look-ahead bias)

**3. SVM Decision Boundary Illustration**
- Visualized SVM decision boundaries on Volatility vs. Momentum feature space
- Bull / Bear / Neutral region classification

**4. Model Evaluation**
- Accuracy, Precision, Recall, F1-Score
- Confusion Matrix analysis
- ROC-AUC curve
- Backtesting on out-of-sample period (2023)

---

## 📊 Key Results

- SVM with RBF kernel achieved the best classification performance
- Model correctly identified major regime shifts during high-volatility periods
- Regime-adaptive portfolio (24.1% annual return) significantly outperformed static 60/40 portfolio (10.3%)
- Max Drawdown reduced from -18.1% (static) to -9.2% (regime-adaptive)

---

## 🛠️ Libraries Used

```python
pandas, numpy, matplotlib, seaborn
sklearn (SVC, GridSearchCV, TimeSeriesSplit, confusion_matrix, roc_auc_score)
```

---

## 📁 Data Sources

- Combined financial market data (2018–2024)
- Features: Returns, Volatility, Momentum, Credit Spreads, VIX

---

## 🔗 Quick Links

| Resource | Link |
|----------|------|
| 📓 Notebook Team A | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mAHH62LApMyhyzYikPjy6Ld7ITf2-jOy) |
| 📓 Notebook Team B | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1JmJWVPMYRUEbAEQMHzZp4344NBlHcfJV) |
| 📊 Dataset | [Google Sheets](https://docs.google.com/spreadsheets/d/1lk4KJzXPWAG2BDJdy5572qjA7MMiJLf72QtOWodVsNA/edit?gid=858330135#gid=858330135) |
| 📋 Guideline | [Google Drive](https://drive.google.com/file/d/1Fbc5t-bsbZfkMp-vSqJQODpIJyLkdZVI/view) |
| 📄 Final Report | [Download PDF](https://wqet-production-uploads-7dm4.s3.us-east-1.amazonaws.com/9fb360c2bffecf2f64b9a4d8c3a1b06f909e5b71ba41da394bcf7b8b2ba20249.pdf) |

---

*Part of MScFE 632 — Machine Learning in Finance | WorldQuant University*
