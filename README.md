# Market Correlation Analysis and Prediction
📚 Project Overview
This project investigates the relationship between major stock indices (DowJones, SP500, NASDAQ) and cryptocurrencies (Bitcoin, Ethereum, BinanceCoin) over the period 2020–2024.

We analyze their correlations, test for Granger causality, and build predictive models to see whether including cryptocurrency returns improves the prediction of stock index returns.

📈 Main Steps:
Downloaded financial data using yfinance.

Performed data preprocessing and return calculation.

Conducted correlation analysis.

Conducted Granger causality tests.

Built predictive models:

Baseline: Predict DowJones returns using only its past returns.

Enhanced: Predict DowJones returns using past returns of both DowJones and Bitcoin.

Compared Linear Regression and Random Forest models.

Evaluated model performance using MSE and MAE.

🔍 Key Findings:
Stock indices are strongly correlated among themselves, while their correlation with cryptocurrencies is moderate to low.

Some Granger causality was observed from cryptocurrencies (especially Bitcoin) to DowJones at short lags.

Linear Regression performed best overall, and adding Bitcoin returns did not improve it.

Random Forest benefited from adding Bitcoin returns, but still underperformed compared to Linear Regression.

🛠️ Tools Used:
Python

Libraries: pandas, numpy, yfinance, statsmodels, scikit-learn, matplotlib, seaborn

This project highlights the importance of testing beyond simple correlations. Even if Granger causality suggests a relationship, it may not always translate into improved predictive performance under different modeling approaches.
