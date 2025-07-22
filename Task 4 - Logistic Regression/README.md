# 📊 Task 1: Logistic Regression for Binary Classification

## 📌 Task Level: Intermediate  
**Domain**: Machine Learning  
**Tools Used**: Python, Pandas, Scikit-learn, Seaborn, Matplotlib

---

## 🎯 Objectives

- Apply **Logistic Regression** to perform binary classification.
- Evaluate the model using:
  - **Confusion Matrix**
  - **Classification Report** (Precision, Recall, F1-score)
  - **Accuracy Score**
- Interpret results and assess the effectiveness of the model.

---

## 🗂️ Dataset

- **File Name**: `2) Social_Network_Ads.csv`
- **Description**: A dataset representing user behavior on a social network.  
  Includes:
  - `Age`  
  - `EstimatedSalary`  
  - `Purchased` (Target: 0 or 1)

---

## ✅ Steps Completed

1. **Imported Required Libraries**  
   Used `pandas`, `numpy`, `matplotlib.pyplot`, `seaborn`, and `sklearn`.

2. **Loaded and Inspected the Dataset**  
   - Displayed data sample and shape  
   - Verified dataset contains no missing values

3. **Selected Relevant Features**  
   - Selected `Age` and `EstimatedSalary` as input features (`X`)  
   - `Purchased` used as target (`y`)

4. **Split Dataset**  
   - 75% for training, 25% for testing using `train_test_split()`  
   - Set `random_state=0` for reproducibility

5. **Feature Scaling**  
   - Standardized features using `StandardScaler` for better model performance

6. **Trained Logistic Regression Model**  
   - Fitted model to training data using `LogisticRegression()`

7. **Model Prediction & Evaluation**  
   - Predicted on test set  
   - Evaluated using:
     - **Confusion Matrix**  
     - **Classification Report**  
     - **Accuracy Score**

8. **Visualized Results**  
   - Plotted decision boundary for both training and test sets  
   - Showed how well the model separates the two classes

---

## 🧠 Final Insights

- Logistic Regression achieved **good classification performance** on the binary problem.
- Model was able to **distinguish between users who purchased and those who didn’t** based on `Age` and `EstimatedSalary`.
- Decision boundary was **clearly visualized** to understand model behavior.
- Confusion matrix and classification report highlighted **balance between precision and recall**, with minor trade-offs.

---

## 📁 Output Files

- Visual plots of decision boundaries for both train and test sets
- Printed evaluation metrics: confusion matrix, classification report, and accuracy score

---
