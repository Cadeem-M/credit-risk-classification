# credit-risk-classification


## Overview of the Analysis

The goal of this project is to train and evaluate a model based on loan risk. I’ll be using a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. Specifically, "loan status" from the data set will be our target vector as we use the remaining data set as our features to generate the model. Once done, the model should be able to distinguish a healthy loan (loan status = 0) from a high-risk loan (loan status = 1).

To summarize the steps taken:
* Used pandas to read are data set as a Dataframe
* Seperated the loan status column into its own vector from the features (the remaining dataframe)
* Ran train_test_split from sklearn package to generate sets for training and testing our model
* Created a logistic regression model and had the data fit onto it
* Used the model to make a prediction using the test data set
* Generated a classification report to analyze the performance of the model


## Results

The Logistic Regression Model Classification report

              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384


* The accuracy of the model was found to be 99%

* For loan status = 0: 
1) Precision is 100%
2) Recall is 99%

* For loan status = 1:
1) Precision is 85%
2) Recall is 91%




## Summary

In conclusion, the logistic regression model seems to do reasonably well at distinguishing loan statuses. With a 99% accuracy, we can say the model does a good job at correctly predicting observations. Furthermore, the model seems to perform really well at determining healthy loans. With a precision of 100%, all of its predicted healthy loans were actually healthy loans and a recall of 99% means it was able to capture 99% of the total healthy loans. 

