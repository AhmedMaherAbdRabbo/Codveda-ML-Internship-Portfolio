# 🤖 Task 3: Implement K-Nearest Neighbors (KNN) Classifier

## 📌 Task Level: Basic  
**Domain**: Machine Learning  
**Tools Used**: Python, Pandas, Scikit-learn, Seaborn, Matplotlib

---

## 🎯 Objectives

- Train a K-Nearest Neighbors (KNN) model on a labeled dataset.
- Evaluate the model using:
  - Accuracy
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-score)
- Compare model performance across different values of **K**.

---

## 🗂️ Dataset

- **File Name**: `1) iris.csv`  
- **Description**: The classic Iris dataset, containing 150 samples with 4 features each (sepal and petal dimensions), categorized into 3 species of iris flowers.

---

## ✅ Steps Completed

1. **Imported Required Libraries**  
   - Used `pandas` for data handling, `seaborn` and `matplotlib` for visualization, and `sklearn` for model training and evaluation.

2. **Loaded and Explored the Dataset**  
   - Previewed with `.head()`, `.tail()`, `.sample()`, checked unique values and data types.

3. **Handled Missing Values**  
   - Confirmed there are no nulls using `.isna().sum()`.

4. **Separated Features and Target**  
   - `X` includes numerical features.  
   - `y` contains the target class `species`.

5. **Split Dataset into Training and Testing Sets**  
   - Used `train_test_split()` with a 70-30 split and `random_state=9`.

6. **Normalized Features**  
   - Standardized features using `StandardScaler` for better KNN performance.

7. **Trained KNN Classifier with Multiple K Values**  
   - Trained and tested the KNN model for `K = 1, 3, 5, 7`.

8. **Evaluated Model Performance**  
   - For each `K`, printed:
     - Accuracy
     - Confusion Matrix
     - Classification Report
   - Visualized confusion matrices with heatmaps.

---

## 🔢 KNN Results Summary

- **K = 1**: High sensitivity to noise, overfitting likely.  
- **K = 3**: Improved generalization, better class separation.  
- **K = 5**: Balanced performance across classes.  
- **K = 7**: Slight drop in performance due to over-smoothing.  

Each K value offered trade-offs between precision and recall across the different iris species. The confusion matrix heatmaps clearly showed how class predictions varied with K.

> (Exact values depend on split randomness and normalization.)

Confusion matrices and classification reports were generated for each K value to analyze the precision, recall, and overall classification performance.


---

## 📦 Outcome

A fully functional KNN classification model was implemented and evaluated.  
The model:
- Achieved high classification performance on the Iris dataset.
- Highlighted the importance of normalization before applying KNN.

---



