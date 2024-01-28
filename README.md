# Credit Card fraud detection model


## Problem Statement:


A credit card is one of the most used financial products to make online purchases and payments. Though the Credit cards can be a convenient way to manage your finances, they can also be risky. Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash.
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. The dataset contains transactions made by credit cards in September 2013 by European cardholders. 


This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. 
We have to build a classification model to predict whether a transaction is fraudulent or not.

## Data
The dataset is taken from the Kaggle website and it has a total of 2,84,807 transactions, out of which 492 are fraudulent.The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
 So it needs to be handled before model building.

## Project Pipeline:
• Data Collection : Here, we need to load the data and understand the features present in it. This would help us to choose the features that you will need for your final model.

• Exploratory data analytics (EDA): Analyzing and understanding the data to identify patterns, relationships, and trends in the data by using Descriptive Statistics and Visualizations.Here we need to check the skewness of the variable as it might cause problems during the model-building.we also need to check for null values.

• Feature Engineering: Here we need to scale the Amount and Time column usin standatd scaller as other columns are already scaled by the PCA transformation. 
• Balancing the data: Here we need to balance the data. so SMOTE was used as a over sampling method for this purpose.

• Model Selection:
Choose appropriate classification algorithms for the problem, considering the imbalanced nature of the data. Common choices include Logistic Regression, Random Forest, Support Vector Machines, or Gradient Boosting models.
Here logistics Regression was used as a classifier.

• Model Training:
Split the data into training and testing sets.
Use the training set to estimate the best model parameters.
Perform hyperparameter tuning .Fine-tune the model parameters based on validation results to improve overall performance.

• Model Validation:
Evaluate the model's performance on the test set using metrics like accuracy, precision, recall, F1 score, and ROC-AUC.
Use confusion matrices to understand the model's performance in detecting fraud and non-fraud cases.The data is highly imbalanced it is is more important to identify which are fraudulent transactions accurately than the non-fraudulent.
Check for signs of overfitting or underfitting.

• Saving the Model:
Here the model was saved using pickle as credit_cardModel.
