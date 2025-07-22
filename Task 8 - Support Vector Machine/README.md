# 🧠 Advanced Task 2: Support Vector Machine (SVM) for Classification

## 📝 Task Overview

**Level:** Advanced  
**Objective:** Implement and evaluate Support Vector Machine (SVM) models using different kernels (linear and RBF) for binary classification, and compare their performance using precision, recall, accuracy, AUC, and ROC curves.

## 📄 Task Description

In this advanced-level task, a **Support Vector Machine (SVM)** model is implemented to perform **binary classification** on a labeled dataset. The objective is to explore and compare the performance of SVM with different kernels, and evaluate the model using various metrics.

---

## 🎯 Objectives

- Train a Support Vector Machine model for binary classification.
- Use different kernels (linear and RBF) to compare performance.
- Normalize features using StandardScaler.
- Evaluate the model using:
  - Accuracy
  - Precision
  - Recall
  - AUC (Area Under Curve)
- Visualize the ROC Curve for each kernel.

---

## 🛠️ Tools Used

- Python
- pandas
- matplotlib
- seaborn
- scikit-learn

---

## 📂 Dataset

The dataset used for this task is:

churn-bigml-80.csv


- Target variable: Churn (0 = No, 1 = Yes)
- Features include call durations, number of customer service calls, usage statistics, and subscription details.

---

## ⚙️ Model Training

- **Label Encoding** for categorical columns (International plan, Voice mail plan, Churn).
- Removed the non-numeric column State.
- Features were **normalized** using StandardScaler.
- Trained SVC models using:
  - kernel='linear'
  - kernel='rbf'

---

## 📊 Evaluation Metrics

For each kernel, the model was evaluated using:

- **Classification Report** (Precision, Recall, F1-score)
- **Confusion Matrix**
- **AUC Score**
- **ROC Curve Visualization**

---

## 🧪 Results

- Each kernel's performance was plotted on the ROC Curve.
- The best kernel was selected based on **highest accuracy**.

> ✅ **Best Accuracy Achieved**: Shown at the end of the notebook  
> 📈 ROC Curve includes performance of both kernels

---

## 📌 Conclusion

This task demonstrated the strength of SVMs in classification, especially when using different kernels. Visualization and evaluation helped determine the optimal configuration for the model.

---