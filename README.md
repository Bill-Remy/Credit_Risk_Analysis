# Credit Risk Analysis  
## Purpose of Analysis

The purpose of this analysis is to use six different machine learning models to evaluate credit risk across several accounts.  The target data, loan status, is either low-risk, value of "1", or high-risk, value of "0".   The models will be evaluated on their ability to detect high-risk loans.

## Results of Analysis

All six models were run using the same data set and using get_dummies to convert string fields to numeric.  The drop_first option was also used to reduce the number of columns without impairing the modeling ability.

A summary of the Balanced Accuracy and Classification Report for each model is shown below.

<img src="model_summaries.png">

### Model Summaries

- Random Oversampling - The Random Oversampling model produced a Balanced Accuracy of 66.8%.  The Precision for "High-Risk" loans was low at 1% buth the Recall was high at 74%.  Given the F1 score of 0.02, the model overall did not product great results.
- SMOTE - The SMOTE model yielded a Balanced Accuracy very similar to the Random Oversampling at 65.1% and very similar Recall, 0.62, and F1 score of 0.02.  Again this model given the low F1 score did not provide great results.
- Under Sampling - The Under Samplng model Balanced Accuracy was quite a bit lower than the prior two models at 56.2%.  The Precision, Recall and F1 scores were very similar to the prior two models and overall this model did not provide better resutls.
