# Diabetes Risk Prediction


---

## 📁 Project Structure

```
CodeClause_internship_heart_disease_risk_prediction/
│
├── dataset/
│   └── diabetes_dataset_enhanced.csv                             # feature engineered dataset
│   └── diabetes_dataset.csv                                      # original dataset
│
├── model/
│   └── xgboost_diabetes_model.pkl                                # Trained model pipeline
│
├── notebooks/
│   ├── EDA.ipynb                                                 # EDA and feature importance
│   ├── model_dev.ipynb                                           # Model development on original dataset
│   └── model_dev.ipynb                                           # Model development on feature engineered dataset
│
│
├── README.md                                                     # Project overview
└── requirements.txt                                              # Required libraries
```

---

## 🧠 Problem Statement

Problem Statement: Diabetes is a growing global health concern, often going undiagnosed until severe complications arise. This app helps users assess their diabetes risk early using basic health inputs, enabling proactive lifestyle changes and timely medical consultation—reducing long-term health and economic impacts.
---

## 📊 Dataset Overview

- **Source:** [Kaggle – Diabetes Health Indicators Dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)
- **Rows:** 253,000+
- **Target Variable:** `diabetes` (0 = No, 1 = Yes)
- **Key Features:** BMI, blood pressure, smoking status, glucose level, physical activity, age, etc.


## ✅ Project Workflow (v1)

1. **EDA**
   - Analyzed class imbalance - slightly imablanced normal in real datasets
   - Visualized distributions and correlations (used heatmap but not present in the current repo)
   - Identified key influencing features

2. **Preprocessing**
   - No missing values found
   - Standardized data using `StandardScaler`

3. **Model Pipeline**
   - Feature selection with `SelectKBest`
   - Used `XGBClassifier` for prediction
   - Hyperparameter tuning with `GridSearchCV`

4. **Evaluation**
   - Achieved ~86% accuracy
   - Good balance between precision and recall
   - Evaluated using confusion matrix & classification report

5. **Feature Importance**
   - Visualized top contributing features using XGBoost’s importance scores

6. **Deployment**
   - Simple and interactive UI built using `Streamlit`
   - Predicts and displays diabetes risk with probability

---

## 📦 Requirements

```
matplotlib
ucimlrepo
pandas
scikit-learn
xgboost
numpy
joblib
```

Install with:

```bash
pip install -r requirements.txt
```

## 📌 Note

This repository is not intended for full workflow simulation but rather to understand the workflow used to build the model.

The model is now deployed as a working app built using **Streamlit** and is currently live.

- 🔗 **App Repository:** [https://github.com/insanjay/diabetes_prediction](https://github.com/insanjay/diabetes_prediction)
- 🚀 **Live App:** [https://heartsafe.streamlit.app/](https://heartsafe.streamlit.app/)

## 👨‍💻 Author

- **Sanjay Kumar**
- [GitHub](https://github.com/insanjay)
- [LinkedIn](https://www.linkedin.com/in/insanjay)

