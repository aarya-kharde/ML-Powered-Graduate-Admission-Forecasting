# 🎓 Graduate Admission Prediction Using Machine Learning

Predict the chances of a student getting admitted to a graduate school based on their profile using classification models like **Logistic Regression**, **Decision Tree**, and **Random Forest**.

---

## 📘 Overview

Applying to graduate programs can be expensive and time-consuming. This project helps students estimate their likelihood of admission based on their academic credentials and profile.

The model is trained on a dataset inspired by the **UCLA Graduate Dataset**, containing key features such as:

- GRE Scores (out of 340)
- TOEFL Scores (out of 120)
- University Rating (1 to 5)
- SOP Strength (1 to 5)
- LOR Strength (1 to 5)
- CGPA (out of 10)
- Research Experience (0 or 1)

---

## 🧾 Problem Statement

The goal is to build predictive models to classify students into:

- `1` → High chance of admission (`Chance of Admit > 0.80`)
- `0` → Low chance of admission (`Chance of Admit ≤ 0.80`)

---

## 🧪 Models Implemented

### ✅ Logistic Regression
- Trained with `max_iter=1000` to prevent convergence warnings
- Threshold tuning (default `0.5`, adjusted to `0.6`) to optimize precision/recall

### 🌳 Decision Tree Classifier
- GridSearchCV for hyperparameter tuning (`criterion`, `max_depth`, `min_samples_leaf`, `min_samples_split`)
- Best CV Accuracy: **~92.5%**
- Test Accuracy: **91%**

### 🌲 Random Forest Classifier
- RandomizedSearchCV for tuning (`n_estimators`, `max_depth`, `criterion`, `bootstrap`)
- Best CV Accuracy: **~93.75%**
- Test Accuracy: **95%**

---

## 🔍 Exploratory Data Analysis (EDA)

- Data shape and data types
- Descriptive statistics
- Correlation matrix using heatmaps
- Pairplot (correlogram) to explore feature relationships
- Pie chart: Distribution of University Ratings

---

## 📈 Evaluation Metrics

- Accuracy Score
- Precision, Recall, F1-score
- Confusion Matrix
- Classification Report

---

## 📊 Visualizations

- 📌 Correlation Heatmap   
- 📌 Pairplot for feature relationships  
- 📌 Pie chart for University Ratings  

---
