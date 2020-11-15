# Credit_Risk_Analysis

## Purpose
The purpose of this analysis was to evaluate the performance of supervised machine learining models in predicting credit card risk. 

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
Balanced accuracy, precision and recall scores can be analyzed as follows: 
1. Accuracy
2. All precision scores for high risk creditors are low which means that there's a large number of false positives. On the other hand, all precision scores for low risk creditors are equal to 1 which means that there are no false positives. In other words, most creditors that are classified as high risk creditors are not high risk creditors, and all creditors that are classified as low risk creditors are in fact low risk creditors. 
3. 

ROS
                 pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.74      0.61      0.02      0.67      0.46       101
   low_risk       1.00      0.61      0.74      0.75      0.67      0.44     17104

avg / total       0.99      0.61      0.74      0.75      0.67      0.44     17205


SMOTE
                 pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.63      0.69      0.02      0.66      0.44       101
   low_risk       1.00      0.69      0.63      0.82      0.66      0.44     17104

avg / total       0.99      0.69      0.63      0.81      0.66      0.44     17205



low precision = large number of false positives 
Recall is the ability of the classifier to find all the positive samples. A low recall is indicative of a large number of false negatives
