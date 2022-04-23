# Credit_Risk_Analysis
## Overview of the analysis
`Imbalanced-learn` and `scikit-learn` libraries were used to build and evaluate models using resampling techniques. The credit card credit dataset used in this analysis was provided by a peer-to-peer services lending company called LendingClub. Various data sampling techniques were performed using the following algorithms with its respective sampling technique indicated: `RandomOverSampler` (oversampling), `SMOTE` (oversampling), `ClusterCentroids` (undersampling), and `SMOTEENN` (combination of over and undersampling). Then two new machine learning models intended to predict credit risk with reduced bias called, `BalancedRandomForestClassifier` and `EasyEnsembleClassifier`, were compared.

## Results
Below are the results of the **balanced accuracy scores** and the **precision and recall scores** of all six machine learning models. 

- `RandomOverSampler`
  - Accuracy Score: 63.7%
  <br />
    <p align="center">
      <img width="355" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/Randomoversamp_accuracy.png">  
    </p>
  <br />
  
    - **High Risk**
    ```
    - Precision: 1.0%
    - Recall: 62.0%
    ```  
    - **Low Risk**
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
    - Precision: 99.0%
    - Recall: 43.0%
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
    <p align="center">
     <img width="600" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN_samp_report.png">
    </p>
   <br/>
------ 
 
- `Balanced Random Forest Classifer`
  - Accuracy:
   <br />
    <p align="center">
      <img width="355" alt="image" src=""https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/Balanced_accuracy.png>
    </p>
   <br />
   
    - **High Risk**
    ```
    - Precision
    - Recall
    ```  
    - **Low Risk**
    ```
    - Precision
    - Recall
    ```
    <p align="center">
     <img width="600" alt="image" src="https://github.com/jwhberrios/Credit_Risk_Analysis/blob/main/Resources/Balanced_samp_report.png">
    </p>
   <br />
------

- `Easy Ensemble Classifer`
  - Accuracy:
    - **High Risk**
    ```
    - Precision
    - Recall
    ```  
    - **Low Risk**
    ```
    - Precision
    - Recall
    ```
-------

## Summary



