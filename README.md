# Credit_Risk_Analysis

## Overview
Use a credit card credit dataset from LendingClub, a peer to peer lending services company, we've been tasked to utilize machine learning models to predict credit risk and produce an evaluation of the model performance with including recommendations.  The following deliverables are required.
  - Use resampling models to predict credit risk
  - Use SMOTEENN algorithm to predict credit risk
  - Use ensemble classifiers to predict credit risk
  - Produce a written report on the credit risk analysis

## Resouces

  - Software
    - Python (Machine Learning Environment)
    - Jupyter Lab
  - Source Data
    - [Loan Data](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Resources/LoanStats_2019Q1.csv)
  - Ipynb Notebooks
    - [Resampling Ipynb](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Notebooks/credit_risk_resampling.ipynb)
    - [Ensemble Ipynb](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Notebooks/credit_risk_ensemble.ipynb)

## Results

### Random Oversampling
![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/RandomOverSampling_Results.png)
- This model may not be the best to predict credit risk due to accuracy and recall for high risk predictions both being below 65%.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

### SMOTE
![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/SMOTE_Results.png)
- This model may not be the best to predict credit risk due to accuracy and recall for high risk predictions both being below 67%.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

### Cluster Centroids Undersampling
![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/ClusterCentroidsUnderSample.png)
- This model may not be the best to predict credit risk due to accuracy level of 54%.  Although recall for high risk predictions is near 70%, it's still well below an acceptable level for most lenders.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

### SMOTEENN
![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/SMOTEENN_Results.png)
- This model may not be the best to predict credit risk due to accuracy level of 66%.  Although recall for high risk predictions is near 75%, it's still well below an acceptable level for most lenders.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

### Random Forest
![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/RandomForest_Results.png)
- This model may not be the best to predict credit risk due to accuracy and recall for high risk predictions both being below 80%.  With that said, some aggressive lenders may accept these results.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

### EEC
![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/EEC_Results.png)
- Given this model has a 93% accuracy level along with 92% recall level for high risk predictions, this should be acceptable for most lenders.   Further explanation on why a high recall for high risk predictions is important can be found in the summary below.


## Summary
- Summarize the results of the machine learning models, and include a recommendation on the model to use, if any.  If you do not recommend any of the models, justify your reasoning.


LINK HELP
    - [Style.css](https://github.com/sbretag/Mapping_Earthquakes/blob/main/Earthquake_Challenge/static/css/style.css)
![image](https://github.com/sbretag/Mapping_Earthquakes/blob/main/Earthquake_Challenge/Images/Map_Options.png)
