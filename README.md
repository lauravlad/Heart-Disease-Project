# Heart-Disease-Project
This folder contains:
1. Heart.csv dataset used to get the names of the columns,
2. processed.cleveland.csv - the dataset we used for modeling,
3. Cleveland dataset.ipynb - this file contains all the code,
4. roc_curve.png - ROC curve visualization for the 5 models used,
5. heart disease presentation pp 1.pdf - power point presentation of the project




In this project we uploaded Heart.csv dataset from kaggle. After analyzing some features I realized that there were some errors in it. To start with: the target feature had 0 for heart disease and 1 for healthy, the exact opposite of what the feature description was. I decided to upload the pre-processed dataset directly from UC Irvine Machine Learning Repository. I cleaned the data, turn category features into dummy categories, normalized continuous data, and checked it for correlations. I built five models using: Bagging, Random Forest, Logistic Regression, XGBoost and KNeighbors. I Used Gridsearch to look for the best hyperparameters. Logistic Regression Model performed the best from Recall score point of view and Accuracy so I used the parameters found with Gridsearch to fit a final Logistic Regression Model. Following the suggestions from the feature importance plot I focused on 4 features: Fasting Blood Sugar seem to be a good indicator for cardiovascular diseases. Thallium stress test result (reversible defect) - High indicator for Heart Disease
Sex - Taken with a grain of salt, man are more prone to developing heart disease.
Exercise Induced Angina - Good indicator for Heart Disease
Recommendations¶ For a cardiologist:
Stress the idea that male in their thirties should watch their diet and work on becoming more active.
Women are more likely to not being taken seriously if they experience heart issues earlier in life.
Recommend further investigations for patients who : - have high level of blood sugar, - experience exercise induced angina, - have a Thallium Stress Test reversible effect.
Future Work¶
Find a more recent dataset with patients evaluated for cardiovascular diseases and build a model on that dataset. Statistics have changed a lot since 30+ years ago.
Improve the XGBoost Model with the best hyper-parameters found with SearchGrid.
Improve the XGBoost Model with the best hyperparameters found with SearchGrid.