# Student-Performance-Prediction-Using-Machine Learning
**Linear Regression vs Random Forest**

## 📌 Project Overview
This project focuses on predicting **student academic performance** using machine learning models. Two regression models are implemented and compared:

- Linear Regression  
- Random Forest Regressor  

The objective is to evaluate model performance in predicting final student grades based on academic, demographic, and behavioral features.

---

## 📊 Dataset
The dataset from Kaggle (https://www.kaggle.com/datasets/larsen0966/student-performance-data-set) contains student-related attributes including:

- Academic scores: `G1`, `G2`
- Demographics: `age`, parental education
- Behavioral factors: `absences`, `freetime`, `goout`, `Walc`, `health`, etc.

**Target variable:**  
- `G3` (Final grade)

---

## 🔎 Exploratory Data Analysis (EDA)
The following EDA steps were performed:

- Histogram of numerical features
- Frequency distribution of categorical (object) features
- Correlation matrix for numerical features
- Age distribution analysis  
  - Result: no outliers detected, no further treatment required

---

## 🧹 Data Preprocessing
- Encoding categorical features
- Train-test split with test size = 0.3
- Feature scaling using StandardScaler

---

## 🤖 Model Training & Evaluation

### Linear Regression
**Performance Metrics:**
- MAE: 0.78  
- MSE: 1.44  
- RMSE: 1.20  
- R² Score: 0.87  

---

### Random Forest Regressor
**Configuration:**
- Number of estimators: 100  

**Performance Metrics:**
- MAE: 0.95  
- RMSE: 1.65  
- R² Score: 0.75  

---

## ⭐ Feature Importance (Random Forest)
Top contributing features:

G2 0.165381
G1 0.104315
absences 0.047812

---

## 📈 Visualization
- Histogram and frequency plots from EDA
- Correlation matrix heatmap
- Prediction vs actual plots for Linear Regression
- Prediction vs actual plots for Random Forest
- Model performance comparison plots

---

## 🧠 Conclusion
- Linear Regression achieved better performance compared to Random Forest.
- The dataset shows strong linear relationships, particularly with previous grades (`G1`, `G2`).
- Random Forest may benefit from further hyperparameter tuning or more complex feature interactions.

---

## 🛠️ Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## 🚀 Future Work
- Hyperparameter tuning for Random Forest
- Cross-validation
- Feature selection
- Experiment with other models (XGBoost, SVR)
