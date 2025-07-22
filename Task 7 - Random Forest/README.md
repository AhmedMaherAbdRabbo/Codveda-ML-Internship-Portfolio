# 🌲 Task 1: Random Forest Classifier – Churn Prediction

## 📝 Task Overview

**Level:** Advanced  
**Objective:** Build a robust classification model using Random Forests to predict customer churn based on behavior and service usage features.

---

## 🎯 Goals

- Load and preprocess the churn dataset.
- Encode categorical variables into numeric format.
- Train a **Random Forest Classifier** with specified hyperparameters.
- Evaluate the model using:
  - **Classification Report**
  - **Confusion Matrix**
  - **Cross-Validation (F1 Score)**
- Analyze feature importance to understand key drivers of churn.

---

## 📂 Dataset

- **Source:** `churn-bigml-20.csv`
- **Target Variable:** `Churn` (binary: 0 = No, 1 = Yes)
- **Removed Column:** `State` (non-numeric, not used in model)
- **Features Include:**
  - Account length, number of customer service calls
  - Day, evening, night, and international call durations and charges
  - `International plan` and `Voice mail plan`

---

## ⚙️ Steps Performed

1. **Data Loading & Exploration**
   - Previewed dataset using `.head()`, `.tail()`, and `.sample()`
   - Checked for missing values and data types using `.info()`

2. **Data Cleaning**
   - Dropped irrelevant column: `State`
   - Converted categorical columns:
     - `International plan`, `Voice mail plan` → 0 (No), 1 (Yes)
     - `Churn` → 0 (False), 1 (True)

3. **Train-Test Split**
   - Split dataset into:
     - 80% training
     - 20% testing
   - Ensured reproducibility with `random_state=42`

4. **Model Training**
   - Trained a `RandomForestClassifier` with:
     - `n_estimators=100`
     - `max_depth=8`

5. **Prediction & Evaluation**
   - Predicted `y_test` using trained model
   - Evaluated model using:
     - `classification_report`
     - `confusion_matrix`

6. **Cross-Validation**
   - Applied 5-fold cross-validation using F1-score
   - Computed average cross-validation F1-score

7. **Feature Importance**
   - Calculated and visualized feature importance using bar plot
   - Identified top predictive features for churn (e.g., `customer service calls`, `international charge`, etc.)

---

## 📈 Model Outcome

- **Classifier Type:** Random Forest (100 trees, depth 8)
- **Evaluation Results:**
  - High precision and recall for both churn and non-churn classes
  - Balanced F1-score confirmed via cross-validation
- **Feature Importance Insights:**
  - Features like `number vmail messages`, `customer service calls`, and `total intl charge` had the highest influence on predictions

---

## 🛠️ Tools Used

- **Python**
- **pandas**, **scikit-learn**, **matplotlib**, **seaborn**

---

