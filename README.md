# Credit Risk Analysis
## Overview of the project
This project is to analyze credit card credit dataset from LendingClub, a peer-to-peer lending services company by applying machine learning.

- Task 1: Use Resampling Models to Predict Credit Risk
- Task 2: Use the SMOTEENN Algorithm to Predict Credit Risk
- Task 3: Use Ensemble Classifiers to Predict Credit Risk

## Resources
- Data: LoanStats_2019Q1.csv
- Software: Jupyter Notebook

## Results
### Naive Oversampling    
- Accuracy score: 68.4% = (50+11710)/17205
- Precision: 1% (high risk), 100% (low risk)
- Recall: 57% (high risk), 58% (low risk)
<img width="485" alt="Naive_Oversampling" src="https://user-images.githubusercontent.com/85041697/155737513-a3a6f4ae-1e36-4137-9dd1-db99cf515c77.png">

### SMOTE Oversampling 
- Accuracy score: 63.5% = (54+10865)/17205
- Precision: 1% (high risk), 100% (low risk)
- Recall: 62% (high risk), 63% (low risk)
<img width="492" alt="SMETO" src="https://user-images.githubusercontent.com/85041697/155737554-b87f16c5-dc38-491f-82e9-15140eaf22b6.png">

### Undersampling
- Accuracy score: 57.1% = (53+9778)/17205
- Precision: 1% (high risk), 100% (low risk)
- Recall: 61% (high risk), 57% (low risk)
<img width="493" alt="Undersampling" src="https://user-images.githubusercontent.com/85041697/155737550-d0ff77dc-0b86-42de-b342-f2f2c2719fc6.png">

### Combination Sampling
- Accuracy score: 58.2% = (61+9948)/17205
- Precision: 1% (high risk), 100% (low risk)
- Recall: 70% (high risk), 58% (low risk)
<img width="502" alt="Combination" src="https://user-images.githubusercontent.com/85041697/155737569-1d33ef01-b0fa-4cdd-b4fe-8cdfe5438ee5.png">

### Balanced Random Forest Classifier 
- Accuracy score: 90.8% = (58+15558)/17205
- Precision: 4% (high risk), 100% (low risk)
- Recall: 67% (high risk), 91% (low risk)
<img width="496" alt="brfc" src="https://user-images.githubusercontent.com/85041697/155737661-79b227bc-ad6e-4a2e-9287-e2f1ab6b14ff.png">

### Easy Ensemble Adaboost Classifier 
- Accuracy score: 79.9% = (79+16139)/17205
- Precision: 7% (high risk), 100% (low risk)
- Recall: 91% (high risk), 94% (low risk)
<img width="502" alt="eec" src="https://user-images.githubusercontent.com/85041697/155737667-198e5843-8802-46bb-b017-77ca90166f19.png">


## Summary
Our accuracy score and recall are not high with the first four models(credit_risk_resampling.ipynb). Among the six models, the Easy Ensemble Classifier has the highest precision and recall scores. However, like the other models, the cunfusion metrix shows that the number of TP, TN, FP, FN are very imbalanced. Therefore, I think these models should not be used to predict credit risk.