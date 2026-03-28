# 🛒 Shop Smart – Purchase Prediction using Machine Learning

## 📌 Overview

This project focuses on predicting whether a user will make a purchase based on their online shopping behavior.
It uses a **Decision Tree Classifier** combined with a **scikit-learn pipeline** to ensure a clean, reproducible, and production-oriented workflow.

The goal of this project is not just model accuracy, but to follow **best practices used in real-world machine learning systems**, such as proper data splitting, preprocessing, and avoiding data leakage.

---

## 🚀 Problem Statement

E-commerce platforms often want to identify users who are likely to make a purchase during a session.
By predicting purchase intent, businesses can:

* Improve targeted marketing
* Optimize recommendations
* Increase conversion rates

---

## 🧠 Approach

### 1. Data Preparation

* Separated features and target variable (`Revenue`)
* Automatically identified:

  * Numerical features
  * Categorical features

### 2. Train-Test Split

* Performed before preprocessing to prevent **data leakage**
* Used stratified sampling to maintain class distribution

### 3. Preprocessing (via Pipeline)

* **Numerical features** → Standard Scaling
* **Categorical features** → One-Hot Encoding
* Used `ColumnTransformer` to handle both types efficiently

### 4. Model

* Decision Tree Classifier with controlled complexity:

  * `max_depth`
  * `min_samples_leaf`
  * `class_weight="balanced"`

### 5. Pipeline Integration

* Combined preprocessing and model into a single pipeline
* Ensures:

  * Consistent transformations
  * Cleaner code
  * Easier deployment

### 6. Evaluation

* Evaluated using:

  * F1 Score
  * Classification Report
  * Confusion Matrix

### 7. Hyperparameter Tuning

* Used GridSearchCV to find optimal model parameters
* Cross-validation used for robust performance estimation

---

## ⚙️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn

---

## 📊 Key Learnings

* Importance of **splitting data before preprocessing**
* How pipelines prevent **data leakage**
* Handling mixed data types using `ColumnTransformer`
* Writing ML code that is closer to **production standards**
* Using F1-score for imbalanced classification problems

---

## 📁 Project Structure

```
shop_smart/
│
├── shop_smart.ipynb
├── README.md
```

---

## 🔮 Future Improvements

* Add Streamlit UI for real-time predictions
* Deploy as a web application
* Experiment with ensemble models (Random Forest, XGBoost)
* Add feature importance visualization

---

## 🙌 Conclusion

This project demonstrates a structured approach to building machine learning models with a focus on correctness, reproducibility, and scalability rather than just achieving high accuracy.

---
