# 📘 GWP 1 — Unsupervised Learning: Stock Clustering in Financial Markets

> **MScFE 632 Machine Learning in Finance | WorldQuant University**
> Cohort: 25/05 | Group Work Project 1

---

## 🎯 Project Objective

This project applies **unsupervised machine learning** techniques to cluster stocks based on their return profiles and correlation structures during the **2008 Financial Crisis**. The goal is to identify natural groupings in financial assets that can inform diversification strategies and risk management.

---

## 🗂️ Folder Contents

| File | Type | Description |
|------|------|-------------|
| `GWP1_Team_Member_A.ipynb` | 📓 Notebook | Technical implementation — Team Member A |
| `GWP1_Team_Member_B.ipynb` | 📓 Notebook | Technical implementation — Team Member B |
| `Final_Report.pdf` | 📄 PDF | Written non-technical report |
| `Guideline.pdf` | 📋 PDF | Project guideline from WQU |
| `dataset_1.csv` | 📊 CSV | Primary dataset (combined stock prices) |
| `dataset_2.csv` | 📊 CSV | Secondary dataset |

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

```python
pandas, numpy, matplotlib, seaborn
sklearn (KMeans, AgglomerativeClustering, silhouette_score)
scipy (linkage, dendrogram, leaves_list)
```

---

## 📁 Data Sources

- Dataset 1: Combined stock price data (2008 Q4)
- Dataset 2: Extended historical data
- Source: Yahoo Finance / WQU provided datasets

---

## 🔗 Quick Links

| Resource | Link |
|----------|------|
| 📓 Notebook Team A | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kzlPNnUv9Vz9T9UX1IRbpPJJZ_5xj4Gb) |
| 📓 Notebook Team B | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1cv3SjUVmS2RjuVpZzljmGbhAjKBH9Abc) |
| 📊 Dataset 1 | [Google Sheets](https://docs.google.com/spreadsheets/d/1nXpqKyao-yfAzCblZj5sZiZ-hvaJX46sEVhuR54Zy80/edit?gid=125658626#gid=125658626) |
| 📊 Dataset 2 | [Google Sheets](https://docs.google.com/spreadsheets/d/1jp_N85YSPMvnzD0yjxsItj-ZXL7p80k6mpWxzLZp7Cc/edit?gid=745697357#gid=745697357) |
| 📋 Guideline | [Google Drive](https://drive.google.com/file/d/1fif_w0oM9UQCY0i107j4KZrPBnFTjcFT/view) |
| 📄 Final Report | [Download PDF](https://wqet-production-uploads-7dm4.s3.us-east-1.amazonaws.com/326044f022cd8aef34196d1f996d2e1e193378d24e1b7f47cdac56d51f26a73d.pdf) |

---

*Part of MScFE 632 — Machine Learning in Finance | WorldQuant University*
