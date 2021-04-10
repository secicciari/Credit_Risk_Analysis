# Credit_Risk_Analysis

## Project Overview
### Purpose
I've been asked to use a credit card credit dataset from LendingClub to test the performance of different models to recommend whether any of them should be used to predict credit risk. I will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Finally, I'l compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results
### RandomOversampler
![RandomOversampler](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/Resources/RandomOversampler.PNG)
- Balanced Accuracy: 0.66
- Precision: 0.01 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.74 when predicting high_risk, 0.58 when predicting low_risk

### SMOTE
![SMOTE](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/Resources/RandomOversampler.PNG)
- Balanced Accuracy: 0.65
- Precision: 0.01 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.62 when predicting high_risk, 0.68 when predicting low_risk

### ClusterCentroids
![ClusterCentroids](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids.PNG)
- Balanced Accuracy: 0.54
- Precision: 0.01 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.69 when predicting high_risk, 0.40 when predicting low_risk

### SMOTEENN
![SMOTEENN](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN.PNG)
- Balanced Accuracy: 0.67
- Precision: 0.01 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.77 when predicting high_risk, 0.57 when predicting low_risk

### Balanced RandomForestClassifer
![BalancedRandomForestClassifer](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForestClassifier.PNG)
- Balanced Accuracy: .77
- Precision: 0.03 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.64 when predicting high_risk, 0.89 when predicting low_risk

### EasyEnsembleClassifier
![EasyEnsembleClassifier](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier.PNG)
- Balanced Accuracy: 0.93
- Precision: 0.09 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.92 when predicting high_risk, 0.94 when predicting low_risk

## Summary
In cases of unbalanced classification like we have here, the balanced accuracy metric is really important in evaluating a model's performance. I would recommend using the EasyEnsembleClassifier model to predict credit risk. Of the six models I tested, this model had the best precision and recall across both classes (low risk and high risk). Although the precision for high risk is still very low, the recall score shows that 92% of actual high risk cases are detected correctly, which is important in flagging accounts.
