# 📊 Task 3: K-Means Clustering – Customer Segmentation

## 📝 Task Overview

**Level:** Intermediate  
**Objective:** Apply K-Means Clustering to segment unlabeled data based on customer behavior.

## 🎯 Goals

- Load and preprocess a customer dataset.
- Apply feature scaling to standardize numerical features.
- Use the **Elbow Method** to determine the optimal number of clusters.
- Apply **K-Means** to segment data.
- Visualize customer clusters using key features.
- Interpret clustering results for business insights.

## 📂 Dataset

- Source: `churn-bigml-80.csv`
- Features used: Numerical attributes related to call duration and plan types.
- Target column (`Churn`) was excluded during clustering.

## ⚙️ Steps Performed

1. **Data Loading & Exploration:**
   - Loaded the dataset and previewed records.
   - Identified and handled missing/null values.

2. **Data Cleaning:**
   - Removed non-numeric and target columns (`State`, `Churn`).
   - Converted categorical plans (`International plan`, `Voice mail plan`) to numeric format.

3. **Feature Scaling:**
   - Used `StandardScaler` to normalize features.

4. **Optimal K Determination:**
   - Implemented the **Elbow Method** with inertia plot.
   - Chose **K = 3** as the optimal number of clusters.

5. **Clustering:**
   - Applied `KMeans(n_clusters=3)`.
   - Added cluster labels to the DataFrame.

6. **Visualization:**
   - Plotted a 2D scatter plot using:
     - `Total day minutes` (x-axis)
     - `Total eve minutes` (y-axis)
     - Colored by cluster label

## 📈 Clustering Outcome

- Customers were segmented into **3 distinct clusters** based on usage patterns.
- Clear separation observed between customers based on daytime and evening call durations.
- This clustering can assist in targeted marketing, plan recommendations, or churn prediction.

## 🛠️ Tools Used

- **Python**  
- **pandas**, **scikit-learn**, **matplotlib**, **seaborn**

---

