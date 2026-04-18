# ICU Sepsis Risk Prediction System

A machine learning-based system designed to estimate the risk of sepsis in ICU patients using vital signs and clinical parameters. This project demonstrates how predictive models and clinical scoring systems can be combined to support early risk assessment.

---

## 🔍 Problem Statement

Sepsis is a life-threatening condition caused by the body's extreme response to infection and is a leading cause of mortality in intensive care units (ICUs).

Early detection is challenging due to:
- Complex and rapidly changing clinical parameters  
- Delayed recognition using traditional methods  
- High dependency on continuous monitoring  

This project aims to build a system that predicts sepsis risk using patient data, enabling earlier identification of high-risk cases.

---

## ⚙️ Approach

The system combines machine learning with clinical rules:

### 1. Data Handling
- Input: Vital signs and lab values (e.g., heart rate, BP, lactate)
- Preprocessing:
  - Handling missing values  
  - Feature scaling using StandardScaler  

### 2. Model Development
- Model: Neural Network (TensorFlow/Keras)
- Input Features: 9 clinical parameters
- Output: Probability score (0–1) representing sepsis risk

### 3. Clinical Integration
- SIRS criteria
- qSOFA scoring
- Rule-based fallback system

### 4. Application Layer
- Built using Streamlit
- Provides real-time input, prediction, and visualization

---

## 📊 Results

- Model trained on **simulated ICU dataset**
- Output: Sepsis risk score (0–100%)

⚠️ Note:
- This project does **not use real patient data**
- Model performance metrics (accuracy, precision, recall) are not clinically validated
- Results are for demonstration purposes only

---

## 📁 Dataset

- Type: Simulated clinical dataset  
- Purpose: To mimic ICU patient conditions for model training  
- Limitation: Does not reflect real-world medical variability  

---

## 🚀 Features

- Patient data input with validation  
- Real-time sepsis risk prediction  
- Interactive dashboard with visualizations  
- Clinical scoring (SIRS, qSOFA)  
- Alert system with risk categorization  

---

## 🧠 Machine Learning Model

- Architecture: Sequential Neural Network  
- Regularization: Dropout layers  
- Activation: Sigmoid (binary classification)  

### Features Used:
- Temperature  
- Heart Rate  
- Respiratory Rate  
- Blood Pressure (Sys/Dia)  
- WBC Count  
- Lactate  
- Age  
- Gender  

---

## 🛠️ Tech Stack

- Frontend: Streamlit  
- ML: TensorFlow / Keras  
- Data: Pandas, NumPy  
- Visualization: Plotly  

---

## ▶️ How to Run

```bash
git clone https://github.com/MrudhulaVarshaShri/ICU-Sepsis-Risk-Prediction-System
cd ICU-Sepsis-Risk-Prediction-System
pip install -r requirements.txt
streamlit run app.py
