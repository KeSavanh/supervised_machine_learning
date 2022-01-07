# Predicting Credit Risk

A machine learning model is to be built that attempts to predict whether a loan from LendingClub will become high risk or not.

## Background

LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API.


## Retrieve the data

In the Generator folder in Resources, there is a GenerateData.ipynb notebook that will download data from LendingClub and output two CSVs:

2019loans.csv
2020Q1loans.csv

You will be using an entire year's worth of data (2019) to predict the credit risk of loans from the first quarter of the next year (2020).
Note: these two CSVs have been undersampled to give an even number of high risk and low risk loans. In the original dataset, only 2.2% of loans are categorized as high risk. To get a truly accurate model, special techniques need to be used on imbalanced data. Undersampling is one of those techniques. Oversampling and SMOTE (Synthetic Minority Over-sampling Technique) are other techniques that are also used.


## Preprocessing: Convert categorical data to numerical

In this step, I decided to use conventional pandas replace method instead of `pd.get_dummies()` to avoid dubble creating the columns. I checked the shape of both trainning and testing data to make sure there won't be any missing columns.

And the following tasks were performed:

## Consider the models
## Fit a LogisticRegression model and RandomForestClassifier model
## Revisit the Preprocessing: Scale the data