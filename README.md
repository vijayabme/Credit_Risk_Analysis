# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis
Build and evaluate several machine learning models to predict credit risk.
## Results
#### Resampling models to predict credit risk
##### Random Over sampler
- With Random over sampler the accuracy is low at 0.66
- The precision for high risk loans is still very low at 0.01 but for high risk loans its high at 1.00. This can also be seen in the f1 score which is low for high risk.
- The recall is higher for high risk loans compared to low risk.
![image](https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/Naive_Random_oversampling.png)
##### SMOTE
- With SMOTE the accuracy didnt improve from Random over sampling.
- The precision score is similar to random over sampler.
- The recall values are lower than the random over sampler. 
![image](https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/SMOTE_oversampling.png)
##### Cluster Centroids
- Under sampling is reducing the accuracy compared to over sampling. The accuracy dropped to 0.54
- The precision didnt change from oversampling.
- The recall dropped quite a bit with high risk at 0.69 and low risk at 0.40.
https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/Cluster_centroids_undersampling.png
##### SMOTEENN
- With SMOTEENN the accuracy dropped compared to SMOTE and random over sampler.
- The precision is similar to the other oversampling methods at 0.01 and 1.00.
![image](https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/Combination_Sampling.png)
#### Ensemble Classifiers to predict credit risk
##### BalancedRandomForestClassifier 

![image](https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/Balanced_RFC.png)
##### EasyEnsembleClassifier

![image](https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/EasyEnsemble_ADABoost.png)
## Summary
