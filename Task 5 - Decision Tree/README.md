# 🌳 Intermediate Task 2 – Decision Trees for Classification

## 📌 Task Level: Intermediate  
**Domain**: Machine Learning  
**Tools Used**: Python, Pandas, Scikit-learn, Seaborn, Matplotlib  

---

## 📌 Task Description

This task involves building a **Decision Tree Classifier** to predict the species of flowers using the **Iris dataset**. The process includes training the model, visualizing the decision tree structure, pruning to control overfitting, and evaluating performance using classification metrics.

---

## 🎯 Objectives

- Train a Decision Tree Classifier on a labeled dataset.
- Predict the flower species based on numerical features.
- Visualize the decision tree structure.
- Apply depth restriction to avoid overfitting (i.e., pruning).
- Evaluate model performance using:
  - Accuracy
  - F1 Score
  - Classification Report

---

## 🧰 Tools & Libraries

- `Python`
- `pandas`
- `scikit-learn`
- `matplotlib`

---

## 🗂️ Dataset Info

- **Dataset Used**: Iris dataset  
- **Target Variable**: `species`  
- **Features**: `sepal length`, `sepal width`, `petal length`, `petal width`

---

## ⚙️ Workflow Summary

1. **Data Loading & Exploration**
   - Checked for missing values and inspected data distribution.

2. **Data Preparation**
   - Separated features (`X`) and target (`y`).
   - Split data into training (80%) and testing (20%) sets.

3. **Model Training**
   - Used `DecisionTreeClassifier` from `sklearn.tree`.
   - Limited tree depth (`max_depth=2`) to reduce overfitting.

4. **Prediction & Evaluation**
   - Made predictions on the test set.
   - Calculated:
     - Accuracy
     - Weighted F1-score
     - Classification report

5. **Visualization**
   - Plotted the decision tree with class names and feature labels.

---

## 📊 Final Results

- **Max Depth**: 2  
- **Accuracy**: ~96.6%  
- **F1 Score**: ~96.6% (weighted)  
- The model showed strong classification performance while remaining simple and interpretable.

---

## Visualization

> The plotted decision tree clearly shows the decision splits based on petal measurements, effectively separating the species classes.

---

## ✔ Achievements

- ✔ Built and trained a Decision Tree Classifier.
- ✔ Controlled overfitting using `max_depth`.
- ✔ Achieved high accuracy and balanced F1-score.
- ✔ Visualized the tree for clear understanding.

---
