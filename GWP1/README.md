# 📘 GWP 1 — Unsupervised Learning: Stock Clustering in Financial Markets

**MScFE 632 Machine Learning in Finance | WorldQuant University**
Cohort: 25/05 | Group Work Project 1

---

## 🎯 Project Objective

This project applies unsupervised machine learning techniques to cluster stocks based on their return profiles and correlation structures during the **2008 Financial Crisis**. The goal is to identify natural groupings in financial assets that can inform diversification strategies and risk management.

---

## 🗂️ Folder Contents

| File | Type | Description |
|---|---|---|
| `GWP1_Team_Member_A.ipynb` | 📓 Notebook | Technical implementation — Team Member A |
| `GWP1_Team_Member_B.ipynb` | 📓 Notebook | Technical implementation — Team Member B |
| `GWP1_Final_Report.pdf` | 📄 PDF | Written non-technical report |
| `Project guideline from WQU 1.pdf` | 📋 PDF | Project guideline from WQU |
| `Primary dataset (combined stock prices).xlsx` | 📊 Excel | Primary dataset (combined stock prices) |
| `Secondary dataset.xlsx` | 📊 Excel | Secondary dataset |

---

## 🔬 Methodology

The project follows a structured pipeline:

**1. Data Acquisition & Preprocessing**
- Historical stock price data for 29 S&P 500 companies (2008–2009)
- Computed daily log returns
- Built correlation matrix to capture co-movement between stocks

**2. Exploratory Analysis**
- Correlation heatmap visualization
- Return distribution analysis

**3. Unsupervised Clustering Models**
- **K-Means Clustering** — partitioned stocks into k optimal clusters using Elbow Method and Silhouette Score
- **Hierarchical Clustering** — built a dendrogram to visualize nested groupings

**4. Evaluation**
- Silhouette Score to validate cluster quality
- Visual inspection of dendrograms
- Sector-level analysis of cluster composition

---

## 📊 Key Results

- Stocks clustered meaningfully into **3–5 distinct groups** based on correlation during the crisis
- Financial sector stocks (BAC, C, JPM, WFC) clustered tightly — confirming systemic risk concentration
- Defensive/utility stocks (XOM, DUK, REG) formed separate clusters with lower correlation to financials
- Hierarchical clustering dendrograms confirmed the K-Means groupings

---

## 🛠️ Libraries Used

```
pandas, numpy, matplotlib, seaborn
sklearn (KMeans, AgglomerativeClustering, silhouette_score)
scipy (linkage, dendrogram, leaves_list)
```

---

## 📁 Data Sources

- **Primary Dataset:** Combined stock price data (2008 Q4)
- **Secondary Dataset:** Extended historical data
- Source: Yahoo Finance / WQU provided datasets

---

## 🔗 Quick Links

| Resource | Link |
|---|---|
| 📓 Notebook Team A | [GWP1_Team_Member_A.ipynb](./GWP1_Team_Member_A.ipynb) |
| 📓 Notebook Team B | [GWP1_Team_Member_B.ipynb](./GWP1_Team_Member_B.ipynb) |
| 📄 Final Report | [GWP1_Final_Report.pdf](./GWP1_Final_Report.pdf) |
| 📋 Guideline | [Project guideline from WQU 1.pdf](<./Project guideline from WQU 1.pdf>) |
| 📊 Primary Dataset | [Primary dataset (combined stock prices).xlsx](<./Primary dataset (combined stock prices).xlsx>) |
| 📊 Secondary Dataset | [Secondary dataset.xlsx](./Secondary%20dataset.xlsx) |

---

*Part of MScFE 632 — Machine Learning in Finance | WorldQuant University*
