# 🌾 CropTrendX: Agricultural Commodity Price Forecasting

CropTrendX is a multivariate machine learning system for forecasting short-term agricultural commodity prices using Random Forest, XGBoost, and LSTM models. The system focuses on predicting modal prices of agricultural commodities such as pulses and vegetables by integrating regional market data and real-world economic factors.

---

## 📌 Overview

Agricultural commodity prices are highly volatile due to unstable supply–demand patterns, inflation, fuel price fluctuations, and regional stock variations. CropTrendX addresses these challenges through a hybrid predictive framework combining statistical learning and deep learning models to capture:

- Linear price trends  
- Non-linear market behavior  
- Long-term temporal dependencies  

The system acts as a decision-support tool for farmers, traders, cold storage owners, and policymakers.

---

## 🚀 Key Features

- **Multivariate Time-Series Forecasting**  
  Predicts modal price trends using historical and engineered features.

- **Hybrid Modeling Framework**  
  - Random Forest for baseline linear and non-linear learning  
  - XGBoost for boosted non-linear modeling  
  - LSTM for deep sequential temporal prediction  

- **Real-Time Economic Factors**  
  Incorporates inflation indicators, fuel prices, and supply–demand metrics.

- **Regional Adaptability**  
  Uses multi-state datasets to enable region-specific forecasting.

- **Advanced Feature Engineering**  
  - Categorical embeddings  
  - Seasonal sin–cos transformations  
  - Lag-based time features  

- **Decision-Support System**  
  Provides actionable insights to reduce risk and stabilize markets.

---

## 📊 Dataset

- **Source:** data.gov.in  
- **Time Range:** January 2022 – Present  
- **States Covered:**  
  West Bengal, Jharkhand, Bihar, Assam, Meghalaya, Odisha, and others  

### Key Attributes

**Categorical Features**
- State  
- District  
- Market  
- Variety  

**Numerical Features**
- Minimum Price  
- Maximum Price  
- Modal Price  

**Engineered Features**
- Lag features (1-day, 10-day)  
- Seasonal encodings (sin/cos of month)  

**Target Variable:** Modal Price

---

## 🧠 Model Pipeline

### 1️⃣ Data Preprocessing

- Label Encoding and Binary Encoding for categorical variables  
- Min-Max scaling for numerical features  
- Lag feature generation for time-series dependency  
- Seasonal feature extraction using sin–cos transforms  
- Sequence generation for LSTM inputs  

### 2️⃣ Models Used

- **Random Forest:** Baseline regression with non-linear capability  
- **XGBoost:** Gradient-boosted tree-based regression model  
- **LSTM:** Deep learning model for temporal sequence forecasting  

### 3️⃣ Evaluation Metrics

- MAE (Mean Absolute Error)  
- RMSE (Root Mean Square Error)  
- MAPE (Mean Absolute Percentage Error)  

---

## 📈 Experimental Results

- LSTM achieved the lowest MAE, RMSE, and MAPE across all commodities.  
- XGBoost performed better than Random Forest but was less accurate than LSTM.  
- Results demonstrate that deep learning models handle agricultural time-series data more effectively than traditional ensemble models.

---

## 🧑‍🌾 Use Cases

- **Farmers:** Plan crop sales and storage decisions  
- **Cold Storage Owners:** Optimize stock release timing  
- **Traders & Suppliers:** Anticipate short-term price volatility  
- **Policymakers:** Support market regulation and inflation control  

---

## 🔮 Future Enhancements

- Integration with live market price APIs  
- Inclusion of weather and satellite data  
- Deployment as a web dashboard using Flask and React  
- Support for additional crops and markets  

---

## 👥 Contributors

- Research Team, Institute of Engineering & Management (IEM)  
- Project mentors and faculty collaborators  
