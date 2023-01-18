# Loan Predication Analysis
## Overview
The purpose of this analysis is to use different techniques to train and evaluate models with unbalanced classes.  While using the imbalanced-learn model and Scikit-learn libraries we will build and evaluate models using resampling.
Using a dataset from LendingClub we will oversample the data using RandomOverSampler and SMOTE algorithms and undersample the data using ClusterCentroids algorithm.  Then we will combine with SMOOTEEN algorithm, then compare using two machine learning models to reduce bias, (BalanceRandomForestClassifier and EasyEnsembleClassifier).  Let’s evaluate whether these models should be used to predict credit risk.
Results:

The first models we compare are two Oversampling algorithms, Naïve Random Oversampling and SMOTE Oversampling.  As seen below there is not a lot of differentiation between the two.

  - Naïve Random Oversampling

    ![Picture1](https://user-images.githubusercontent.com/110787194/213091187-e06fac95-8d6d-4d37-838f-f4d91a363c77.png)

  - SMOTE Oversampling

    ![Picture2](https://user-images.githubusercontent.com/110787194/213091194-7ef6ac02-d831-4828-99bc-21a8c9252fc2.png)


The Next models we compare are two Undersampling algorithms,  ClusterCentroids resampler and the Combination (Over and Under) Sampling.  There is a slight differentiation between these two if you take a look at the f1

  - ClusterCentroids resampler
 
    ![Picture3](https://user-images.githubusercontent.com/110787194/213091198-6f2745b1-ced1-4f01-9554-6d55e04251b1.png)

  - SMOTEENN
  
    ![Picture4](https://user-images.githubusercontent.com/110787194/213091202-1b2a1e1c-d44b-4973-bfa5-603b509532cc.png)

   


