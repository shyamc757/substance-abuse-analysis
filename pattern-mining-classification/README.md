# 🧩 Project 1: Pattern Mining & Classification

This subproject focuses on uncovering patterns in substance abuse cases and building classification models to predict the type of abuse based on demographic and regional attributes.

It forms one half of the broader **substance-abuse-analysis** repository, built on real-world data from the **Drug Abuse Warning Network (DAWN)** — a national surveillance system that tracks drug-related visits to emergency departments across the U.S.



## 🌍 Why This Matters

Substance abuse is not only a personal health issue but a major societal challenge. Its patterns are deeply influenced by social, economic, and regional factors — making it crucial to detect where and how abuse manifests.

This project aims to:
- Help **public health officials** identify at-risk demographics
- Guide **regional interventions** with localized pattern analysis
- Enable **preventive policies** through machine learning–driven predictions
- Offer a scalable framework that could be extended to new or evolving abuse trends

By combining pattern mining with predictive modeling, this work provides both **interpretability and actionability**, helping move from insight to intervention.



## 🔍 Objectives

- Discover frequent patterns in substance use across different metro areas
- Compare regional similarities using Jaccard similarity
- Classify abuse cases using machine learning models
- Analyze feature importance to understand key predictive factors



## ⚙️ Components

### 1. `fp_growth_pattern_mining.ipynb`
- Applies the FP-Growth algorithm to find frequent and unique substance abuse patterns
- Extracts patterns by metro area and time range
- Calculates Jaccard similarity heatmaps to show regional overlaps

### 2. `visualizations.ipynb`
- Provides rich exploratory visuals for:
  - Age-wise abuse distribution
  - Time-of-day analysis
  - Geographic variation across U.S. metro areas

### 3. `classifiers.ipynb`
- Compares performance of:
  - Random Forest
  - CatBoost
  - Naive Bayes
- Evaluates with precision, recall, F1-score, and accuracy metrics

### 4. `feature_importance.ipynb`
- Uses Random Forest to assess the predictive power of:
  - Demographics (age, sex, race)
  - Location (metro area)
  - Case attributes (time of day, type of abuse)



## 📊 Highlights

- **Alcohol abuse among individuals under 21** is consistently prominent
- **Metro-level drug patterns** vary greatly, emphasizing the need for localized strategies
- **CatBoost outperformed other models** in predicting substance abuse types
- **Feature importance** revealed that certain predictors (like age or case type) vary in relevance year-to-year and city-to-city



## 📁 Folder Location

This project lives in the [`pattern-mining-classification/`](./) folder of the main repository.

It shares preprocessed data with:
- [`time-series-forecasting/`](../time-series-forecasting)
- [`data_processing/`](../data_processing)



## 📎 Related

📄 For full methodology and context, see the [main report](../report/Data_Mining_Paper.pdf)  
📁 Return to the [main repository README](../README.md)



## 📜 License

This project is part of the `substance-abuse-analysis` repository and is licensed under the MIT License.
