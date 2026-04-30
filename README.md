# 🧠 Diabetes Prediction using Machine Learning

## 📌 Overview
This project builds a machine learning model to predict whether a person has diabetes based on medical and demographic features.

The dataset is **highly imbalanced**, making this a realistic healthcare problem where detecting diabetic patients is critical.

---

## 🎯 Objective
- Predict diabetes (1) vs no diabetes (0)
- Handle class imbalance effectively
- Compare multiple ML models
- Improve model performance
- Extract meaningful insights

---

## 📊 Dataset Features
- **gender**
- **age**
- **hypertension**
- **heart_disease**
- **smoking_history**
- **bmi**
- **HbA1c_level**
- **blood_glucose_level**
- **diabetes (target)**

---

## ⚠️ Challenge: Imbalanced Dataset
- 0 (No Diabetes): ~91%
- 1 (Diabetes): ~9%

Handled using:
- Class weights
- SMOTE
- Threshold tuning

---

## 🔧 Workflow

### 1. Data Exploration
- Checked missing values, duplicates
- Analyzed distributions
- Identified key features

---

### 2. Data Preprocessing
- Removed invalid values (e.g., "Other" in gender)
- Handled "No Info"
- One-hot encoding
- Stratified train-test split
- Standardization

---

### 3. Feature Engineering
- Created new features (BMI categories, risk levels)
- Feature importance analysis

---

### 4. Model Building
Models used:
- Logistic Regression
- Decision Tree
- Random Forest

Metrics:
- Precision
- Recall
- F1-score
- ROC-AUC

---

### 5. Model Improvement
- SMOTE for imbalance
- Hyperparameter tuning
- Threshold tuning

---

## 📊 Model Performance

| Model               | Precision | Recall | F1-score |
|--------------------|----------|--------|----------|
| Logistic Regression | 0.42     | 0.88   | 0.57     |
| Decision Tree       | 0.68     | 0.73   | 0.70     |
| Random Forest       | Best overall |

---

## 🧠 Key Insights
- HbA1c and blood glucose are strongest predictors
- High recall ensures most diabetic cases are detected
- Some false positives exist (acceptable in healthcare)

---

## 🚀 Future Improvements
- Use XGBoost / LightGBM
- Cross-validation
- Deploy as web app
- Add more real-world features

---

## 🛠️ Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn
- Plotly

---

## 👨‍💻 Author
Kishore Kannan

---

## ⭐ Support
If you like this project, give it a star ⭐
