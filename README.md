# 🛒 Commodity Price Prediction using Ridge Regression

## 📌 Overview

This project focuses on predicting commodity prices using a multiple regression approach, specifically Ridge Regression. The dataset includes various temporal and market-based numeric features such as date, market, latitude, longitude,	category,	commodity, unit, priceflag,	pricetype and more. The model aims to capture trends and relationships within the data to estimate the price of commodities accurately.

---

## 🧠 Objectives

- Build a predictive model for commodity prices using the features.
- Explore and visualize feature correlations.
- Evaluate model performance using appropriate regression metrics.
- Optionally combine date-related features into a unified timestamp for better temporal insight.

---

## 🗂 Dataset Description

The dataset includes the following columns:

| Feature        | Description                                  |
|----------------|----------------------------------------------|
| `year`         | Year of the observation                      |
| `month`        | Month of the observation                     |
| `day`          | Day of the observation                       |
| `market_freq`  | Frequency or score of market availability    |
| `category`     | Encoded category of the commodity            |
| `commodity`    | Encoded commodity ID                         |
| `unit_numeric` | Unit measurement in numeric form             |
| `priceflag`    | Numeric flag indicator (e.g., quality, type) |
| `pricetype`    | Encoded type of price reported               |
| `price`        | Target variable — price of the commodity     |


## 🛠️ Tools & Libraries

- Python 3
- pandas
- NumPy
- scikit-learn
- matplotlib / seaborn (for correlation plots)

---

## 🔁 Workflow

1. **Data Cleaning & Preprocessing**
   - extract `year`, `month`, `day` from  date.
   - Encoding and Normalizing Data.

2. **Feature Selection**
   - Use correlation matrix to identify high-impact features on `price`.

3. **Model Training**
   - Split data into training and testing sets.
   - Use `StandardScaler` and `Ridge` in a pipeline.

4. **Evaluation**
   - Metrics: Mean Squared Error (MSE), R² Score.
