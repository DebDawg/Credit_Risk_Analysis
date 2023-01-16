# Loan Predication Analysis
## Overview
The purpose of this analysis is to use different techniques to train and evaluate models with unbalanced classes.  While using the imbalanced-learn model and Scikit-learn libraries we will build and evaluate models using resampling.
Using a dataset from LendingClub we will oversample the data using RandomOverSampler and SMOTE algorithms and undersample the data using ClusterCentroids algorithm.  Then we will combine with SMOOTEEN algorithm, then compare using two machine learning models to reduce bias, (BalanceRandomForestClassifier and EasyEnsembleClassifier).  Let’s evaluate whether these models should be used to predict credit risk.
Results:
-	Logistic Regression Model
-	Balanced Accuracy Score
-	Confusion Matrix
-	Imbalanced Classification Report
Naïve Random Oversampling
SMOTE Oversampling
Undersampling
Combination (Over and Under Sampling)
Balanced Random Forest Classifier

Easy Ensemble AdaBoost Classifier
-	precision
-	recall scores of all six machine learning models (15 pt)
•	Summary:
o	There is a summary of the results (2 pt)
o	There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
