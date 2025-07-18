# ❤️ Heart Disease Prediction using Machine Learning and also testing as simple webpage

This project aims to predict the likelihood of heart disease using various machine learning models. It includes data preprocessing, training multiple models (Logistic Regression, Decision Tree, Random Forest, Neural Network), model evaluation, and interpretability using SHAP. A user-friendly web app is also deployed using Streamlit and Ngrok.

---

## 📊 Dataset

The dataset used is the **Cleveland Heart Disease dataset**, consisting of features such as:

- Age, Sex, Chest Pain Type (`cp`)
- Resting Blood Pressure (`trestbps`)
- Serum Cholesterol (`chol`)
- Fasting Blood Sugar (`fbs`)
- Max Heart Rate (`thalach`)
- ST Depression (`oldpeak`)
- Slope, CA, Thal, and more

The original `condition` column is converted to a binary `target`:
- `0`: No Heart Disease
- `1`: Heart Disease Likely

---

## 🧠 Models Trained

1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest**
4. **Neural Network (Keras)**

Each model is evaluated using:
- Accuracy
- Confusion Matrix
- Classification Report
- ROC-AUC Curve

---

## 📈 Feature Importance

- Random Forest Feature Importance via `.feature_importances_`
- SHAP values for model interpretability
  - Mean absolute SHAP values visualized using pie charts
  - SHAP summary plots help understand the most impactful features

---

## 🧪 Evaluation Results (Sample)

 Model                Accuracy 

Logistic Regression   73.3%    
Decision Tree         65.0%    
Random Forest         70.0%    
Neural Network        68.3%    

---

## 💻 Web App (Streamlit)

A live demo web app allows users to input patient data and get real-time predictions using the trained Neural Network model.

### 🔗 Access the App

> **Click here to open the app:**  
> [https://0ff97bbdd545.ngrokfree.app](https://0ff97bbdd545.ngrokfree.app)

### Features:
- Input sliders/radio for all relevant features
- Model prediction with heart disease risk
- Probability score output

---
##  Project Structure

heart_disease_prediction/
│
├── heart_cleveland_upload.csv       # Dataset
├── heart_nn_model.keras             # Trained neural network
├── scaler.save                      # Saved scaler
├── app.py                           # Streamlit web app
├── heart_disease_notebook.ipynb     # Full analysis and training notebook
└── README.md                        # This file


---


## 🚀 How to Run Locally

### 🧰 Requirements

Install required libraries:

``bash
pip install -r requirements.txt
