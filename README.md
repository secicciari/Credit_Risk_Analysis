# Credit_Risk_Analysis

##Project Overview
### Purpose
I've been asked to utilize Tableau to create visualizations that we can present to investors in order to show them that a bike-sharing program in Des Moines is a solid business proposal. I completed the analysis using August Citi Bike data from New York City in order to get a better understanding of what a bike-sharing program in Des Moines might look like.

## Results
### RandomOversampler
![RandomOversampler](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/resources/RandomOversampler.PNG)
- Balanced Accuracy: 0.66
- Precision: 0.01 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.74 when predicting high_risk, 0.58 when predicting low_risk

### SMOTE
![SMOTE](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/resources/RandomOversampler.PNG)
- Balanced Accuracy: 0.65
- Precision: 0.01 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.62 when predicting high_risk, 0.68 when predicting low_risk

### ClusterCentroids
![ClusterCentroids](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/resources/RandomOversampler.PNG)
- Balanced Accuracy: 0.54
- Precision: 0.01 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.69 when predicting high_risk, 0.40 when predicting low_risk

### SMOTEENN
![SMOTEENN](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/resources/RandomOversampler.PNG)
- Balanced Accuracy: 0.67
- Precision: 0.01 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.77 when predicting high_risk, 0.57 when predicting low_risk

### Balanced RandomForestClassifer
![BalancedRandomForestClassifer](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/resources/RandomOversampler.PNG)
- Balanced Accuracy: .77
- Precision: 0.03 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.64 when predicting high_risk, 0.89 when predicting low_risk

### EasyEnsembleClassifier
![EasyEnsembleClassifier](https://github.com/secicciari/Credit_Risk_Analysis/blob/main/resources/RandomOversampler.PNG)
- Balanced Accuracy: 0.93
- Precision: 0.09 when predicting high_risk, 1.00 when predicting low_risk
- Recall: 0.92 when predicting high_risk, 0.94 when predicting low_risk

## Summary

