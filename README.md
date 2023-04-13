# Credit Risk Analysis


## Overview of the analysis
The purpose of this analysis to to evaluate different machine learning modesl to predict credit risk. This analysis was performed using a credit card dataset from LendingClub. In this analysis, we
- oversampled the data using the RandomOverSampler and SMOTE algorithms
- undersampled the data using the ClusterCentroids algorithm
- used a combination approach of oversampling and undersampling using the SMOTEENN algorithm
- compared two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk


## Results
In our results, we are checking the balanced accuracy score, the precision, or positive predictive value, score, and the recall, or sensitivity, score.

#### RandomOverSampler Model
- The balanced accuracy score is 63
- The precision score is 1
- The recall score is 68

![RandomOverSampler](https://github.com/amiecostello22/Credit_Risk_Analysis/blob/main/Images/RandomOverSampler%20Model.png)

#### SMOTE Model
- The balanced accuracy score is 63
- The precision score is 1
- The recall score is 63

![SMOTE](https://github.com/amiecostello22/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Model.png)

#### ClusterCentroids Model
- The balanced accuracy score is 51
- The precision score is 1
- The recall score is 43

![ClusterCentroids](https://github.com/amiecostello22/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids%20Model.png)

#### SMOTEENN Model
- The balanced accuracy score is 62
- The precision score is 1
- The recall score is 54

![SMOTEENN](https://github.com/amiecostello22/Credit_Risk_Analysis/blob/main/Images/SMOTEENN.png)

#### BalancedRandomForestClassifier Model
- The balanced accuracy score is 79
- The precision score is 1
- The recall score is 91

![BalancedRandomForestClassifier](https://github.com/amiecostello22/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForestClassifier.png)

#### EasyEnsembleClassifier Model
- The balanced accuracy score is 93
- The precision score is 1
- The recall score is 94

![EasyEnsemble](https://github.com/amiecostello22/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleClassifier.png)


## Summary
All six of the models yielded a low precision score when we determine a high credit risk. However, the EasyEnsembleClassifier Model and the BalancedRandomForestClassifier Model had a much higher sensistivity in detecting high risk applicants as opposed to the other four models. Still, because of the consecutive low precision scores, I would not necessarily recommend any of these models for the bank to use to predict accurate credit risk of the applicants.
