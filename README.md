# Breast-Cancer-Drug-ADMET-ML-Solubility-Prediction

Machine learning models for predicting aqueous solubility (ESOL Log S) of breast cancer drug candidates using ADMET descriptors. Includes multiple regression algorithms, trained models, and performance comparison.

---

## Breast Cancer Drug ADMET Solubility Prediction using Machine Learning

This repository contains machine learning models developed to predict the aqueous solubility (ESOL Log S) of potential breast cancer drug candidates using ADMET descriptors. Solubility prediction is an important step in drug discovery because it influences absorption, distribution, and overall drug efficacy. The project applies several regression algorithms and compares their predictive performance.

---

## Project Objective

The primary goal of this project is to build and evaluate machine learning models capable of predicting the aqueous solubility of compounds using molecular ADMET features.

By comparing multiple algorithms, the project identifies the most reliable model for solubility prediction, which can help prioritize compounds during early-stage drug discovery.

---

## Dataset

The dataset used in this project consists of molecular descriptors and ADMET-related properties used as input features.

The target variable for prediction is **ESOL Log S**, which represents the logarithmic aqueous solubility of compounds.

During preprocessing:

- Text-based columns such as compound name
- SMILES strings
- Chemical formulas

were removed so that only **numerical descriptors** are used for model training.

---

## Machine Learning Models Used

Six regression algorithms were trained and evaluated in this project:

- Ridge Regression  
- Gradient Boosting Regressor  
- Random Forest Regressor  
- ElasticNet Regression  
- K-Nearest Neighbors Regressor  
- Support Vector Regression  

These models were selected to compare both **linear and non-linear machine learning approaches** for predicting solubility.

---

## Project Workflow

The workflow of this project follows a standard machine learning pipeline:

1. Load and preprocess the ADMET dataset  
2. Remove non-numeric features  
3. Separate input features and target variable (ESOL Log S)  
4. Split the dataset into training and testing sets  
5. Standardize features using feature scaling  
6. Train multiple regression models  
7. Evaluate model performance using R² score and RMSE  
8. Save trained models for future prediction  

---

## Model Performance

The performance of each algorithm was evaluated using:

- **Coefficient of Determination (R² Score)**
- **Root Mean Squared Error (RMSE)**

### Results

**Ridge Regression**
- R² Score: **0.9867**
- RMSE: **0.1780**

**Gradient Boosting Regressor**
- R² Score: **0.9864**
- RMSE: **0.1795**

**Random Forest Regressor**
- R² Score: **0.9757**
- RMSE: **0.2402**

**ElasticNet Regression**
- R² Score: **0.9572**
- RMSE: **0.3189**

**K-Nearest Neighbors Regressor**
- R² Score: **0.7723**
- RMSE: **0.7359**

**Support Vector Regression**
- R² Score: **0.6570**
- RMSE: **0.9031**

Among all models, **Ridge Regression** and **Gradient Boosting** demonstrated the best predictive accuracy.

---

## Repository Structure

ML_model_accuracy_predictions.ipynb  
Notebook containing model training, evaluation, and prediction workflow

Six_Models_Performance_Metrics.csv  
Performance comparison of all machine learning models

Ridge_Regression_Model.pkl  
Trained Ridge Regression model

Gradient_Boosting_Model.pkl  
Trained Gradient Boosting model

Random_Forest_Model.pkl  
Trained Random Forest model

ElasticNet_Model.pkl  
Trained ElasticNet model

K-Nearest_Neighbors_Model.pkl  
Trained KNN model

Support_Vector_Regression_Model.pkl  
Trained SVR model

---

## Technologies and Libraries

Python  
Pandas  
NumPy  
Scikit-learn  
Joblib  
Google Colab / Jupyter Notebook  

---

## How to Use the Models

Clone this repository to your local system:
