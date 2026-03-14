# Breast-Cancer-Drug-ADMET-ML-Solubility-Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange.svg)
![Domain](https://img.shields.io/badge/Domain-Drug%20Discovery-green.svg)
![Status](https://img.shields.io/badge/Project-Active-success.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

Machine learning models for predicting **aqueous solubility (ESOL Log S)** of breast cancer drug candidates using **ADMET descriptors**.
This repository includes **multiple regression algorithms, trained models, and performance comparisons**.

---

# 🧬 Breast Cancer Drug ADMET Solubility Prediction using Machine Learning

This repository contains **machine learning models developed to predict the aqueous solubility (ESOL Log S)** of potential **breast cancer drug candidates** using **ADMET descriptors**.

Solubility prediction is a **critical step in drug discovery** because it directly influences:

* **Absorption**
* **Distribution**
* **Drug efficacy**
* **Pharmacokinetics**

This project applies **multiple regression algorithms** and compares their **predictive performance**.

---

# 🎯 Project Objective

The primary goal of this project is to **build and evaluate machine learning models** capable of predicting **aqueous solubility of compounds** using **molecular ADMET features**.

### Objectives

* Develop predictive models for **ESOL Log S**
* Compare **multiple regression algorithms**
* Identify the **most reliable model**
* Assist **early-stage drug discovery prioritization**

---

# 📊 Dataset

The dataset contains **molecular descriptors and ADMET-related properties** used as **input features**.

### Target Variable

* **ESOL Log S**
  Represents the **logarithmic aqueous solubility of compounds**

### Preprocessing Steps

* Removed **text-based columns**

  * Compound name
  * SMILES strings
  * Chemical formulas
* Retained **numerical molecular descriptors** only
* Prepared dataset for **machine learning model training**

---

# 🤖 Machine Learning Models Used

Six regression algorithms were trained and evaluated:

* **Ridge Regression**
* **Gradient Boosting Regressor**
* **Random Forest Regressor**
* **ElasticNet Regression**
* **K-Nearest Neighbors Regressor**
* **Support Vector Regression**

These models allow comparison between:

* **Linear models**
* **Non-linear machine learning approaches**

---

# 🔬 Project Workflow

The project follows a **standard machine learning pipeline**:

1. Load and preprocess the **ADMET dataset**
2. Remove **non-numeric features**
3. Separate **input features and target variable (ESOL Log S)**
4. Split the dataset into **training and testing sets**
5. Apply **feature scaling and standardization**
6. Train **multiple regression models**
7. Evaluate models using:

   * **R² Score**
   * **RMSE**
8. Save trained models for **future predictions**

---

# 📈 Model Performance

Model performance was evaluated using:

* **Coefficient of Determination (R² Score)**
* **Root Mean Squared Error (RMSE)**

### Results

* **Ridge Regression**

  * R² Score: **0.9867**
  * RMSE: **0.1780**

* **Gradient Boosting Regressor**

  * R² Score: **0.9864**
  * RMSE: **0.1795**

* **Random Forest Regressor**

  * R² Score: **0.9757**
  * RMSE: **0.2402**

* **ElasticNet Regression**

  * R² Score: **0.9572**
  * RMSE: **0.3189**

* **K-Nearest Neighbors**

  * R² Score: **0.7723**
  * RMSE: **0.7359**

* **Support Vector Regression**

  * R² Score: **0.6570**
  * RMSE: **0.9031**

### 🏆 Best Performing Models

* **Ridge Regression**
* **Gradient Boosting**

These models demonstrated the **highest predictive accuracy**.

---

# 📁 Repository Structure

```
Breast-Cancer-Drug-ADMET-ML-Solubility-Prediction
│
├── ML_model_accuracy_predictions.ipynb
├── Six_Models_Performance_Metrics.csv
│
├── Ridge_Regression_Model.pkl
├── Gradient_Boosting_Model.pkl
├── Random_Forest_Model.pkl
├── ElasticNet_Model.pkl
├── K-Nearest_Neighbors_Model.pkl
├── Support_Vector_Regression_Model.pkl
```

### File Description

* **ML_model_accuracy_predictions.ipynb**
  Notebook containing **training, evaluation, and prediction workflow**

* **Six_Models_Performance_Metrics.csv**
  Comparison of **model performance metrics**

* **Model Files (.pkl)**
  Saved machine learning models for **future prediction**

---

# ⚙️ Technologies and Libraries

This project uses the following tools:

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Joblib**
* **Google Colab**
* **Jupyter Notebook**

---

# 🚀 How to Use the Models

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/Breast-Cancer-Drug-ADMET-ML-Solubility-Prediction.git
```

### 2️⃣ Install Dependencies

```bash
pip install pandas scikit-learn joblib numpy
```

### 3️⃣ Load a Trained Model

```python
import joblib

model = joblib.load("Ridge_Regression_Model.pkl")
```

### 4️⃣ Predict Solubility

Use the loaded model to **predict ESOL Log S** for new molecular descriptor data.

---

# 🧪 Applications

This project can be used in:

* **Drug discovery and development**
* **Early-stage screening of breast cancer drug candidates**
* **Computational ADMET prediction**
* **Bioinformatics and cheminformatics research**
* **Machine learning in pharmaceutical research**

---

# 🔮 Future Improvements

Potential enhancements for this project include:

* Incorporating **additional molecular descriptors**
* Using **molecular fingerprints**
* Applying **deep learning models**
* Performing **hyperparameter optimization**
* Developing a **web interface for real-time prediction**
* Expanding the dataset with **more compounds**

---

# 📜 License

This project is released under the **MIT License**.

You are free to:

* Use
* Modify
* Distribute

with **proper attribution**.

---

# 👨‍🔬 Author

Developed as part of a **computational drug discovery and machine learning project** focused on predicting **ADMET-related properties of breast cancer drug candidates**.
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
