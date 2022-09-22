# Credit_Risk_Analysis

## Overview 
Python was used to build and evaluate multiple learning models to predict credit risk. We did this by using the following techniques:
*Oversampling the data with the RandomOverSampler and SMOTE algorithms
*Undersampling the data with the ClusterCentroids algorithm
*Using a combinatorial approach of over/undersampling using the SMOTEENN algorithm
*Compare two bias reducing machine learning models - BalancedRandomForestClassifier and EasyEnsembleClassifier

## Results

### RandomOverSampler 
The balanced accuracy score was 65%. The high_risk precision was ~1% with a sensitivity of 62%. F1 of 2%. Due to the high number of the low_risk population, the precision is nearly 100% with a sensitivity of 68%.

![image](https://user-images.githubusercontent.com/106290364/191669081-b46c1c47-2cd7-4247-be5b-2580026d2d39.png)


### SMOTE model
The balanced accuracy score was 64%. The high_risk precision was ~1% with a sensitivity of 63%. F1 of 2%. Due to the high number of the low_risk population, the precision is nearly 100% with a sensitivity of 66%.

![image](https://user-images.githubusercontent.com/106290364/191669174-7b8924fa-553c-4106-88a5-7353b2c8a0e5.png)


### ClusterCentroids model
The balanced accuracy score was 52%. The high_risk precision was ~1% with a sensitivity of 63%. F1 of 1%. Due to the high number of false positives, the low_risk population is 40%. 

![image](https://user-images.githubusercontent.com/106290364/191669244-d15141f0-3158-43ef-a1dd-8302cdf252b7.png)


### SMOTEENN model
The balanced accuracy score was 62%. The high_risk precision was ~1% with a sensitivity of 68%. F1 of 2%. Due to the high number of false positives, the low_risk population is 57%. 

![image](https://user-images.githubusercontent.com/106290364/191669315-b970709d-f003-4953-ba43-5a790ba65347.png)


### BalancedRandomForestClassifier model
The balanced accuracy score was 79%. The high_risk precision was 4% with a sensitivity of 67%. F1 of 7%. The low_risk population is 91% with 100% precision. 

![image](https://user-images.githubusercontent.com/106290364/191669384-b713e847-ebb2-4231-a090-c22811484444.png)


### EasyEnsembleClassifier model
The balanced accuracy score was 93%. The high_risk precision was 7% with a sensitivity of 91%. F1 of 14%. The low_risk population is 94% with 100% precision. 

![image](https://user-images.githubusercontent.com/106290364/191669448-a087774b-de12-46bb-8435-8fbcd8b781a2.png)


## Summary
After using all six machine learning models, the EasyEnsembleClassifer model yielded the best results with an accuracy rate of 93% and a 9% precision rate when predicting "High Risk candidates. The sensitivity rate was also the highest compared to the other models. The result for predicting "Low Risk" were also the highest with the sensitivity rate of 94% and an F1 score of 97%. This would make the EasyEnsembleClassifer model the best choice when predicting credit risk. 
