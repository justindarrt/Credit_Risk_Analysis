# Credit_Risk_Analysis

## Overview of Project
The purpose of this project is to use LendingClub data on borrowers to predict if a loan is approved or declined. We use supervised machine learning in python to conduct the analysis. The data was oversampled using RandomOverSampler and SMOTE. We also undersampled using ClusterCentroids and SMOTEENN. The BalancedRandomForestClassifier and EasyEnsembleClassifier were used to predict credit risk of borrowers.

## Results
The RandomOverSampler has an accuracy score of 64%. The high-risk precision and recall values are 1% and 69%. The low-risk precision and recall values are 100% and 59%.
![pic1](https://user-images.githubusercontent.com/103381098/183312433-9c13973a-d90a-4fd6-b796-2c6b3236e9e1.png)

SMOTE oversampling has an accuracy score of 66%. The high-risk precision and recall values are 1% and 63%. The low-risk precision and recall values are 100% and 69%.
![pic2](https://user-images.githubusercontent.com/103381098/183312440-107aaba0-21cb-4b5e-be0e-17a469168327.png)

ClusterCentroids undersampling has an accuracy score of 54%. The high-risk precision and recall values are 1% and 69%. The low-risk precision and recall values are 100% and 40%.
![pic3](https://user-images.githubusercontent.com/103381098/183312447-dd05e798-1970-4f21-b2f6-354f54817e4a.png)

SMOTEENN combination has an accuracy score of 64%. The high-risk precision and recall values are 1% and 70%. The low-risk precision and recall values are 100% and 57%.
![pic4](https://user-images.githubusercontent.com/103381098/183312452-aba58351-87ec-46a8-aed3-9b3baa367008.png)

## Summary
All the different supervised machine learning models are weak in predicting the precision of high-risk credit but, precision for low-risk borrowers is very high. Undersampling generated the lowest f1 score and I wouldn’t recommend using this one. The EasyEnsembleClassifier has the best results with stronger recall values for both high and low risk. Despite this being the strongest model used it still has a weak F1 score. I wouldn’t recommend using any of the supervised machine learning models for accessing high credit risk. It is however good at identifying low credit risk although this isn't very helpful on its own.
