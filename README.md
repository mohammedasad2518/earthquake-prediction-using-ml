# 🌍 Earthquake Magnitude Prediction using Machine Learning

## 📌 Project Overview

This project focuses on predicting the **magnitude of earthquakes** using Machine Learning techniques. The model is trained on historical seismic data and evaluated on real-time earthquake data to analyze its performance in practical scenarios.

---

## 🚀 Objectives

* Predict earthquake magnitude based on geographical and temporal features
* Analyze model performance on both historical and real-time datasets
* Visualize earthquake distribution across the globe
* Understand the challenges of real-world prediction

---

## 📊 Datasets Used

### 1️⃣ Kaggle Dataset (Training Data)

* Large dataset (~200,000+ records)
* Covers multiple years of earthquake data
* Includes engineered features for better prediction

### 2️⃣ USGS Dataset (Testing Data)

* Real-time earthquake data (last 30 days)
* Used to evaluate model performance in real-world conditions

---

## 🧠 Features Used

* Latitude
* Longitude
* Depth
* Year
* Month
* Day

---

## ⚙️ Technologies Used

* Python
* Pandas & NumPy
* Scikit-learn
* Matplotlib
* GeoPandas

---

## 🔧 Project Workflow

### 1. Data Collection

* Downloaded historical dataset from Kaggle
* Collected real-time data from USGS

### 2. Data Preprocessing

* Removed unnecessary columns
* Handled missing values
* Converted time into usable features (year, month, day)

### 3. Feature Engineering

* Extracted temporal features
* Converted categorical variables into numerical format

### 4. Model Training

* Used **Random Forest Regressor**
* Trained on Kaggle dataset

### 5. Model Evaluation

* Evaluated using Mean Absolute Error (MAE)

Results:

* 📊 Kaggle MAE ≈ **0.23**
* 🌍 USGS MAE ≈ **3.65**

---

## 📉 Key Insight

The model performs well on historical data but shows higher error on real-time data due to:

* Feature mismatch
* Lack of engineered features in USGS dataset
* Differences in data distribution

---

## 📊 Visualizations

* Actual vs Predicted Magnitude Graph
* Error Distribution
* Feature Importance
* Global Earthquake Map 🌍

---

## 🌍 Geospatial Visualization

Earthquake locations were plotted on a world map using GeoPandas, with color indicating predicted magnitude.

---

## ⚠️ Limitations

* Cannot predict exact future earthquakes
* Model depends heavily on feature quality
* Real-time data lacks advanced features

---

## 🔮 Future Improvements

* Add time-series models (LSTM)
* Improve feature engineering for real-time data
* Build classification model (High risk / Low risk)
* Create interactive maps

---

## 🎯 Conclusion

This project demonstrates how machine learning can be applied to seismic data for magnitude prediction. While exact earthquake prediction remains a challenge, this approach provides valuable insights into earthquake patterns and risk analysis.

---

## 📌 Author

**Mohammed Asad**
Computer Science Engineering Student

---
