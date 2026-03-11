# 📊 MScFE 632 — Machine Learning in Finance

**WorldQuant University | Master of Science in Financial Engineering**
**Course: 25/05 MScFE 632 Machine Learning in Finance**

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![Google Colab](https://img.shields.io/badge/Google%20Colab-Open-yellow?logo=googlecolab)](https://colab.research.google.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

---

## 📌 Course Overview

This repository contains all **Group Work Projects (GWPs)** completed for **MScFE 632 — Machine Learning in Finance** at **WorldQuant University**. The course covers the theory and practical application of machine learning techniques in financial markets, including unsupervised learning, supervised classification, and deep learning for portfolio optimization.

Each project folder contains:

- 📓 **Technical Colab notebooks** (Team Member A & B)
- 📄 **Final written report** (PDF)
- 📋 **Project guideline** (PDF from WQU)
- 📊 **Dataset** (Excel/CSV files)
- 📘 **Project-level README.md** with full methodology

---

## 🗂️ Repository Structure

```
MScFE-632-Machine-Learning-in-Finance/
│
├── GWP1/                                          # Unsupervised Learning — Stock Clustering
│   ├── README.md                                  ✅ Project summary & methodology
│   ├── GWP1_Team_Member_A.ipynb                   ✅ Notebook — Team Member A
│   ├── GWP1_Team_Member_B.ipynb                   ✅ Notebook — Team Member B
│   ├── GWP1_Final_Report.pdf                      ✅ Written non-technical report
│   ├── Project guideline from WQU 1.pdf           ✅ Project guideline
│   ├── Primary dataset (combined stock prices).xlsx ✅ Primary dataset
│   └── Secondary dataset.xlsx                     ✅ Secondary dataset
│
├── GWP2/                                          # Supervised Learning — Market Regime Classification
│   ├── README.md                                  ✅ Project summary & methodology
│   ├── GWP2_Team_Member_A.ipynb                   ✅ Notebook — Team Member A
│   ├── GWP2_Team_Member_B.ipynb                   ✅ Notebook — Team Member B
│   ├── GWP2_Final_Report.pdf                      ✅ Written non-technical report
│   ├── Project guideline from WQU 2.pdf           ✅ Project guideline
│   └── Financial market dataset.xlsx              ✅ Financial market dataset
│
├── GWP3/                                          # Deep Learning — LSTM Portfolio Optimization
│   ├── README.md                                  ✅ Project summary & methodology
│   ├── GWP3_Team_Member_A.ipynb                   ✅ Notebook — Team Member A
│   ├── GWP3_Team_Member_B.ipynb                   ✅ Notebook — Team Member B
│   ├── GWP3_Final_Report.pdf                      ✅ Written non-technical report
│   └── Project guideline from WQU 3.pdf           ✅ Project guideline
│
└── README.md                                      ✅ Main repository overview (this file)
```

---

## 📁 Group Work Projects

### 🔵 GWP 1 — Unsupervised Learning: Stock Clustering in Financial Markets

> **Topic:** Applying K-Means & Hierarchical Clustering to identify stock market groupings and sector patterns during the 2008 Financial Crisis.

| Resource | Link |
|---|---|
| 📘 Project README | [GWP1/README.md](./GWP1/README.md) |
| 🧑‍💻 Notebook — Team Member A | [GWP1_Team_Member_A.ipynb](./GWP1/GWP1_Team_Member_A.ipynb) |
| 👤 Notebook — Team Member B | [GWP1_Team_Member_B.ipynb](./GWP1/GWP1_Team_Member_B.ipynb) |
| 📄 Final Report | [GWP1_Final_Report.pdf](./GWP1/GWP1_Final_Report.pdf) |
| 📋 Guideline | [Project guideline from WQU 1.pdf](<./GWP1/Project guideline from WQU 1.pdf>) |
| 📊 Primary Dataset | [Primary dataset (combined stock prices).xlsx](<./GWP1/Primary dataset (combined stock prices).xlsx>) |
| 📊 Secondary Dataset | [Secondary dataset.xlsx](./GWP1/Secondary%20dataset.xlsx) |

**Key Methods:** K-Means Clustering · Hierarchical Clustering · Dendrogram · PCA · Silhouette Score

---

### 🟢 GWP 2 — Supervised Learning: Market Regime Classification with SVM

> **Topic:** Using Support Vector Machines (SVM) to classify and predict financial market regimes (bull/bear/neutral) from engineered features.

| Resource | Link |
|---|---|
| 📗 Project README | [GWP2/README.md](./GWP2/README.md) |
| 🧑‍💻 Notebook — Team Member A | [GWP2_Team_Member_A.ipynb](./GWP2/GWP2_Team_Member_A.ipynb) |
| 👤 Notebook — Team Member B | [GWP2_Team_Member_B.ipynb](./GWP2/GWP2_Team_Member_B.ipynb) |
| 📄 Final Report | [GWP2_Final_Report.pdf](./GWP2/GWP2_Final_Report.pdf) |
| 📋 Guideline | [Project guideline from WQU 2.pdf](<./GWP2/Project guideline from WQU 2.pdf>) |
| 📊 Dataset | [Financial market dataset.xlsx](<./GWP2/Financial market dataset.xlsx>) |

**Key Methods:** SVM · Feature Engineering · TimeSeriesSplit CV · ROC-AUC · Backtesting

---

### 🟠 GWP 3 — Deep Learning: LSTM-Based Portfolio Optimization

> **Topic:** LSTM networks + Random Forest signals for adaptive portfolio weight allocation and time-series forecasting.

| Resource | Link |
|---|---|
| 📙 Project README | [GWP3/README.md](./GWP3/README.md) |
| 🧑‍💻 Notebook — Team Member A | [GWP3_Team_Member_A.ipynb](./GWP3/GWP3_Team_Member_A.ipynb) |
| 👤 Notebook — Team Member B | [GWP3_Team_Member_B.ipynb](./GWP3/GWP3_Team_Member_B.ipynb) |
| 📄 Final Report | [GWP3_Final_Report.pdf](./GWP3/GWP3_Final_Report.pdf) |
| 📋 Guideline | [Project guideline from WQU 3.pdf](<./GWP3/Project guideline from WQU 3.pdf>) |

**Key Methods:** LSTM · PyTorch · Random Forest Signals · Reinforcement Learning Env · Bayesian Hyperparameter Optimization

---

## 🛠️ Technologies & Libraries

| Category | Tools |
|---|---|
| Language | Python 3.x |
| Environment | Google Colab / Jupyter Notebook |
| Data Manipulation | pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | scikit-learn, scikit-optimize |
| Deep Learning | PyTorch (torch, nn, optim) |
| Finance | yfinance, custom portfolio environments |

---

## 📚 Course Information

| Field | Details |
|---|---|
| University | WorldQuant University (WQU) |
| Program | Master of Science in Financial Engineering (MScFE) |
| Course Code | MScFE 632 |
| Course Name | Machine Learning in Finance |
| Cohort | 25/05 |
| Projects | GWP1 · GWP2 · GWP3 |

---

## 👤 Author

**MD RASHEDUL ISLAM RASEL**
MScFE Student — WorldQuant University

[![GitHub](https://img.shields.io/badge/GitHub-Rashed17a-black?logo=github)](https://github.com/Rashed17a)

> *This repository is maintained for academic and portfolio purposes.*
