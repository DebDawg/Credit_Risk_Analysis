# Credit Risk Analysis

## Overview

The purpose of this analysis is to use different techniques to train and evaluate models with unbalanced classes.  While using the imbalanced-learn model and Scikit-learn libraries we will build and evaluate models using resampling.

Using a dataset from LendingClub we will oversample the data using RandomOverSampler and SMOTE algorithms and undersample the data using ClusterCentroids algorithm.  Then we will combine with SMOOTEEN algorithm, then compare using two machine learning models to reduce bias, (BalanceRandomForestClassifier and EasyEnsembleClassifier).  Let’s evaluate whether these models should be used to predict credit risk.

## Results

The first models we compare are two Oversampling algorithms, Naïve Random Oversampling and SMOTE Oversampling.  As seen below there is not a lot of differentiation between the two.

  - Naïve Random Oversampling

    ![Picture1](https://user-images.githubusercontent.com/110787194/213091187-e06fac95-8d6d-4d37-838f-f4d91a363c77.png)

  - SMOTE Oversampling

    ![Picture2](https://user-images.githubusercontent.com/110787194/213091194-7ef6ac02-d831-4828-99bc-21a8c9252fc2.png)


The Next models we compare are two Undersampling algorithms,  ClusterCentroids resampler and the Combination (Over and Under) Sampling.  There is a slight differentiation between these two if you look at the f1 score, however the prediction stays the same.  I don't feel this model proved to be the one to use, due to the lower f1 scores.

  - ClusterCentroids resampler
 
    ![Picture3](https://user-images.githubusercontent.com/110787194/213091198-6f2745b1-ced1-4f01-9554-6d55e04251b1.png)

  - SMOTEENN
  
    ![Picture4](https://user-images.githubusercontent.com/110787194/213091202-1b2a1e1c-d44b-4973-bfa5-603b509532cc.png)
    
After resampling the date and using two methods, Random Forest Classifier and Easy Ensemble AdaBoost Classifier did increase the f1 ratio, which is at 0.97, which is the closest model to reach the 1.00.

  - Random Forest Classifier

    <img width="355" alt="Picture5" src="https://user-images.githubusercontent.com/110787194/213639174-bd496468-3383-44be-974c-0c777cd431ab.png">

  - Easy Ensemble AdaBoost Classifier

    <img width="354" alt="Picture6" src="https://user-images.githubusercontent.com/110787194/213639551-e4774e6a-be5e-4988-ae63-3967cb14dc63.png">


## Summary

The Easy Ensemble AdaBoot Classifier (EEAC), proved to be the better models out of all the testing for credit risk.  I do feel if we added more data to this analysis, we may see better results.  Each model did prove to have differences with the precision meeting the needs of each model.  However, the Easy Ensemble AdaBoost Classifier (EEAC) did prove to be the best model with 0.97 f1 score.  Having a f1 score closer to 1 seems a bit more respectable.  The EEAC did help determine credit risk.  I do believe with more data there could be better results.



