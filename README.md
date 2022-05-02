# Credit_Risk_Analysis
Using supervised machine learning and python to assess credit risk

## Overview: 
The purpose of this analysis is to use several supervised machine learning techniques to analyze credit risk of loan applicants. Since credit risk is an inherintly skewed dataset, the analysis utilizes various forms of handling imablanced data, including SMOTEENN, random oversampling, and random forests. The performance of these different types of machine learning is then evaluated based on precision, balanced accuracy, and recall.

## Results: 
- Balanced Accuracy Scores:
  - Oversampling: 0.6573
  - SMOTE: 0.6622
  - Undersampling: 0.5442
  - SMOTEENN: 0.6231
  - Balanced Random Forests: 0.7885
  - Easy Ensemble: 0.9316
  
Conclusion: The Easy Ensemble Classifier had the best balanced accuracy score and the random undersampling had the worst balanced accuracy score.

- Precision Scores:
  - Oversampling: Avg: 0.99, High Risk: 0.01, Low Risk: 1.00
  - SMOTE: Avg: 0.99, High Risk: 0.01, Low Risk: 1.00
  - Undersampling: Avg: 0.99, High Risk: 0.01, Low Risk: 1.00
  - SMOTEENN: Avg: 0.99, High Risk: 0.01, Low Risk: 1.00
  - Balanced Random Forests: Avg: 0.99, High Risk: 0.03, Low Risk: 1.00
  - Easy Ensemble: Avg: 0.99, High Risk: 0.09, Low Risk: 1.00
  
Conclusion: There was very high precision for Low Risk samples, and very low precision for High Risk samples. This is most likely due to High Risk samples being under-represented in the dataset (68470 low risk samples versus 347 high risk samples). However, the Easy Ensemble Classifier had a slightly higher precision score for the High Risk samples.

- Recall Scores:
  - Oversampling: Avg: 0.60, High Risk: 0.71 Low Risk: 0.60
  - SMOTE: Avg: 0.69, High Risk: 0.63 Low Risk: 0.69
  - Undersampling: Avg: 0.40, High Risk: 0.69 Low Risk: 0.40
  - SMOTEENN: Avg: 0.59, High Risk: 0.65 Low Risk: 0.59
  - Balanced Random Forests: Avg: 0.87, High Risk: 0.70 Low Risk: 0.87
  - Easy Ensemble: Avg: 0.94, High Risk: 0.92 Low Risk: 0.94

Conclusion: The Easy Ensemble classifier had the highest recall and the random undersampling had the lowest recall.

## Summary: 
Due to the extreme imbalanced in the two categories, this was a difficult dataset for the machine to train on. Many of the models behaved poorly, with balanced accuracy scores around 0.60. However, the EasyEnsembleClassifier seemed to work the best out of all the models. This model had the highest balanced accuracy score and the highest recall of all the models. However, due to all the models having a very low precision score for High Risk samples, I would not recommend any model. There are far too many low risk credit scores being flagged as high risk, which will be difficult for both the business and the customer to fix.
