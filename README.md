# Credit Card Default Prediction (Ensemble Boosting & SVM)

This project compares modern gradient boosting algorithms (AdaBoost, Gradient Boosting, XGBoost, and LightGBM) and Support Vector Machines (SVM) to predict whether a credit card client will default on their next payment.

## What is in this project?
- Dataset: 30,000 credit card client records with 23 financial and demographic features (e.g., credit limit, age, bill statements, previous repayments).
- Data Preprocessing: Label-encoded categorical variables (SEX, EDUCATION, MARRIAGE) and scaled input features.
- Algorithms Compared:
  - AdaBoost Classifier (AdaBoostClassifier)
  - Gradient Boosting Classifier (GradientBoostingClassifier)
  - Extreme Gradient Boosting (XGBClassifier)
  - LightGBM Classifier (LGBMClassifier)
  - Support Vector Classifier (SVC(kernel='linear') and SVC(kernel='rbf'))
- Feature Importance: Extracted and ranked the top 10 predictive features influencing client defaults (e.g., PAY_1, PAY_AMT1).

## Results Summary
- LightGBM achieved the highest test accuracy of ~82.5% with the fastest wall-clock training efficiency.
- Gradient Boosting achieved ~82.3% test accuracy.
- AdaBoost scored ~82.2% test accuracy.
- Repayment status in September (PAY_1) was identified as the single most critical predictor of default across all tree models.

## Tools Used
- Python
- Pandas & NumPy
- Scikit-Learn
- XGBoost & LightGBM
- Seaborn & Matplotlib
