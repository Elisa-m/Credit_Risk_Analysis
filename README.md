# Credit_Risk_Analysis

## Purpose
The purpose of this analysis was to evaluate the performance of supervised machine learining models in predicting credit risk to identify which accoutns should be given loans. 

## Results
### Model #1: RandomOverSampler
1. Balanced accuracy score: 0.6742571941946299
2. Precision and recall scores:

![](ros.png)

### Model #2: SMOTE Oversampling
1. Balanced accuracy score: 0.6623356588465208
2. Precision and recall scores:

![](smote.png)

### Model #3: ClusterCentroids Undersampling
1. Balanced accuracy score: 0.544392082449592
2. Precision and recall scores:

![](cc.png)

### Model #4: SMOTEENN Over and Under Sampling
1. Balanced accuracy score: 0.6447701423556762
2. Precision and recall scores: 

![](smoteen.png)

### Model #5: Balanced Random Forest Classifier
1. Balanced accuracy score: 0.7885466545953005
2. Precision and recall scores:

![](brf.png)

### Model #6: Easy Ensemble AdaBoost Classifier
1. Balanced accuracy score: 0.9316600714093861
2. Precision and recall scores:

![](ecc.png)

## Summary
All low credit risk precision scores are 1 which means that all models are 100% reliable at predicting low credit risk. In other words, there's a 100% chance that all accounts classified as low credit risk have low credit risk. However, all precision scores for high credit risk are low which means that most accounts that are classified as having high credit risk do not have high credit risk. No matter the model used, all loans given will go to accounts with low credit risk, yet many low credit risk accounts will be denied access to loans. 

Our biggest concern with these models is the high number of accounts with low credit risk that will be denied loans. Therefore, we would want to use a model with high recall scores for low credit risk which would indicate that most accounts being denied loans have high credit risk and should be denied loans. The model with the highest recall score for low credit risk is Model #6 with a recall score of 0.94. This means that 94% of accounts who have low credit risk were correctly assigned to having low credit risk.  
