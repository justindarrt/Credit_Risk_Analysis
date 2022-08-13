# Credit_Risk_Analysis

## Overview of Project
The purpose of this project is to use LendingClub data on borrowers to predict if a loan is approved or declined. We use supervised machine learning in python to conduct the analysis. The data was oversampled using RandomOverSampler and SMOTE. We also undersampled using ClusterCentroids and SMOTEENN. The BalancedRandomForestClassifier and EasyEnsembleClassifier were used to predict credit risk of borrowers.

## Results
### RandomOverSampler 
* Accuracy score: 64%
* Precision values: high 1% and low 100%
* Recall values: high 69% and low 59%
![pic1](https://user-images.githubusercontent.com/103381098/183312433-9c13973a-d90a-4fd6-b796-2c6b3236e9e1.png)

### SMOTE 
* Accuracy score: 66%
* Precision values: high 1% and low 100%
* Recall values: high 63% and low 69%
![pic2](https://user-images.githubusercontent.com/103381098/183312440-107aaba0-21cb-4b5e-be0e-17a469168327.png)

### ClusterCentroids 
* Accuracy score: 54%
* Precision values: high 1% and low 100%
* Recall values: high 69% and low 40%
![pic3](https://user-images.githubusercontent.com/103381098/183312447-dd05e798-1970-4f21-b2f6-354f54817e4a.png)

### SMOTEENN Combination 
* Accuracy score: 64%
* Precision values: high 1% and low 100%
* Recall values: high 70% and low 57%
![pic4](https://user-images.githubusercontent.com/103381098/183312452-aba58351-87ec-46a8-aed3-9b3baa367008.png)

### BalancedRandomForestClassifier
* Accuracy score: 79%
* Precision values: high 3% and low 100%
* Recall values: high 70% and low 87%
![pic5](https://user-images.githubusercontent.com/103381098/184502188-b99e1137-e958-41a4-9e2d-b826b7c98dd1.png)

### EasyEnsembleClassifier
* Accuracy score: 93%
* Precision values: high 9% and low 100%
* Recall values: high 92% and low 94%
![pic6](https://user-images.githubusercontent.com/103381098/184502229-18e0b1e8-b6c8-4960-9cb7-b1fd7bc1abee.png)


## Summary
All the different supervised machine learning models are weak in predicting the precision of high-risk credit but, precision for low-risk borrowers is very high. Undersampling generated the lowest f1 score and I wouldn’t recommend using this one. The EasyEnsembleClassifier has the best results with stronger recall values for both high and low risk. Despite this being the strongest model used it still has a weak F1 score. I wouldn’t recommend using any of the supervised machine learning models for accessing high credit risk. It is however good at identifying low credit risk although this isn't very helpful on its own.
