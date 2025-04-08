# 📈 Project 2: Time Series Forecasting & Granger Causality

This subproject focuses on modeling and forecasting trends in substance abuse over time, and investigating the **economic factors** that may influence those trends. It uses time series analysis and causality testing to uncover how external shocks — like the 2008 housing crash — relate to shifts in public health behavior.

This is the second half of the broader **substance-abuse-analysis** repository, based on real-world data from the **Drug Abuse Warning Network (DAWN)** — a national database tracking drug-related emergency room visits across U.S. metro areas.



## 🌍 Why This Matters

Understanding the **temporal dynamics** of substance abuse is essential for proactive public health policy.

This project goes beyond "what is happening" to ask **"when and why?"** — exploring how events like economic downturns may correlate with, or even predict, spikes in drug and alcohol-related ER visits.

By forecasting abuse patterns and testing for Granger causality, this project can:
- Help policy makers **anticipate** public health risks
- Guide **resource planning** for healthcare systems
- Inform **economic intervention strategies** linked to substance abuse



## 🔍 Objectives

- Forecast future trends in substance abuse cases using historical data
- Evaluate forecasting performance using statistical metrics
- Test whether economic indicators (e.g., housing market trends) influence public health outcomes
- Highlight time lags where economic changes precede abuse surges



## ⚙️ Components

### 1. `prophet_forecasting.ipynb`
- Uses Facebook Prophet to forecast ER visit trends related to substance abuse
- Evaluates model performance with RMSE and MAPE
- Highlights unexpected dips post-2008 that the model couldn't anticipate

### 2. `granger_causality_analysis.ipynb`
- Overlays drug abuse time series with housing price index
- Conducts Granger causality tests across multiple lag values
- Identifies statistically significant lags where housing market trends **precede** shifts in drug abuse



## 📊 Highlights

- Forecasting revealed a **significant decline in abuse cases after 2008**, which Prophet could not predict — suggesting an external disruption
- **Granger causality tests** confirmed that housing price trends have a statistically significant predictive relationship with substance abuse at certain time lags
- These findings imply that **economic indicators could act as early warning signals** for future substance abuse spikes



## 📁 Folder Location

This project lives in the [`time-series-forecasting/`](./) folder of the main repository.

It shares preprocessed data with:
- [`pattern-mining-classification/`](../pattern-mining-classification)
- [`data_processing/`](../data_processing)



## 📎 Related

📄 For full methodology and context, see the [main report](../report/Data_Mining_Paper.pdf)  
📁 Return to the [main repository README](../README.md)



## 📜 License

This project is part of the `substance-abuse-analysis` repository and is licensed under the MIT License.
