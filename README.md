# ❤️ Heart Disease Risk Prediction Using Machine Learning  
### A Data-Driven Approach for Early Diagnosis and Prevention
## 📌 Project Overview

This project leverages advanced machine learning techniques to predict the **risk of heart disease** based on multiple physiological and lifestyle indicators. With heart disease being a leading cause of death globally, early diagnosis and prevention are essential. By building robust classification models, this project aims to empower healthcare professionals and individuals with data-driven insights to take timely preventive measures.

---
## 🧠 Dataset Description

The dataset consists of **70,000 patient records** with the following features:

- **Symptoms**: Chest Pain, Shortness of Breath, Fatigue, Palpitations, Dizziness, Swelling, Pain in Arms/Jaw/Back, Cold Sweats/Nausea  
- **Medical Conditions**: High Blood Pressure, High Cholesterol, Diabetes  
- **Lifestyle**: Smoking, Obesity, Sedentary Lifestyle, Chronic Stress  
- **Demographics**: Gender, Age  
- **Target Variable**: `Heart_Risk` (1 = At Risk, 0 = Not at Risk)

---
## 🔍 Exploratory Data Analysis (EDA)

- 📊 Correlation analysis identified strong positive associations between chronic conditions (e.g., High_BP, High_Cholesterol) and heart risk.
- 🧩 Age and Sedentary_Lifestyle also showed significant impact.
- 📌 Balanced distribution of the target class allowed fair modeling.

All EDA was accompanied by professional visualizations (heatmaps, countplots, KDE plots, and boxplots) to gain in-depth insight into patterns.

---
## ⚙️ Data Preprocessing

- Checked for nulls and cleaned data
- Applied feature scaling using `StandardScaler`
- No categorical encoding was needed as all features were numeric
- Split data into training (80%) and testing (20%)

---

## 🤖 Machine Learning Models

We trained and fine-tuned **three classification models** using GridSearchCV with 5-fold cross-validation:

### 🔹 Logistic Regression
- Tuned hyperparameters: `C`, `penalty`, `solver`
- 📊 **Accuracy**: `0.9909`

### 🔹 Random Forest Classifier
- Tuned hyperparameters: `n_estimators`, `max_depth`, `min_samples_split`
- 📊 **Accuracy**: `0.9920`

### 🔹 XGBoost Classifier
- Tuned hyperparameters: `n_estimators`, `max_depth`, `learning_rate`, `subsample`
- 📊 **Accuracy**: `0.9930`

---

## 📊 Model Performance & Evaluation

### ✅ Logistic Regression:
```
Precision: 0.99 | Recall: 0.99 | F1-Score: 0.99  
Test Accuracy: 0.9909
```

### ✅ Random Forest:
```
Precision: 0.99 | Recall: 0.99 | F1-Score: 0.99  
Test Accuracy: 0.9920
```

### ✅ XGBoost:
```
Precision: 0.99 | Recall: 0.99 | F1-Score: 0.99  
Test Accuracy: 0.9930
```

### 📉 Overfitting Check:
- Plotted Actual vs Predicted distributions
- Confusion matrices showed minimal false positives/negatives
- Accuracy gap between Train and Test was negligible — no overfitting detected

---

## 💼 Business Impact

- 🏥 **Clinical Use**: Doctors can use this predictive model as a triage tool to identify high-risk individuals early, leading to timely diagnostics and preventive treatment.
- 💸 **Healthcare Cost Reduction**: Preventing heart attacks through early intervention can drastically reduce emergency and surgical healthcare costs.
- 📲 **Personal Health Apps**: Can be integrated into wearable device ecosystems to alert users about potential cardiac risks in real-time.
- 🌍 **Scalability**: The model performs well with minimal features, making it scalable for large public health applications and rural telemedicine deployments.



