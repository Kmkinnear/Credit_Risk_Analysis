# Credit_Risk_Analysis

## Overview

The overview of this analysis was to use multiple machine learning models to train and evaluate models related to our Credit Risk Analysis. We did this by using the "imbalanced-learn" and "scikit-learn" libraries to build and evaluate our models using resampling.  We used "RandomOverSampler" and "SMOTE" to oversample our data and used the "ClusterCentroids" algorithm to undersample the data. After that we used the "SMOTEENN" algorithm to use a combination of approaches through over- and undersampling the data. Finally, we will compare two more models aimed at reducing bias, "BalancedRandomForestClassifier" and "EasyEnsembleClassifier" to try and predict credit risk for our analysis. Once we have run our different models, we will be able to make a recommendation on whether or not this is a reliable approach to predict credit risk.

## Results

### 1. Naive Random Oversampling

![image](https://user-images.githubusercontent.com/110848660/213277645-aa5c85e0-0f6c-41c8-b1af-32083bf03901.png)

- This model has a balanced accuracy score of 64.5%. 
- The precision for the high-risk loans was 1% and the precision for the low-risk loans was 100%. 
- The recall values for the high-risk loans was 62% and the low-risk loans was 67%.

### 2. SMOTE Oversampling

![image](https://user-images.githubusercontent.com/110848660/213277765-d7d6bd65-24dc-489e-a234-e2cdaf7d6264.png)

- This model has a balanced accuracy score of 66.3%. 
- The precision for the high-risk loans was 1% and the precision for the low-risk loans was 100%. 
- The recall values for the high-risk loans was 63% and the low-risk loans was 69%.

### 3. Undersampling

![image](https://user-images.githubusercontent.com/110848660/213277901-bb0eef20-f2dd-4c57-bae1-e5d27317d44c.png)

- This model has a balanced accuracy score of 66.3%. 
- The precision for the high-risk loans was 1% and the precision for the low-risk loans was 100%. 
- The recall values for the high-risk loans was 69% and the low-risk loans was 40%.
 
### 4. Combination (Over and Under) Sampling

![image](https://user-images.githubusercontent.com/110848660/213278026-28e0029d-bfa0-4b8f-97e4-a24685a11621.png)

- This model has a balanced accuracy score of 54.5%. 
- The precision for the high-risk loans was 1% and the precision for the low-risk loans was 100%. 
- The recall values for the high-risk loans was 76% and the low-risk loans was 59%.

### 5. Balanced Random Forest Classifier

![image](https://user-images.githubusercontent.com/110848660/213278183-87098b36-2e89-49f0-aceb-380bb06166f2.png)

- This model has a balanced accuracy score of 78.9%. 
- The precision for the high-risk loans was 3% and the precision for the low-risk loans was 100%. 
- The recall values for the high-risk loans was 70% and the low-risk loans was 87%.
 
### 6. Easy Ensemble AdaBoost Classifier

![image](https://user-images.githubusercontent.com/110848660/213278284-597126e9-d0fa-4e78-9f85-10260a6fb4a0.png)

- This model has a balanced accuracy score of 93.2%. 
- The precision for the high-risk loans was 9% and the precision for the low-risk loans was 100%. 
- The recall values for the high-risk loans was 92% and the low-risk loans was 94%.

## Summary

![image](https://user-images.githubusercontent.com/110848660/213284706-505a0082-bef3-427b-9dab-5baa333ecea9.png)

All six of our models performed differently as you can see from the data above. We can see that our two Ensemble models performed better than our first four resampling models by providing the most balanced numbers. Specifically, the Easy Ensemble model produced the best results across the five measurements that we used. 

One downside of all the models is that they all produced a low percentage for precision with high-risk loans. We did not have any model that produced anything greater than 10%. I would recommend trying to come up with more data to use in our analysis to see if we can get the precision numbers up or explore using some different models that may be more precise in detecting risky loans.
