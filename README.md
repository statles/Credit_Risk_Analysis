# Credit_Risk_Analysis
Using supervised machine learning and python to assess credit risk

## Overview: 
The purpose of this analysis is to use several supervised machine learning techniques to analyze credit risk of loan applicants. Since credit risk is an inherintly skewed dataset, the analysis utilizes various forms of handling imablanced data, including SMOTEENN, random oversampling, and random forests. The performance of these different types of machine learning is then evaluated based on precision, accuracy, f1 score and .

## Results: 
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.
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
  - Oversampling: 
  - SMOTE: 
  - Undersampling: 
  - SMOTEENN: 
  - Balanced Random Forests: 
  - Easy Ensemble:

Conclusion

## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
