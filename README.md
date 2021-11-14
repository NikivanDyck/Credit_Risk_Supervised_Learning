# Credit Risk via Supervised Machine Learning
Module 12

---
## Overview of the Analysis
The analysis presented was to review historical lending data and build a model that can identify the creditworthiness of borrowers. The data attributes of loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt were compared against the loan status (healthy vs. high risk).   Separate test data was held back and later compared against machine learning results to validate results.  

One of the challenging aspects of this data set is more positive loan status vs. negative status. 
To manage this, we completed two data reviews: 1) using a logistic regression model (please see notes for additional information about models) on the original data and 2) applying the logistic regression model after oversampling.   

---
## Results
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

*Machine Learning Model 1/ LogisticRegression
  * Model 1 uses data as presented with an underrepresented number of negative results.    
  * Accuracy of predicting positive(yes) healthy loan status is 99%, and predicted negative(no) high risk is 91%,
  * Precision of Yes is 100%, the Precision of No 85%
  * Recall of Yes 99%, No 91%

*Machine Learning Model 2 / LogisticRegression with OverSampledData
 * Model 2 uses an equal number of positive and negative results by adding an equal number of negative results into the data set
 * Accuracy of predicting positive(yes) healthy loan status is 99%, and predicted negative(no) high risk is 99% 
 * Precision of Yes is 99%, the Precision of No 99%  
 * Recall of Yes 99%, No 99%

---
## Summary
Balancing the data sets by adding at-risk loans created a model that has 99% accuracy for both healthy and at-risk loans.   The precision of predicting healthy loans changed from 100% in Model 1 to 99% in Model 2, and the precision of predicting high risk loans changed from 85% in Model 1, to 99% in Model 2. High-risk loans can indicate increased loan defaults; Machine Learning Model 2 using oversampled data allows for more accurate results on this high-risk classification of customer while having little to no impact on healthy loans.   


Please refer to "Notes" within this git notebook to learn more about types of Supervised Machine Learning and what they do, or understand more about the definitions of principles discussed in this review.  
