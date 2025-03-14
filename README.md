# 📌 Energy Efficiency Regression and Clustering Analysis

## 🚀 Project Overview
This project analyzes **energy efficiency in buildings** using machine learning techniques. The dataset, **ENB2012_data.xlsx**, contains various architectural and environmental factors influencing heating and cooling loads. The analysis is split into two parts:

1. **Part A: Clustering Analysis** – Investigates the structure of the data using **DBSCAN and Agglomerative Clustering** with feature preprocessing methods such as **Standardization and PCA**.
2. **Part B: Regression Modeling** – Predicts energy efficiency using **Random Forest, Gradient Boosting, SGD Regressor, and Linear Regression**, with hyperparameter tuning and performance evaluation.

---

## 📊 Dataset: ENB2012_data.xlsx
The dataset includes **architectural features** (e.g., wall area, roof area, orientation) and **target variables**:  
- **Heating Load (Y1)** – Energy required to heat the building.  
- **Cooling Load (Y2)** – Energy required to cool the building.  

---

## ⚡ Part A: Clustering Analysis
We applied **unsupervised learning** to explore patterns in the dataset:  

### 🔍 **Preprocessing**
- Standardization and PCA for dimensionality reduction.

### 🔗 **Clustering Techniques**
- **DBSCAN** (Density-Based Spatial Clustering of Applications with Noise)
- **Agglomerative Clustering**

### 📏 **Evaluation Metrics**
- **Silhouette Score**  
- **Calinski-Harabasz Index**  
- **Davies-Bouldin Index**  

### 📈 **Key Findings**
- PCA significantly improved clustering performance.
- DBSCAN identified outliers.
- Agglomerative Clustering captured hierarchical structures.

---

## 🔥 Part B: Regression Modeling
In **supervised learning**, we predicted energy efficiency using **various regression models** and assessed their reliability.

### 🔎 **Methodology**
1. **Feature Engineering**:  
   - Created an **interaction term** between features.
2. **Random Splitting & K-Fold Cross-Validation**:
   - Assessed model robustness using **MSE, variance, and IQR**.
3. **Hyperparameter Tuning**:
   - **RandomizedSearchCV** optimized **Random Forest** parameters.
4. **Comparison of Models**:
   - **Random Forest, Gradient Boosting, SGD Regressor, Linear Regression**.
   - Evaluated **generalization vs. memorization**.

### 📈 **Key Results**
- **Gradient Boosting** showed the lowest **MSE variance**, ensuring stable predictions.
- **SGD Regressor** exhibited extreme instability with **IQR of 2.01 * 10^29**.
- **Random Forest** performed well with moderate variance and strong generalization.


---

## 🛠 Technologies Used
- **Python (Jupyter Notebook)**
- **Pandas, NumPy** (Data Manipulation)
- **Scikit-Learn** (Machine Learning)
- **Matplotlib, Seaborn** (Data Visualization)

---

## 📌 How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/energy-efficiency-analysis.git
