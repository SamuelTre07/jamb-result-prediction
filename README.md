# Student Result Prediction Using Machine Learning

This project aims to predict student academic results based on study habits, assignment performance, and demographic features. Using a dataset of student records, I explore underlying patterns and train regression models to estimate outcomes.

## Dataset
The dataset contains student records with features including:

- Gender, age, and parental education level  
- Study habits and assignment scores
- Target variable: final result score
  Source: [Student Performance in 2024 JAMB](https://www.kaggle.com/datasets/idowuadamo/students-performance-in-2024-jamb)

## EDA Highlights
- Most students have similar study assignment scores; variance is limited.  
- Target distribution is moderately spread, with no severe skew.
- Correlations between features and the target are weak, limiting predictive power.  

## Models Trained
Several regression models were trained and compared:  

- **Linear Regression (baseline)**  
- **Polynomial Features + Linear Regression**  
- **Ridge Regression** with hyperparameter tuning  

Feature scaling (MinMaxScaler) and polynomial feature expansion were tested.  

## 📈 Best Model Performance
After training on combined training and validation sets, the final **Ordinary Linear Regression** model performed best:  

| Metric | Value |
|--------|-------|
| RMSE   | 38.687 |

This represents about **22% of the mean of the target variable**, which is acceptable but indicates limited explanatory power.  

## Future Improvements
- Explore advanced models (e.g. XGBoost).
- Collection of additional features e.g **prior test scores** to boost predictive power.
- Feature engineering with domain expertise to capture stronger predictors.  
- Collect more diverse data to improve variance and correlations.

## Tech Stack
- Python, Jupyter Notebook  
- scikit-learn, pandas, matplotlib, seaborn, numpy