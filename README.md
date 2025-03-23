# 🍷 Predicting-White-Wine-Quality
This project aims to predict the quality of white wine based on its physicochemical characteristics using regression models and data analysis.

---

## 📌 **Project Objective**
Predict the quality of white wine based on its chemical composition, using different regression models to find the best fit for the problem.

--- 

## 📂 **Dataset**
The dataset used is the [Wine Quality](https://archive.ics.uci.edu/dataset/186/wine+quality) from the UCI Machine Learning Repository, containing data related to the chemical composition of white wine an its quality.

---

## 📝 **Methodology**
1. **Exploratory Data Analysis (EDA):**
  - Analysis of variable distribution.
  - Checking correlations between variables.
  - Removing outliers using the IQR method.

2. **Data Preprocessing:**
   - Splitting features (`features`) and target (`target`).
   - Data scaling with `StandardScaler`.

3. **Feature Selection:**
   - Applying `SelectKBest` to analyze feature importance.

4. **Models Applied:**
   - Linear Regression.
   - Lasso.
   - Ridge.
   - Decision Tree.

5. **Model Evaluation:**
   - Metrics used: `MSE`, `RMSE`, `MAE`, `MAPE`, `R²`.
   - Performance comparison between models.
  
  ---

## 🔍 **Results**
| Model              | MSE  | RMSE | MAE  | MAPE (%)  | R²    |
|--------------------|------|------|------|-----------|-------|
| Linear Regression  | 0.470| 0.685| 0.563| 9.888     | 0.233 |
| Lasso              | 0.516| 0.719| 0.582| 10.294    | 0.157 |
| Ridge              | 0.470| 0.685| 0.563| 9.888     | 0.233 |
| Decision Tree      | 0.582| 0.763| 0.460| 8.221     | 0.051 |

--- 

## 📊 **Analysis of Results**
- **Linear Models (Linear Regression, Lasso, Ridge):**  
  - Showed similar results, indicating that L1 and L2 regularization did not bring significant improvements.  
  - The MAPE around 10% suggests that linear models are struggling to capture the complexity of the problem.  

- **Decision Tree:**  
  - Showed the lowest MAPE (~8.22%), indicating that a non-linear approach is better suited for this problem.  
  - However, the low R² suggests potential overfitting or the need for hyperparameter tuning.  

---

## 💡 **Potential Improvements**
- Test more complex models such as `Random Forest` and `XGBoost`.
- Tune model hyperparameters to improve performance.
- Perform more robust feature selection to eliminate irrelevant variables.
- Reassess the impact of outlier removal on model performance.

---

## 📌 **Conclusion**
Linear models showed similar performance, indicating that regularization techniques were not effective in improving the model. The Decision Tree achieved better performance in terms of MAPE, but with a low R². 

---

## 🚀 **Next Steps**
- Implement advanced techniques such as Random Forest and XGBoost.  
- Perform hyperparameter tuning to enhance model performance.  

---
