---

CropTrendX: Agricultural Commodity Price Forecasting

A multivariate machine learning system for predicting agricultural commodity prices using Random Forest, XGBoost, and LSTM.

Overview

CropTrendX is a predictive analytics system designed to forecast short-term price movements of agricultural commodities such as pulses and vegetables. The model integrates real-time market factors, multi-state datasets, and advanced machine learning techniques to support decision-making for farmers, traders, cold storage owners, and policymakers.

Price volatility in agriculture often arises from unstable supply–demand patterns, inflation effects, fuel price changes, and regional stock variations. CropTrendX addresses these challenges by using both statistical and deep learning models that capture linear trends, non-linear behavior, and long-term temporal dependencies.


---

Key Features

Multivariate Time-Series Forecasting targeting modal price trends.

Hybrid Modeling: Random Forest, XGBoost, and LSTM for comprehensive linear, non-linear, and sequential pattern learning.

Real-Time Factors: Incorporates inflation, fuel prices, supply metrics, and demand–supply indicators.

Regional Adaptability: Dataset aggregated from multiple Indian states for region-specific forecasting.

Feature Engineering: Categorical embeddings, seasonal sin–cos transforms, and lag-based variables.

Decision-Support System: Provides actionable insights for market stability and risk reduction.



---

Dataset

Source: data.gov.in

Time Range: January 2022 to Present

States Covered: West Bengal, Jharkhand, Bihar, Assam, Meghalaya, Odisha, and others

Key Attributes:

Categorical: state, district, market, variety

Numerical: min price, max price, modal price

Engineered: lag features (1-day, 10-day), seasonal encodings (sin/cos of month)


Primary Target Variable: Modal Price



---

Model Pipeline

1. Data Preprocessing

Label Encoding and Binary Encoding for categorical fields

Min-Max scaling for numerical fields

Lag creation for time-dependent modeling

Seasonal feature extraction using sin–cos transforms

Sequence generation for LSTM inputs



2. Models Used

Random Forest for linear + non-linear baseline modeling

XGBoost for boosted non-linear learning

LSTM for deep temporal sequence prediction



3. Evaluation Metrics

MAE (Mean Absolute Error)

RMSE (Root Mean Square Error)

MAPE (Mean Absolute Percentage Error)





---

Experimental Results

LSTM outperformed all models, providing the lowest MAE, RMSE, and MAPE across commodities.

XGBoost performed better than Random Forest but remained less accurate than LSTM.

The results demonstrate that deep learning handles temporal agricultural price data more effectively than traditional ensemble models.



---

Use Cases

Farmers: Plan crop sales and storage decisions.

Cold Storage Owners: Optimize release of stock based on predicted price movements.

Traders & Suppliers: Reduce risk by anticipating short-term price volatility.

Policymakers: Improve market regulation and inflation control.


---

Future Enhancements

Integration with live price APIs

Inclusion of weather and satellite data

Deployment as a web dashboard (Flask/React)

Support for additional crops and markets



---

Contributors

Research Team, Institute of Engineering & Management (IEM)

Project mentors and faculty collaborators



---
