# predictive-maintenance-ml
Production-grade IoT Predictive Maintenance System using Time-Series ML. Includes feature engineering, XGBoost model, SHAP explainability, and Flask API deployment.
# Predictive Maintenance ML

## Project Overview
This project predicts machine failures using time-series sensor data (temperature, vibration, pressure).

## Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn, XGBoost
- SHAP (Explainability)
- Flask API
- Docker

# Predictive Maintenance ML Project

##  Datasets
- AI4I Predictive Maintenance Dataset (Classification)
- NASA Turbofan Engine Dataset (Regression)

---

## Models Used

### AI4I (Classification)
- Logistic Regression
- Random Forest
- XGBoost (Final Model)

### NASA (Regression)
- Linear Regression
- Random Forest Regressor
- XGBoost Regressor (Final Model)

---

## Techniques Applied
- Feature Engineering
- SMOTE (Class Imbalance Handling)
- GridSearchCV (Hyperparameter Tuning)

---

## Results

### AI4I Dataset

|   Model             | Accuracy | Precision | Recall | F1 Score |
|------|--------------|----------|-----------|--------|----------|
| Logistic Regression | ~0.95    | ~0.41     | ~0.97  | ~0.57    |
| Random Forest       | ~0.97    | ~0.56     | ~0.97  | ~0.71    |
| XGBoost             | ~0.98    | ~0.66     | ~0.97  | ~0.78    |

Final Model: **XGBoost Classifier**

---

### NASA Dataset

                    | Model| MAE | RMSE |
                    |------|-----|------|
| Linear Regression | ~29  | ~36 |
| Random Forest     | ~17  | ~23 |
| XGBoost           | ~16  | ~22 |
| Tuned XGBoost     | 15.58| 21.63|

Final Model: **Tuned XGBoost Regressor**

---

## Key Insights
- AI4I dataset is highly imbalanced → handled using SMOTE
- Recall is critical for failure prediction
- XGBoost outperformed all baseline models
- Hyperparameter tuning improved performance

---

## Final Conclusion
Tuned XGBoost models achieved the best performance for both classification and regression tasks.
