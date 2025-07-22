# 🏠 Task 2: Build a Simple Linear Regression Model

## 📌 Task Level: Basic  
**Domain**: Machine Learning  
**Tools Used**: Python, Pandas, Scikit-learn

---

## 🎯 Objectives

- Load and preprocess a housing dataset.
- Train a linear regression model using Scikit-learn.
- Interpret the model coefficients to understand feature impact.
- Evaluate the model using R-squared (R²) and Mean Squared Error (MSE).

---

## 🗂️ Dataset

- **File Name**: `4) house Prediction Data Set.csv`  
- **Description**: Boston Housing dataset containing various features related to houses in Boston suburbs, aiming to predict median house value (`MEDV`).

---

## ✅ Steps Completed

1. **Imported Required Libraries**  
   - Used `pandas` and `numpy` for data handling.  
   - Used `sklearn` for model building and evaluation.

2. **Loaded the Dataset**  
   - Data was read using `read_csv()` with whitespace separator and no header.  
   - Assigned meaningful column names manually.

3. **Exploratory Data Inspection**  
   - Previewed the data using `.head()`, `.tail()`, `.sample()`  
   - Checked data types and unique values using `.info()` and `.nunique()`.

4. **Handled Missing Values**  
   - Verified there are no missing values using `.isna().sum()`.

5. **Separated Features and Target Variable**  
   - `X` includes all features.  
   - `y` is the target variable `MEDV` (median house price).

6. **Split the Dataset**  
   - Split into training (80%) and testing (20%) using `train_test_split`.

7. **Trained Linear Regression Model**  
   - Model trained using `LinearRegression().fit(X_train, y_train)`  
   - Printed the learned coefficients for each feature.

8. **Interpreted Model Coefficients**  
   - Positive coefficient ➝ feature increase leads to higher price.  
   - Negative coefficient ➝ feature increase leads to lower price.

9. **Evaluated the Model**  
   - Used `mean_squared_error` and `r2_score` for performance metrics.

---

## 📊 Model Performance

```

X\_train shape: (404, 13)
X\_test shape:  (102, 13)
y\_train shape: (404,)
y\_test shape:  (102,)

```

### 🔍 Evaluation Results

```

Mean Squared Error (MSE): 24.291
R-squared Score (R²):     0.668

```

---

## 📦 Outcome

The linear regression model was successfully built and evaluated.  
It is now ready for use in predicting house prices based on input features such as crime rate, number of rooms, and property tax rate.

---


