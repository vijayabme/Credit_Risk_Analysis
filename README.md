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
- The precision is still very low for the high risk category.
- The recall dropped quite a bit with high risk at 0.69 and low risk at 0.40.
![image](https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/Cluster_centroids_undersampling.png)
##### SMOTEENN
- With SMOTEENN the accuracy dropped compared to SMOTE and random over sampler.
- The precision is similar to the other oversampling methods at 0.01 and 1.00.
- The recall is low for low-risk at 0.57
![image](https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/Combination_Sampling.png)
#### Ensemble Classifiers to predict credit risk
##### BalancedRandomForestClassifier 
- The accuracy is 0.78 which is an improvement from all the oversampling and undersampling techniques used above.
- The precision for high risk is still low at 0.03
- The recall for the high-risk is 0.70 and low-risk is 0.86 which are slightly better
![image](https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/Balanced_RFC.png)
##### EasyEnsembleClassifier
- The Easy ensemble ADA boost has the best accuracy so far at 0.93
- The precision for high-risk is also the highest compared to other techniques at 0.09
- The recall is high for both high categories.
- The f1 score is also higher compared to other techniques above at 0.16
![image](https://github.com/vijayabme/Credit_Risk_Analysis/blob/main/Resources/EasyEnsemble_ADABoost.png)
## Summary
 - Of all the machine learning models the ADA boost had the highest accuracy and had a higher recall and precision for the high risk loans
 - The precision is still low at 0.09 which is not enough to predict the high credit risk accurately.
 - So none of these machine learning algorithms are giving good results.
 - We would have to look at the feature importance and remove some of the less important features and try again to get a better precision and accuracy.
