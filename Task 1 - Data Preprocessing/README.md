# 🧹 Task 1: Data Preprocessing for Machine Learning

## 📌 Task Level: Basic  
**Domain**: Machine Learning  
**Tools Used**: Python, Pandas, Scikit-learn

---

## 🎯 Objectives

- Handle missing data (e.g., using mean, median, or dropping).
- Encode categorical variables using One-Hot Encoding.
- Normalize or standardize numerical features.
- Split the dataset into training and testing sets.

---

## 🗂️ Dataset

- **File Name**: `churn-bigml-20.csv`
- **Description**: This dataset contains customer behavior data used to predict churn (whether a customer will leave a service).

---

## ✅ Steps Completed

1. **Imported Required Libraries**  
   - Used `pandas` for data manipulation and `scikit-learn` for preprocessing and splitting.

2. **Loaded and Explored the Dataset**  
   - Viewed the first and last few rows, checked the data types, sample entries, and unique values.

3. **Handled Missing Values**  
   - Checked for nulls using `.isna().sum()` and `.info()`.

4. **Separated Features and Target**  
   - Features stored in `X`, and the target variable `Churn` converted to integers in `y`.

5. **Encoded Categorical Variables**  
   - Applied One-Hot Encoding to categorical columns using `pd.get_dummies()` with `drop_first=True` to avoid multicollinearity.

6. **Standardized Numerical Features**  
   - Used `StandardScaler` to normalize all numerical columns.

7. **Split the Data**  
   - Split into training and testing sets using `train_test_split()` with an 80-20 ratio.

---

## 📊 Output Shapes

```

X_train shape: (533, 68)
X_test shape: (134, 68)
y_train shape: (533,)
y_test shape: (134,)

```

---

## 📦 Outcome

The dataset is now fully preprocessed and ready for machine learning models.  
It is:
- Clean (no missing values)
- Encoded (all categorical features are numeric)
- Standardized (numerical features are scaled)
- Split into training and testing sets

---
