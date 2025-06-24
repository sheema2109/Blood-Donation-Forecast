Blood Donation Forecasting using Machine Learning
This project aims to predict whether a person is likely to donate blood in the future using a classification model. It addresses a significant challenge in the healthcare system by helping forecast blood donations based on past behavior.

Dataset
The dataset used is the Blood Transfusion Service Center Data Set, available from the UCI Machine Learning Repository. It contains 748 records and 5 columns:
Recency: months since last donation
Frequency: total number of donations
Monetary: total blood donated (in c.c.)
Time: months since first donation
Donation: target variable (1 if donated in March 2007, else 0)

Objectives
The goal is to train a machine learning model to accurately predict future blood donations using features such as donation frequency, recency, and time. The process includes data preprocessing, model training, hyperparameter tuning, evaluation, and interpretation.

Technologies Used
Python
Pandas and NumPy for data handling
Matplotlib and Seaborn for data visualization
Scikit-learn for model building and evaluation

Steps Followed
Loaded and explored the dataset
Visualized data relationships and distributions
Preprocessed the data (standard scaling, train-test split)
Built baseline models using Logistic Regression and Random Forest
Tuned the Random Forest model using GridSearchCV
Evaluated model performance using classification metrics and ROC-AUC
Visualized feature importance to understand key predictors

Results
The tuned Random Forest model achieved a test ROC-AUC score of approximately 0.78. It performed well in identifying non-donors but had room for improvement in identifying actual donors due to class imbalance. The most important features were time since first donation and donation frequency.

Conclusion
This project demonstrates how machine learning can be used to support healthcare forecasting. With improved feature engineering or additional data, the model could be enhanced further to assist blood banks in donor prediction and outreach.
