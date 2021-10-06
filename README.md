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

![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/RandomOverSampling_Results.png)
- This model may not be the best to predict credit risk due to accuracy and recall for high risk predictions both being below 65%.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/SMOTE_Results.png)
- This model may not be the best to predict credit risk due to accuracy and recall for high risk predictions both being below 67%.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/ClusterCentroidsUnderSample.png)
- This model may not be the best to predict credit risk due to accuracy level of 54%.  Although recall for high risk predictions is near 70%, it's still well below an acceptable level for most lenders.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/SMOTEENN_Results.png)
- This model may not be the best to predict credit risk due to accuracy level of 66%.  Although recall for high risk predictions is near 75%, it's still well below an acceptable level for most lenders.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/RandomForest_Results.png)
- This model may not be the best to predict credit risk due to accuracy and recall for high risk predictions both being below 80%.  With that said, some aggressive lenders may accept these results.  Further explanation on why a high recall for high risk predictions is important can be found in the summary below.

![image](https://github.com/sbretag/Credit_Risk_Analysis/blob/main/Images/EEC_Results.png)
- Given this model has a 93% accuracy level along with 92% recall level for high risk predictions, this should be acceptable for most lenders.   Further explanation on why a high recall for high risk predictions is important can be found in the summary below.


## Summary
- In the case of credit risk analysis, the majority of the time the lender will want to remain conservative when it comes to risk.  Mistakes in assessing credit risk could cost lenders hundreds of thousands if not millions of dollars.  In extreme examples, misevaluating risk can lead to global recessions like what we saw during the mortgage crisis in the late 2000's and early 2010's.  Therefore, we would want to have a model that is not only accurate, but has a high degree of sensitivity (recall) versus precision when it comes to predicting high risk.  In other words, predicting that a borrower is high risk when they are actually not is not the end of the world, generally this leads to further analysis into the borrower before making any final decision.
- Overall the resampling models (Random Oversampling, SMOTE, Cluster Centroids, and SMOOTEN) all had relatively low accuracy and high risk prediction sentivity levels.  Generally speaking, they would not meet lender expectations.  The ensemble models (Random Forest & Esemble Adaboost) accuracy and high risk prediction sensitivty levels were both relatively higher.  Of the two, the Ensemble Adaboost Classifier algorithm produced the best results and would meet most if not all lender expectations when it comes to evaluating risk.



