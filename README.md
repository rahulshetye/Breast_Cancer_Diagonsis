
---

# 🩺 Breast Cancer Diagnosis – Supervised Classification Pipeline

## 📌 Objective

Build a supervised machine learning model to classify breast tumors as **Malignant (M)** or **Benign (B)** while demonstrating the **complete machine learning workflow**, including:

* Problem framing
* Data preparation
* Model training
* Evaluation
* Generalization error analysis

---

## 📂 Dataset

**Breast Cancer Wisconsin (Diagnostic) Dataset**
🔗 [https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)

### Dataset Details

* **Instances:** 569
* **Features:** 30 numeric features computed from digitized images of breast mass
* **Target Label:**

  * `M` → Malignant
  * `B` → Benign

---

## 🧠 Problem Framing

This is a **binary classification problem** where the goal is to predict whether a tumor is malignant or benign based on extracted features.
Since this is a medical diagnosis task, **generalization performance** and **recall** are especially important to minimize false negatives.

---

## ⚙️ Workflow Overview

### 1️⃣ Data Preparation

* Load dataset (`data.csv`)
* Drop non-informative ID column
* Encode target labels (`M = 1`, `B = 0`)
* Split data into **training and testing sets**
* Apply **feature standardization** (required for Logistic Regression)

---

### 2️⃣ Model Training

Two models are trained and compared:

| Model               | Description                     |
| ------------------- | ------------------------------- |
| Logistic Regression | Baseline linear classifier      |
| Decision Tree       | Non-linear, high-capacity model |

---

### 3️⃣ Model Evaluation

Each model is evaluated using:

* **Training Error**
* **Test Error**
* **Generalization Gap**
* **Accuracy**
* **Precision**
* **Recall**
* **F1-score**
* **Confusion Matrix**

---


## 📉 Generalization Error Analysis

* **Logistic Regression** shows a small gap between training and test error, indicating **good generalization**.
* **Decision Tree** achieves very low training error but higher test error, indicating **overfitting due to high variance**.
* This highlights the **bias–variance tradeoff** and the importance of controlling model complexity.

---

## ⚠️ Overfitting & Underfitting Discussion

* **Decision Tree:**

  * Low training error
  * Significantly higher test error
  * Exhibits **overfitting**

* **Logistic Regression:**

  * Slightly higher bias
  * Lower variance
  * More stable and reliable for deployment

---

## 🧩 Machine Learning Issues Addressed

* Feature scaling for gradient-based models
* Class imbalance considerations
* Feature correlation
* Risk of data leakage during preprocessing
* Bias–variance tradeoff

---
## 📘 NoteBook Link
🔗https://colab.research.google.com/drive/1toag12ASyX_Ucvlv_mZgAfcB3n-qeIPs?usp=sharing
---

## ✅ Conclusion

Although both models perform well on training data, **Logistic Regression generalizes better** and exhibits a smaller generalization gap. The Decision Tree, while more expressive, overfits the training data and performs worse on unseen data. For medical diagnosis tasks where robustness and interpretability are critical, simpler models with controlled variance are often preferable.

---

## 📌 Author

**Rahul Shetye**

---

