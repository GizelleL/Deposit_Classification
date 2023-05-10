# Deposit_Classification

#### Purpose/Goal: 
Using Naive Bayes analysis, construct a classification algorithm and present the accuracy and AUC score for those clients that will or will not subscribe to a term deposit.

#### Results: 
Naïve Bayes is a categorical classification algorithm, often used as a benchmark against other classification algorithms. That means it can be compared to other models to determine if they are useful or not.
The confusion matrix shows a total of 3,088 predictions. There are 1,223 true negative responses, which reflect that the model correctly predicted clients that did not subscribe to term deposits (no). The 984 true positives (yes) are correct predictions for clients that actually subscribed to term deposits. The 557 false negatives are the incorrect predictions that clients will not subscribe to term deposits when in fact they did. The 324 false positives indicate incorrect predictions that a client will subscribe to a term deposit when in fact they do not. The accuracy of the models is 0.71, meaning that the overall accuracy of correctly predicting the outcome of a client’s decision is 71%. Again, Naïve Bayes is a benchmark model, so other classification models need to have higher accuracy in order to be useful. 

*see notebook for more detail: https://github.com/GizelleL/Deposit_Classification/blob/main/NaiveBayesAnalysis_BankDeposits.ipynb 

A ROC curve was created showing that the curve is closer to the upper-left corner reflecting a higher TPR, lower FPR and greater area under the curve (AUC), which measures the model’s ability to distinguish between positive and negative cases. The AUC is 77%, indicating a significantly better likelihood of correctly distinguishing between 'yes' and 'no' than random guessing. Other models in this study will require at least an AUC of 77% to be considered useful.

![image](https://github.com/GizelleL/Deposit_Classification/blob/main/NB_ROC_CURVE.png)

Although a key aspect of the research was to identify customers that will subscribe to term deposits (positive cases), it is important that the models can determine non-subscribers (negative cases) as well, for higher overall accuracy.


#### Summary:
1. Naive Bayes performs well on text classification tasks, such as spam detection or sentiment analysis, where the input features are typically word frequencies or presence/absence of words. In this case, it is useful for simply and efficiently identifying clients that will or will not subscribe to a term deposit based on their indicated yes or no value. 
2. The model has an overall accuracy of 0.71 (71%), and AUC of 0.77 (77%); accuracy measures the overall performance of a model in terms of correct predictions, while AUC measures the model's ability to distinguish between positive and negative examples.
3. Given that the goal is to determine which customers will or will not purchase a term deposit, it is important to have a model with both high AUC and Accuracy. Again, the AUC indicates that the model is good at distinguishing between customers who will purchase a term deposit and those who will not. In comparison, measures the overall percentage of correct predictions made by the model on the data set. 
