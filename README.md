# ✈️ Flight Delay Prediction

Predicting flight delays using machine learning and data mining techniques.

## 📌 Overview

Flight delays cause inconvenience for travelers and financial losses for airlines. This project applies **data mining and machine learning models** to predict flight delays. The models handle both **regression** (predicting delay time) and **classification** (identifying airline categories) tasks, providing insights into delay patterns.

## 🎯 Objectives

- Analyze **key factors** affecting flight delays.
- Implement **various machine learning models** to predict delays.
- Compare **model performance** to identify the most accurate predictor.

## 📂 Dataset

- **Source:** [Flight Delay Dataset](https://figshare.com/articles/dataset/flights_csv/9820139)
- **Size:** ~105,000 cleaned records
- **Features:** 30 attributes, including:
  - Flight details (airline, origin, destination)
  - Time-based features (departure/arrival times)
  - Delay-related information (departure/arrival delays)

## 🛠️ Data Processing

- **Cleaning:** Removed irrelevant/missing data, dropping features like `DIVERTED` and `CANCELLED`.
- **Feature Engineering:** Encoded categorical variables (`AIRLINE`, `ORIGIN_AIRPORT`, `DESTINATION_AIRPORT`).
- **Normalization:** Applied `StandardScaler()` to standardize numerical features.
- **Feature Selection:** Used `SelectKBest` with ANOVA F-test to retain the 10 most relevant features.

## 📊 Exploratory Data Analysis (EDA)

- **Correlation Matrix:** Explored relationships between time-based and delay-related variables.
- **Airport Delays:** Identified top 10 airports with the most delays.
- **Flight Distribution:** Visualized flight frequency across different airlines and routes.

## 🤖 Model Implementation

| Model | Purpose | Insights |
|--------|---------|-----------|
| **Linear Regression** | Predict delay duration | Understands linear relationships between time and delays |
| **Random Forest** | Predict departure delays | Captures non-linear patterns and ranks feature importance |
| **Gradient Boosting (XGBoost)** | Regression & classification | Provides high accuracy for delay predictions |
| **Neural Networks** | Deep learning approach | Captures complex relationships but may require tuning |
| **Decision Tree Regression** | Delay prediction | Uncovers patterns but may suffer from overfitting |

## 🔧 Hyperparameter Tuning & Cross-Validation

- Used **grid search** and **cross-validation** to fine-tune models.
- Neural networks achieved **the highest accuracy**, suggesting strong pattern recognition.

## 📈 Results & Conclusion

- The **Neural Network model** performed best
- Overfitting concerns were mitigated through cross-validation and feature selection.
- Future work could focus on **real-time delay prediction** and **weather impact analysis**.


## 📌 Future Improvements

- **Incorporate weather data** for enhanced predictions.
- **Real-time predictions** using streaming services (Kafka, Spark).
- **Deploy the model** as a web-based API.

## 👥 Contributors

- **Shubham Gaur**
- **Malhar Ghogare**

## 📜 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
