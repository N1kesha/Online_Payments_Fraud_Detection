# Online Payments Fraud Detection Project

Detecting fraudulent online transactions is a crucial task, since it is aimed at protecting financial systems and personal data of users.

In this project I implemented CatBoost Classifier, the Yandex's Gradient Boosting model which is based on Decision Trees. ROC AUC of fine-tuned model equals 0.985 on test dataset and 0.999 on train dataset, considering that I also used validation dataset for finding optimal hyperparameters.

Data: https://www.kaggle.com/datasets/jainilcoder/online-payment-fraud-detection

## Train data features: 

step: represents a unit of time where 1 step equals 1 hour

type: type of online transaction

amount: the amount of the transaction

nameOrig: customer starting the transaction

oldbalanceOrig: balance before the transaction

newbalanceOrig: balance after the transaction

nameDest: recipient of the transaction

oldbalanceDest: initial balance of recipient before the transaction

newbalanceDest: the new balance of recipient after the transaction

isFraud: fraud transaction
