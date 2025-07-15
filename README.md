# SVM-PySpark
Cardiovascular disease prediction using PySpark and SVM on Kaggle health dataset.

# 🫀 Cardiovascular Disease Prediction with PySpark and SVM

This project utilizes the [Cardiovascular Disease Dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset) from Kaggle to predict whether a patient is likely to suffer from cardiovascular disease. The pipeline is built using **PySpark**, leveraging its scalability and parallelism for large-scale data processing, and a **Support Vector Machine (SVM)** classifier for prediction.

---

## 📌 Objective

To build a machine learning pipeline using PySpark for preprocessing and training an SVM model to classify cardiovascular disease risk based on patient health data.

---

## 📊 Dataset Description

The dataset consists of 70,000 records with 13 features related to medical attributes of patients. The target variable `cardio` indicates whether the patient has cardiovascular disease.

- **Features:**
  - `age` (in days)
  - `gender` (1: women, 2: men)
  - `height` (cm)
  - `weight` (kg)
  - `ap_hi` (Systolic blood pressure)
  - `ap_lo` (Diastolic blood pressure)
  - `cholesterol` (1: normal, 2: above normal, 3: well above normal)
  - `gluc` (glucose level)
  - `smoke` (0/1)
  - `alco` (alcohol intake: 0/1)
  - `active` (physical activity: 0/1)
  - `cardio` (target variable: 0 = no disease, 1 = has disease)

---

## 🛠️ Technologies Used

- Python 3
- PySpark (Spark MLlib)
- pandas, seaborn, matplotlib (for EDA)
- Jupyter Notebook

---

## 🔄 Workflow

1. **Data Loading**: Dataset loaded using Spark DataFrame.
2. **Data Cleaning**: Outliers removed; data types cast properly.
3. **Feature Engineering**: BMI and Age in years derived.
4. **Data Preprocessing**: Scaling, One-Hot Encoding (if needed), vectorization.
5. **Model Training**: Linear SVM trained with cross-validation and hyperparameter tuning.
6. **Model Evaluation**: Accuracy, Precision, Recall, F1-Score metrics calculated.

---

## 📈 Results

- Achieved competitive precision and recall using SVM on a balanced and cleaned dataset.
- Performance evaluation was done using confusion matrix and ROC-AUC.

