# Credit_Risk_Analysis

## Overview:
In this project, we are using Python and multiple supervised machine learning models to predict credit risk. 

The following machine learning models were evaluated in this process:
* Oversampling: RandomOverSampler and SMOTE algorithms
* Undersampling: Cluster Centroids algorithm
* Combination approach of over and undersampling: SMOTEENN algorithm.
* Comparing machine learning models that reduce bias: Balanced Random Forest Classifier and Easy Ensemble Classifier.

## Results:
### RandomOverSampler Algorithm Results:
<img width="773" alt="randomoversampler" src="https://user-images.githubusercontent.com/103595718/188203090-a1b4fcee-e3f2-4584-9fdf-942e3e7e8fce.png">

* The balanced accuracy score is 64%.
* High_risk category: 1% precision and 66% recall score
* Low-risk category: 100% precision and 62% recall score

### SMOTE Algorithm Results:
<img width="751" alt="smoteoversampling" src="https://user-images.githubusercontent.com/103595718/188203132-ea588327-a515-4387-a55a-6e14879546f0.png">

* The balanced accuracy score is 65%.
* High_risk category: 1% precision and 61% recall score
* Low-risk category: 100% precision and 69% recall score

### Cluster Centroids Algorithm Results:
<img width="760" alt="clustercentroidsundersampling" src="https://user-images.githubusercontent.com/103595718/188203163-6a00e9f2-8aa1-456e-b196-5a8817f07a4b.png">

* The balanced accuracy score is 54%.
* High_risk category: 1% precision and 69% recall score
* Low-risk category: 100% precision and 40% recall score

### SMOTEENN Algorithm Results: 
<img width="731" alt="smoteenn" src="https://user-images.githubusercontent.com/103595718/188203147-84f128d3-af88-48b2-a16d-7e8a38a13548.png">

* The balanced accuracy score is 64%.
* High_risk category: 1% precision and 72% recall score
* Low-risk category: 100% precision and 52% recall score

### BalancedRandomForestClassifies Results: 
<img width="730" alt="balancedrandomforest" src="https://user-images.githubusercontent.com/103595718/188203185-663cd88a-66e0-4e1a-b19d-4db5b4318179.png">

* The balanced accuracy score is 68%.
* High_risk category: 88% precision and 37% recall score
* Low-risk category: 100% precision and 100% recall score

### EasyEnsemble Results: 
<img width="728" alt="easyensemble" src="https://user-images.githubusercontent.com/103595718/188203197-7dd5b7a3-7076-4342-9c96-d8edd95326e8.png">

* The balanced accuracy score is 93%.
* High_risk category: 9% precision and 92% recall score
* Low-risk category: 100% precision and 94% recall score


## Summary:
All of the models used show weak precision in determining if there is high credit risk. The ensemble (balanced random forest and easy ensemble) models were overall better due to higher accuracy and precision than the other models. The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit. With low precision in this model, a lot of low risk credits are still falsely detected as high risk. In this aspect, the balanced random forest model has higher recall for the high risk category if the bank is seeking to increase their number/revenue by approving more credit to customers that would be otherwise labeled as high-risk. Overall, I would suggest that the company uses the Balanced Random Forest Algorithm for predicting credit risk.
