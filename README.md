# Credit_Risk_Analysis
## Overview
The purpose of this project is to train and evaluate models that predict credit risk using data from LendingClub. Three different approaches and a total of 6 models will be attempted and compared:
  1. Resampling Models 
  3. SMOTEENN Algorithm
  4. Ensemble Classifiers

## Resources
- Data: [LoanStats_2019Q1.csv and Salary_Data.csv](https://github.com/mcarson16/Credit_Risk_Analysis/blob/main/Resources.zip)
- Software: Jupyter Notebooks

## Results

### Resampling Models
- #### Naive Random Oversampling
  - Balanced Accuracy Score: 65%
  - High Risk Precision Score: 0.01
  - Low Risk Precision Score: 1.00
  - Recall Score Difference: 0.02  
  - ![image](https://user-images.githubusercontent.com/83254435/133009827-f67e21fe-90be-458e-ab9c-0e5d09b8d85f.png)

- #### SMOTE Oversampling
  - Balanced Accuracy Score: 62%
  - High Risk Precision Score: 0.01
  - Low Risk Precision Score: 1.00
  - Recall Score Difference: 0.16
  - ![image](https://user-images.githubusercontent.com/83254435/133009850-4e0c7850-16f9-4be6-bed1-1481c830c44b.png)

- #### ClusterCentroids Resampling
  - Balanced Accuracy Score: 52%
  - High Risk Precision Score: 0.01
  - Low Risk Precision Score: 1.00
  - Recall Score Difference: 0.13
  - ![image](https://user-images.githubusercontent.com/83254435/133009905-9e8b8029-5b09-43a1-833f-ac6d6101828c.png)

### SMOTEENN Algorithm
  - Balanced Accuracy Score: 65%
  - High Risk Precision Score: 0.01
  - Low Risk Precision Score: 1.00
  - Recall Score Difference: 0.18
  - ![image](https://user-images.githubusercontent.com/83254435/133010002-5b3e1fe3-015a-4cc3-bb6f-8bd91de99d55.png)

### Ensemble Classifiers
- #### Balanced Random Forest Classifier
  - Balanced Accuracy Score: 79%
  - High Risk Precision Score: 0.03
  - Low Risk Precision Score: 1.00
  - Recall Score Difference: 0.17
  - ![image](https://user-images.githubusercontent.com/83254435/133010134-13e7d4e8-cfcb-4bed-936e-9a6f35db4a80.png)

- #### Easy Ensemble AdaBoost Classifier
  - Balanced Accuracy Score: 93%
  - High Risk Precision Score: 0.09
  - Low Risk Precision Score: 1.00
  - Recall Score Difference: 0.02
  - ![image](https://user-images.githubusercontent.com/83254435/133010174-85d9e39a-a82d-4e2a-9e83-12092551b9fc.png)

## Summary
Of the methods tested, the Easy Ensemble AdaBoost Classifier model has the highest balanced accuracy score at 93%. It also has one of the lowest Recall Score differences, at 0.02. The High Risk Precision score, though higher than the other models at 0.09, is still low. Additional modifications to the model may be required to generate accurate predictions for the High Risk classification.
