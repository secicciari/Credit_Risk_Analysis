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

### BalancedRandomForestClassifer
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
In summary, all six models lack precision when it comes to identifying high risk accounts. This is not surprising, since there are significantly fewer low risk accounts than high risk accounts in the data set, however low precision would be problematic in this case. Across all six models, we see that many of the accounts that the model flags as high risk are not actually high risk, which can cause frustration and confusion for account holders and extra work for bank employees. However, both of the ensemble models performed better than the over, under, and combination sampling models in terms of precision and balanced accuracy.

I would not recommend using any of these models to predict credit risk because of the low precision. That being said, if I had to choose one of the six, the best option is the EasyEnsembleClassifier model. Of the six models I tested, this model had the best precision and recall across both classes (low risk and high risk). Although the precision for high risk is still very low, the recall score shows that 92% of actual high risk cases are detected correctly, which is important in flagging accounts. You can be confident that most of the high risk cases would be correctly identified. Also, in cases of unbalanced classification like we have here, the balanced accuracy metric is really important in evaluating a model's performance. The EEC model has a balanced accuracy of 93%, which is the highest accuracy score across all six models that were tested. However, the low precision rate shows us that  If you chooose to move forward with this model, I would recommend reducing the number of features to see if that improves the quality of the model.
