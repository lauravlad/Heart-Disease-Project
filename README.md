# Heart-Disease-Project

In this project we uploaded Heart.csv dat aset from kagle. After analysing some features I realized that there were some errors in it. To start with: the target feature had 0 for heart disease and 1 for healthy, the eaxct oposite of what the feature description was. I decided to uploade the pre-processed dataset directly from UC Irvine Machine Learning Repository. I cleaned the data, turn category features into dummy categories, normalized continuous data, and checked it for correlations.
I built five models using: Bagging, Random Forest, Logistic Regression, XGBoost and KNeighbors. 
I Used Gridsearch to look for the best hyperparameters.
Logistic Regression Model performed the best from Recall score point of view and Accuracy so I used the parameters found with Gridsearch to fit a final Logistic Regression Model.
Following the suggestions from the feature importance plot I focused on 4 features:
Fasting Blood Sugar seem to be a good indicator for cardiovascular diseases.
Thalium stress test result (reversible defect) - High indicator for Heart Disease
                                               

Sex                                            - Taken with a grain of salt, man are more                                                      prone to developing heart disease.

Exercise Indused Angina                        - Good indicator for Heart Disease
            
Recommendations¶
For a cardiologist:

Stress the ideea that male in their thirties should watch their diet and work on becoming more active.

Women are more likely to not beeing taken seriously if they experience heart issues earlier in life.

Recommend further investigations for pacients who : - have high level of blood sugar,
                                                    - experience exercise induced angina,
                                                    - have a Thalium Stress Test reversible effect.
                                                    
Future Work¶

Find a more recent dataset with pacients evaluated for cardiovascular diseases and buid a model on that dataset. Statistics have changed a lot since 30+ yewars ago.

Improve the XGBoost Model with the best hyperparameters found with SearchGrid.