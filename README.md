# 🛡 Fraud Detection Using Random Forest

This project focuses on detecting *fraudulent ATM transactions* using a *Random Forest Classifier. The dataset, provided by an Australian bank, contains behavioral and risk-based features. A major challenge is the **severe class imbalance*, as fraudulent transactions are extremely rare.

---

## 📁 Project Structure


---

## 🎯 Objective

- Predict fraudulent transactions using Random Forest.
- Improve detection of rare fraud cases through SMOTE oversampling.
- Evaluate the model using appropriate metrics (not just accuracy).

---

## 🧪 Workflow Overview

### 🔹 Data Preprocessing
- Null value checks
- Label encoding of categorical variables
- Scaling if needed

### 🔹 Class Imbalance Handling
- Used *SMOTE* to oversample the minority class (fraud cases)

### 🔹 Model Used
- *Random Forest Classifier*
  - Handled high-dimensional data
  - Captured non-linear relationships
  - Provided feature importance

### 🔹 Evaluation Metrics
- Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix
- ROC AUC Score

---

## 📈 Results

### 🔹 Training Set Performance

| Metric         | Score  |
|----------------|--------|
| Accuracy       | 1.00   |
| Precision      | 1.00   |
| Recall         | 1.00   |
| F1-Score       | 1.00   |

- Support (0.0 / Genuine): 181,961
- Support (1.0 / Fraud): 315

### 🔹 Test Set Performance

| Metric               | Score  |
|----------------------|--------|
| Accuracy             | 1.00   |
| Precision (Fraud)    | 0.95   |
| Recall (Fraud)       | 0.72   |
| F1-Score (Fraud)     | 0.82   |
| ROC AUC (Macro Avg)  | 0.91   |

- Support (0.0 / Genuine): 45,490
- Support (1.0 / Fraud): 79

📝 *Insight*: The model detects most frauds, but recall on unseen data is slightly lower, which is common in imbalanced problems. Using more domain features or ensemble tuning could improve this further.

---

## 🛠 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- imbalanced-learn (SMOTE)
- Matplotlib, Seaborn

---

## ✅ How to Run

1. Clone the repository:
```bash
git clone https://github.com/amalroy2003/Fraud-Detection-Projec.git
cd Fraud-Detection-Project
