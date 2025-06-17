**Yellow Taxi Trip Fare & Tip Prediction**
This project explores and models 2017 NYC Yellow Taxi trip data using machine learning to solve two real-world problems:

Project Goals:
1)Predict Fare Amount : Applied Linear Regression to estimate taxi fare based on trip features.
2)Predict Tip Behavior : Used Random Forest and XGBoost classifiers to predict whether a customer would leave a tip.

Dataset Overview
Source: NYC Taxi & Limousine Commission
~22,000 records from 2017 Yellow Taxi trips
Features include:
Pickup & dropoff datetime
Trip distance & passenger count
Payment type
Fare, tip, tolls, and total amounts
Pickup/Dropoff location IDs

Model Performance:
1. Linear Regression – Fare Prediction
R²: 0.891
MAE: 1.99
RMSE: 3.48
✅ Explained ~89% of fare variability with low prediction error.

2. Random Forest & XGBoost – Tip Classification
Model	Precision	Recall	F1 Score	Accuracy
RF (CV)	0.6749	0.7573	0.7136	0.6802
RF (Test)	0.6753	0.7791	0.7235	0.6865
XGB (CV)	0.6689	0.7234	0.6950	0.6658
XGB (Test)	0.6772	0.7455	0.7097	0.6790
✅ Random Forest slightly outperformed XGBoost on most metrics.

Technologies & Tools:
Python, Jupyter Notebook
Pandas, NumPy, Scikit-learn, XGBoost
Matplotlib, Seaborn

Key Takeaways:
Trip distance is the most significant predictor of fare.
Tipping behavior is influenced by distance and payment type (card users tip more).
Further feature engineering (e.g., day of week, time of day) could improve model performance.
Demonstrates practical applications of regression and classification in real-world transport data.


