# 💳 Credit Card Fraud Detection using Machine Learning

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using machine learning techniques. Fraud detection is a critical problem in the financial industry due to the highly imbalanced nature of transaction data, where fraudulent transactions represent a very small fraction of the total dataset.
The goal of this project is to build and evaluate machine learning models that can accurately identify fraudulent transactions while minimizing false positives.

---

## 🎯 Objectives

- Analyze and understand transaction data
- Handle highly imbalanced datasets
- Build baseline and advanced classification models
- Evaluate models using appropriate metrics
- Compare model performance from a business perspective

---

## 📊 Dataset

- Source: Credit Card Fraud Dataset
- Total transactions: 284,807
- Fraudulent transactions: 492 (~0.17%)
- Features: 30 anonymized features (V1–V28), Time, Amount
- Target variable:
  - `0` → Normal Transaction
  - `1` → Fraudulent Transaction

- NOTE : Due to GitHub size limitations, the dataset is hosted externally.
Download here : https://drive.google.com/file/d/1LQaHcbCQnxAN6CrIJrhylNQrXQ54SoD5/view?usp=sharing

---

## ⚙️ Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## 🧠 Methodology

### 1. Data Preprocessing
- Loaded dataset and explored structure
- Separated fraud and valid transactions
- Analyzed class imbalance

---

### 2. Exploratory Data Analysis (EDA)
- Analyzed fraud vs normal transaction ratio
- Studied transaction amount distributions
- Visualized class imbalance using count plots

---

### 3. Model Building

#### 🔹 Logistic Regression (Baseline Model)
- Used `class_weight='balanced'` to handle imbalance
- Provided interpretable baseline performance

#### 🔹 Random Forest (Advanced Model)
- Ensemble learning method for better performance
- Captures non-linear relationships

---

### 4. Hyperparameter Tuning
- Used **RandomizedSearchCV**
- Tuned parameters like:
  - Number of estimators
  - Max depth
  - Min samples split

---

### 5. Model Evaluation

Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Matthews Correlation Coefficient (MCC)

Confusion matrices and ROC curves were used for visualization.

---

## 📈 Results

| Model                | Precision | Recall | F1 Score | ROC-AUC |
|---------------------|----------|--------|----------|---------|
| Logistic Regression | High     | Good   | Good     | 0.97    |
| Random Forest       | Higher   | Better | Better   | 0.95    |

👉 Random Forest achieved better recall, making it more effective for fraud detection.

---

## 💡 Key Insights

- The dataset is highly imbalanced (~0.17% fraud cases)
- Recall is the most critical metric in fraud detection
- Random Forest performs better in identifying fraudulent transactions
- Ensemble models outperform linear models in complex datasets

---

## 📌 Conclusion

This project demonstrates the application of machine learning in fraud detection using real-world imbalanced data. By comparing baseline and advanced models, we identified that Random Forest provides better performance, especially in detecting fraudulent transactions.

---
