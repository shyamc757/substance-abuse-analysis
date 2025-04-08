# 📊 Dynamics of Substance Abuse: A Dual Project Analysis

This repository explores trends and patterns in substance abuse across U.S. metropolitan areas using data from the **Drug Abuse Warning Network (DAWN)**. The dataset includes over **2.2 million hospital emergency room records** from 2004 to 2011, offering a rich basis for data mining and public health insights.

---

## 🧠 Project Overview

This work is divided into **two distinct yet interconnected projects**, both built on a common data foundation and processing pipeline.

### 🧩 Project 1: Pattern Mining & Classification
Focuses on discovering substance abuse patterns and building predictive models to classify abuse cases based on demographic and geographic features.

Key methods:
- Pattern mining using FP-Growth
- Jaccard similarity across metro areas
- Classification using CatBoost, Random Forest, Naive Bayes
- Feature importance analysis

📁 [`pattern-mining-classification/`](./pattern-mining-classification) — includes its own `README.md`

---

### 📈 Project 2: Time Series Forecasting & Granger Causality
Analyzes temporal trends and explores whether economic indicators like the housing market crash in 2008 can help predict changes in substance abuse cases.

Key methods:
- Forecasting with Facebook Prophet
- Granger causality test for economic influence

📁 [`time-series-forecasting/`](./time-series-forecasting) — includes its own `README.md`

---

## ⚙️ Data Preprocessing

All data cleaning and preparation steps are handled in a shared preprocessing notebook.

📁 [`data_processing/data_preprocessing.ipynb`](./data-processing/data_preprocessing.ipynb)

> **Note:** The raw data is excluded from this repository. Refer to the DAWN [official source](https://www.samhsa.gov/data/data-we-collect/dawn-drug-abuse-warning-network) for access.

---

## 📄 Project Report

For a full deep dive into methodology, analysis, visuals, and results:

📄 [`report/Data_Mining_Paper.pdf`](./report/Data%20Mining%20Paper.pdf)

---

## 📦 Repository Structure

```
substance-abuse-analysis/
│
├── pattern-mining-classification/     # Project 1: Classification & pattern mining
│   ├── classifiers.ipynb
│   ├── feature_importance.ipynb
│   ├── fp_growth_pattern_mining.ipynb
│   ├── visualizations.ipynb
│   └── README.md
│
├── time-series-forecasting/           # Project 2: Time series & Granger causality
│   ├── prophet_forecasting.ipynb
│   ├── granger_causality_analysis.ipynb
│   └── README.md
│
├── data-processing/                   # Shared preprocessing for both projects
│   └── data_preprocessing.ipynb
│
├── report/                            # Research paper write-up
│   └── Data Mining Paper.pdf
│
└── README.md                          # Master README (this file)
```

---

## 📥 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/substance-abuse-analysis.git
   ```

2. Install the required dependencies in your Python environment.

3. Open the relevant Jupyter notebooks in each project folder to explore the code.

---

## 🙏 Acknowledgments

Special thanks to **Professor Jiebo Luo** for invaluable guidance throughout this project.

---

## 📜 License

This project is licensed under the MIT License.
