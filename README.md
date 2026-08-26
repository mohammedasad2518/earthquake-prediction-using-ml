<div align="center">

# 🌍 Earthquake Magnitude Prediction Using Machine Learning

### Predicting Earthquake Magnitude from Historical Seismic Data and Evaluating the Model on Recent USGS Data

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-FF9800?style=for-the-badge)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![GeoPandas](https://img.shields.io/badge/GeoPandas-139C5A?style=for-the-badge)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

</div>

---

## 📖 About

**Earthquake Magnitude Prediction Using Machine Learning** is a machine learning project focused on predicting earthquake magnitude using historical seismic and geographical data.

The project uses a **Random Forest Regressor** trained on historical earthquake data and evaluates the model using recent earthquake observations obtained from the **United States Geological Survey (USGS)**.

It also includes data preprocessing, feature engineering, model evaluation, and geospatial visualization to analyze earthquake activity across different regions.

> ⚠️ **Disclaimer:** This project is intended for educational, experimental, and data-analysis purposes. It is not an operational earthquake early-warning or earthquake prediction system.

---

## 🎯 Objectives

- Predict earthquake magnitude using Machine Learning
- Analyze historical earthquake data
- Perform data preprocessing and feature engineering
- Train a Random Forest regression model
- Evaluate model performance
- Test the trained model against recent USGS data
- Compare performance across different datasets
- Visualize earthquake activity geographically
- Understand real-world Machine Learning generalization

---

## 🌋 Problem Statement

Earthquake prediction is a highly complex problem because seismic events are influenced by numerous geological factors.

Instead of attempting to predict the exact time and location of future earthquakes, this project focuses on a specific Machine Learning problem:

**Predict the magnitude of an earthquake using available geographical and temporal features.**

The project also evaluates how a model trained on historical data performs when applied to newer real-world observations.

---

## 📊 Datasets

### 📚 Historical Earthquake Dataset

Historical earthquake data is used to train the Machine Learning model.

The dataset contains information such as:

- Earthquake magnitude
- Latitude
- Longitude
- Depth
- Date and time
- Other seismic attributes

### 🌍 USGS Dataset

Recent earthquake data from the **United States Geological Survey (USGS)** is used to evaluate the trained model.

The project uses recent earthquake observations covering approximately the last 30 days.

This provides an opportunity to examine how well a model trained on historical data generalizes to newer observations.

---

## 🧩 Features Used

| Feature | Description |
|---|---|
| **Latitude** | Geographic latitude of the earthquake |
| **Longitude** | Geographic longitude of the earthquake |
| **Depth** | Depth of the earthquake below the surface |
| **Year** | Year of occurrence |
| **Month** | Month of occurrence |
| **Day** | Day of occurrence |

---

## 🧹 Data Preprocessing

The preprocessing workflow includes:

- Loading earthquake datasets
- Removing unnecessary columns
- Handling missing values
- Cleaning raw data
- Converting timestamps
- Extracting year, month, and day
- Preparing input features
- Preparing target values
- Aligning relevant features between datasets

---

## 🧠 Feature Engineering

Timestamp information is transformed into useful numerical features.

<pre>
Timestamp
    │
    ├── Year
    ├── Month
    └── Day
</pre>

These temporal features are combined with geographical information such as latitude, longitude, and depth.

---

## 🌲 Machine Learning Model

### Random Forest Regressor

The project uses a **Random Forest Regressor** to predict earthquake magnitude.

Random Forest is an ensemble learning algorithm that combines multiple decision trees to generate a final prediction.

The model learns relationships between the input features and earthquake magnitude from historical observations.

---

## 🔄 Machine Learning Workflow

<pre>
                Historical Data
                       │
                       ▼
              Data Preprocessing
                       │
                       ▼
              Feature Engineering
                       │
                       ▼
                Train/Test Split
                       │
                       ▼
              Random Forest
                 Regressor
                       │
                       ▼
                Model Training
                       │
                       ▼
             Magnitude Prediction
                       │
              ┌────────┴────────┐
              ▼                 ▼
       Historical Test     Recent USGS
           Dataset             Data
              │                 │
              └────────┬────────┘
                       ▼
                Model Evaluation
                       │
                       ▼
              Geospatial Analysis
</pre>

---

## 🏋️ Model Training

The Random Forest Regressor is trained using historical earthquake observations.

<pre>
Historical Dataset
        ↓
Data Preprocessing
        ↓
Feature Engineering
        ↓
Feature Selection
        ↓
Train/Test Split
        ↓
Random Forest Training
        ↓
Trained Model
</pre>

---

## 📏 Model Evaluation

The primary evaluation metric used in this project is **Mean Absolute Error (MAE)**.

MAE measures the average absolute difference between the actual earthquake magnitude and the predicted magnitude.

### Model Results

| Dataset | Mean Absolute Error |
|---|---:|
| 📚 Historical Kaggle Data | **≈ 0.23** |
| 🌍 Recent USGS Data | **≈ 3.65** |

The model performs considerably better on the historical dataset than on the recent USGS dataset.

---

## 📉 Important Observation

The difference in performance demonstrates an important Machine Learning challenge known as **distribution shift**.

A model may perform well on data that resembles its training data but perform differently when exposed to a new dataset with different characteristics.

Possible factors include:

- Differences in feature distributions
- Dataset structure differences
- Differences in data collection
- Missing engineered features
- Temporal differences
- Differences between training and real-world data

This makes the project useful not only as an earthquake magnitude prediction experiment, but also as a demonstration of **real-world model evaluation and generalization**.

---

## 🌍 Geospatial Visualization

The project uses **GeoPandas** and visualization libraries to analyze earthquake activity geographically.

The visualization can be used to explore:

- 🌍 Global earthquake distribution
- 📍 Earthquake locations
- 📊 Magnitude information
- 🗺️ Geographic patterns
- 🌋 Regional seismic activity

---

## 📊 Visualizations

The project includes visual analysis such as:

### 📈 Actual vs Predicted Magnitude

Compares actual earthquake magnitudes with the magnitudes predicted by the Machine Learning model.

### 📉 Prediction Error

Shows the difference between actual and predicted earthquake magnitudes.

### 🌲 Feature Importance

Helps identify which input features contribute most to the Random Forest model's predictions.

### 🌍 Global Earthquake Map

Displays earthquake locations geographically and provides a visual representation of earthquake magnitude.

---

## 🛠️ Technologies Used

### Programming

- Python

### Machine Learning

- Scikit-Learn
- Random Forest Regression

### Data Processing

- Pandas
- NumPy

### Visualization

- Matplotlib

### Geospatial Analysis

- GeoPandas

### Development

- Jupyter Notebook
- VS Code
- Git
- GitHub

---

## 📂 Repository Structure

<pre>
earthquake-prediction-using-ml/
│
├── Earthquake Prediction Model.ipynb
├── all_month.csv
├── stage_4_earthquake_dataset.csv
├── README.md
└── LICENSE
</pre>

---

## 🚀 Getting Started

### 1. Clone the Repository

<pre>
git clone https://github.com/mohammedasad2518/earthquake-prediction-using-ml.git
</pre>

### 2. Navigate to the Project

<pre>
cd earthquake-prediction-using-ml
</pre>

### 3. Install Dependencies

<pre>
pip install pandas numpy scikit-learn matplotlib geopandas jupyter
</pre>

### 4. Launch Jupyter Notebook

<pre>
jupyter notebook
</pre>

Open **Earthquake Prediction Model.ipynb** and run the notebook cells sequentially.

---

## 🧪 Experiments

The project can be extended by experimenting with:

- Random Forest hyperparameters
- Different regression algorithms
- Additional seismic features
- Improved feature engineering
- Different train/test splits
- Cross-validation
- Time-series approaches
- Alternative Machine Learning models
- Advanced geospatial analysis

---


## 🔮 Future Improvements

Potential future enhancements include:

- 🧠 Experiment with LSTM and other time-series models
- 🌍 Improve real-time USGS data integration
- 📊 Add additional seismic features
- 🎯 Develop earthquake risk classification
- 🗺️ Build interactive earthquake maps
- 📈 Create a real-time earthquake monitoring dashboard
- 🔄 Implement automated model retraining
- 🧪 Compare multiple Machine Learning algorithms
- ⚙️ Perform advanced hyperparameter optimization
- 🚀 Deploy the model as a web application
- 📡 Integrate continuous seismic data streams

---

## 🎓 Learning Outcomes

Through this project, I gained practical experience with:

- Machine Learning regression
- Random Forest Regression
- Data preprocessing
- Feature engineering
- Model evaluation
- Mean Absolute Error
- Real-world dataset comparison
- Distribution shift
- Geospatial data analysis
- Data visualization
- Jupyter Notebook workflows
- Applying Machine Learning to seismic datasets

---

## 🌟 Project Highlights

- 🌍 Earthquake magnitude prediction
- 🌲 Random Forest Regression
- 📚 Historical earthquake dataset
- 📡 Recent USGS data evaluation
- 🧹 Data preprocessing
- 🧩 Feature engineering
- 📏 MAE-based evaluation
- 🗺️ Global geospatial visualization
- 📊 Model performance analysis
- 🔬 Real-world ML generalization analysis

---


<div align="center">

### 🌍 Data → Machine Learning → Prediction → Insight

**Exploring how Machine Learning can be applied to real-world seismic data.**

</div>
