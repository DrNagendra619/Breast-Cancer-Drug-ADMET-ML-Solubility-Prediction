# Breast-Cancer-Drug-ADMET-ML-Solubility-Prediction
Machine learning models for predicting aqueous solubility (ESOL Log S) of breast cancer drug candidates using ADMET descriptors. Includes multiple regression algorithms, trained models, and performance comparison.
Breast Cancer Drug ADMET Solubility Prediction using Machine Learning

This repository contains machine learning models developed to predict the aqueous solubility (ESOL Log S) of potential breast cancer drug candidates using ADMET descriptors. Solubility prediction is an important step in drug discovery because it influences absorption, distribution, and overall drug efficacy. The project applies several regression algorithms and compares their predictive performance.

Project Objective

The primary goal of this project is to build and evaluate machine learning models capable of predicting the aqueous solubility of compounds using molecular ADMET features. By comparing multiple algorithms, the project identifies the most reliable model for solubility prediction, which can help prioritize compounds during early-stage drug discovery.

Dataset

The dataset used in this project consists of molecular descriptors and ADMET-related properties used as input features. The target variable for prediction is ESOL Log S, which represents the logarithmic aqueous solubility of compounds. Text-based columns such as compound name, SMILES strings, and chemical formulas are removed during preprocessing so that only numerical descriptors are used for model training.

Machine Learning Models Used

Six regression algorithms were trained and evaluated in this project:

Ridge Regression
Gradient Boosting Regressor
Random Forest Regressor
ElasticNet Regression
K-Nearest Neighbors Regressor
Support Vector Regression

These models were selected to compare both linear and non-linear machine learning approaches for predicting solubility.

Project Workflow

The workflow of this project follows a standard machine learning pipeline:

Load and preprocess the ADMET dataset

Remove non-numeric features

Separate input features and target variable (ESOL Log S)

Split the dataset into training and testing sets

Standardize features using feature scaling

Train multiple regression models

Evaluate model performance using R² score and RMSE

Save trained models for future prediction

Model Performance

The performance of each algorithm was evaluated using the coefficient of determination (R² Score) and Root Mean Squared Error (RMSE).

Ridge Regression achieved the highest performance with an R² score of 0.9867 and RMSE of 0.1780.
Gradient Boosting also performed strongly with an R² score of 0.9864 and RMSE of 0.1795.
Random Forest achieved an R² score of 0.9757 with RMSE of 0.2402.
ElasticNet achieved an R² score of 0.9572 with RMSE of 0.3189.
K-Nearest Neighbors achieved an R² score of 0.7723 with RMSE of 0.7359.
Support Vector Regression achieved an R² score of 0.6570 with RMSE of 0.9031.

Among all models, Ridge Regression and Gradient Boosting demonstrated the best predictive accuracy.

Repository Structure

ML_model_accuracy_predictions.ipynb – Notebook containing model training, evaluation, and prediction workflow
Six_Models_Performance_Metrics.csv – Performance comparison of all machine learning models
Ridge_Regression_Model.pkl – Trained Ridge Regression model
Gradient_Boosting_Model.pkl – Trained Gradient Boosting model
Random_Forest_Model.pkl – Trained Random Forest model
ElasticNet_Model.pkl – Trained ElasticNet model
K-Nearest_Neighbors_Model.pkl – Trained KNN model
Support_Vector_Regression_Model.pkl – Trained SVR model

Technologies and Libraries

Python
Pandas
NumPy
Scikit-learn
Joblib
Google Colab / Jupyter Notebook

How to Use the Models

Clone this repository to your local system.

git clone https://github.com/yourusername/Breast-Cancer-Drug-ADMET-ML-Solubility-Prediction.git

Install required dependencies.

pip install pandas scikit-learn joblib numpy

Load a saved model in Python.

import joblib
model = joblib.load("Ridge_Regression_Model.pkl")

Use the model to make predictions on new molecular descriptor data.

Applications

Drug discovery and development
Early-stage screening of breast cancer drug candidates
Computational ADMET prediction
Machine learning in bioinformatics and cheminformatics

Future Improvements

Incorporate additional molecular descriptors and fingerprints
Use deep learning models for prediction
Perform hyperparameter optimization for improved performance
Develop a web interface for real-time prediction
Expand the dataset to include more compounds

License

This project is released under the MIT License. You are free to use, modify, and distribute this project with proper attribution.

Author

Developed as part of a computational drug discovery and machine learning project focused on predicting ADMET-related properties of breast cancer drug candidates.
