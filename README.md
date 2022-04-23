# Credit_Risk_Analysis
## Overview of the analysis
`Imbalanced-learn` and `scikit-learn` libraries were used to build and evaluate models using resampling techniques. The credit card credit dataset used in this analysis was provided by a peer-to-peer services lending company called LendingClub. Various data sampling techniques were performed using the following algorithms with its respective sampling technique indicated: `RandomOverSampler` (oversampling), `SMOTE` (oversampling), `ClusterCentroids` (undersampling), and `SMOTEENN` (combination of over and undersampling). Then two new machine learning models intended to predict credit risk with reduced bias called, `BalancedRandomForestClassifier` and `EasyEnsembleClassifier`, were compared.

## Results
Below are the results of the **balanced accuracy scores** and the **precision and recall scores** of all six machine learning models. 

- `RandomOverSampler`
  - Accuracy Score: 63.7%
  <br />
    <p align="center">
      <img width="425" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/Randomoversamp_accuracy.png">  
    </p>
  <br />
  
    - **High Risk**
    ```
    - Precision: 1.0%
    - Recall: 62.0%
    ```  
    - **Low Risk**
    ```
    - Precision: 100.0%
    - Recall: 65.0% 
    ```
    - **Avg/Total**
    ```
    - Precision: 99.0%
    - Recall: 65.0% 
    ```
    <p align="center">
      <img width="600" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/Randomoversamp_report.png">  
    </p>
   <br />
------

- `SMOTE`
  - Accuracy: 63.0%
   <br />
    <p align="center">
      <img width="355" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/SMOTE_accuracy.png">
    </p>
   <br />
  
    - **High Risk**
    ```
    - Precision: 1.0%
    - Recall: 62.0%
    ```  
    - **Low Risk**
    ```
    - Precision: 100.0%
    - Recall: 64.0%
    ```
    - **Avg/Total**
    ```
    - Precision: 99.0%
    - Recall: 64.0% 
    ```
    
    <p align="center">
     <img width="600" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/SMOTE_samp_report.png">
    </p>
   <br />
    
    
------

- `ClusterCentroids`
  - Accuracy: 51.6%
    <br />
    <p align="center">
      <img width="355" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids_accuracy.png">
    </p>
   <br />
   
    - **High Risk**
    ```
    - Precision: 1.0%
    - Recall: 60%
    ```  
    - **Low Risk**
    ```
    - Precision: 100.0%
    - Recall: 43.0%
    ```
    - **Avg/Total**
    ```
    - Precision: 99.0%
    - Recall: 44.0% 
    ```
    <p align="center">
     <img width="600" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids_samp_report.png">
    </p>
   <br />
    
------

- `SMOTEENN`
  - Accuracy: 62.5%
    <br />
    <p align="center">
      <img width="355" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN_accuracy.png">
    </p>
   <br />
  
    - **High Risk**
    ```
    - Precision: 1.0%
    - Recall: 71.0% 
    ```  
    - **Low Risk**
    ```
    - Precision: 99.0%
    - Recall: 54.0%
    ```
    - **Avg/Total**
    ```
    - Precision: 99.0%
    - Recall: 54.0% 
    ```
    <p align="center">
     <img width="600" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN_samp_report.png">
    </p>
   <br />
------ 
 
- `Balanced Random Forest Classifer`
  - Accuracy: 78.9%
    <br />
    <p align="center">
     <img width="355" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/Balanced_accuracy.png">
    </p>
   <br />
   
    - **High Risk**
    ```
    - Precision: 3.0%
    - Recall: 70.0%
    ```  
    - **Low Risk**
    ```
    - Precision: 100.0%
    - Recall: 87.0%
    ```
    - **Avg/Total**
    ```
    - Precision: 99.0 %
    - Recall: 87.0 % 
    ```
    <p align="center">
     <img width="600" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/Balanced_samp_report.png">
    </p>
   <br />
------

- `Easy Ensemble Classifer`
  - Accuracy: 93.2%
    <br />
    <p align="center">
      <img width="355" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/Easy_accuracy.png">  
    </p>
  <br />
  
    - **High Risk**
    ```
    - Precision: 9.0%
    - Recall: 92.0%
    ```  
    - **Low Risk**
    ```
    - Precision: 99.0%
    - Recall: 94.0% 
    ```
    - **Avg/Total**
    ```
    - Precision: 99.0 %
    - Recall: 94.0 % 
    ```
     <p align="center">
     <img width="600" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/Easy_samp_report.png">
    </p>
   <br />

-------

## Summary
The `RandomOverSampler`, `SMOTE`, `ClusterCentroids`, and `SMOTEENN` yielded moderately strong accuracy and F-1 scores, but not at a high enough score where they are recommended to be used to accurately predict for credit card credit risk.

The `Balanced Random Forest Classifer` yielded a much higher accuracy score (78.9%) than the previous 4 models discussed along with a very strong F-1 score (93%). Out of the 5 models discussed so far, this is the strongest prediction model.

However, the `Easy Ensemble Classifer` model yielded the highest accuracy score (93.2%), percentages in average precision (99%.0) and recall (94%). In addiiton, its F1-score (97.0%) was the highest out of all the models. These values support the accuracy of the model and its strong accurate potential to identify high risk applicants who are applying for a loan. Out of the 6 models, this is the recommended model to use to accurately predict credit card credit risk applicants with confidence.




