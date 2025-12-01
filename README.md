# 🚜 Crop Yield Prediction — EDA + Machine Learning Pipeline  
*A complete end-to-end data cleaning, EDA, feature engineering, and regression modelling project.*

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shambhvi2006/EDA_crop-yield/blob/main/Crop_Yield_EDA_and_ML.ipynb)

---

## 📌 Project Overview  
This project explores and models agricultural crop yield data collected from farmers, containing soil composition, fertilizer usage, water sources, humidity, rainfall, and environmental factors.

The notebook performs a **full ML pipeline**:

- Data cleaning & preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature engineering  
- Encoding & scaling  
- Regression modelling  
- Deep learning (MLP neural network)  
- Model comparison using R²  

This showcases the ability to handle messy, real-world data and extract meaningful insights.

---

## 🧹 Data Cleaning & Preprocessing  
The dataset contained messy values, inconsistent categories, missing data, and malformed numeric fields.

Preprocessing steps include:

- Removing fully empty rows/columns  
- Renaming survey-style column names  
- Handling missing values using **mean/mode imputation**  
- Regex-based numeric cleaning (fixing “2.3.46”, removing text, symbols, etc.)  
- Encoding categorical variables (yes/no → 1/0)  
- One-hot encoding for “Soil_Addition”  
- MinMax scaling of numerical features  

This pipeline transforms raw agricultural data into a clean, ML-ready dataset.

---

## 📊 Exploratory Data Analysis  
Performed visual and statistical analysis to understand:

- Distribution of production values  
- Outliers using boxplots  
- Soil chemical properties  
- Water source contribution  
- Relationship between nutrients & production  

EDA helps identify feature importance and variability in crop production.

---

## 🤖 Models Trained  
Trained 12+ regression models:

- Linear Regression  
- Ridge / Lasso / ElasticNet  
- Random Forest  
- Gradient Boosting  
- Extra Trees  
- XGBoost  
- LightGBM  
- CatBoost  
- Support Vector Regression  
- Deep Learning MLP (TensorFlow/Keras)  

Evaluation metrics:

- **MSE** (Mean Squared Error)  
- **MAE** (Mean Absolute Error)  
- **R² score**  

### 🏆 Best Model  
**CatBoost Regressor** achieved the highest R² score on the cleaned dataset.

---

## 🧠 Deep Learning Model  
Built and trained a **3-layer MLP neural network** using TensorFlow:

- Dense(128, ReLU)  
- Dropout(0.3)  
- Dense(64, ReLU)  
- Dense(1)  

Evaluated using MSE, MAE, and R².

---

## 📈 Model Comparison  
A bar graph visualizes performance across all regression models based on **R² score**.

This helps determine which algorithms best handle real-world agricultural data.

---

