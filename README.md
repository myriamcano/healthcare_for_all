# Healthcare For All

## Overview

The objective of this task is to address data imbalance in classification models using the 'Healthcare For All' dataset. The datasets, named `numerical.csv`, `categorical.csv` and `target.csv` are utilized to predict the likelihood of donation (TargetB) and the donation amount (TargetD).

## Context

This task revolves around the Healthcare for All Case Study, leveraging historical donor data to construct a machine learning model. The aim is to identify potential donors and forecast their donation amounts.

## Tasks Undertaken

### Initial Data Assessment and Preprocessing

1. Imported necessary libraries.
2. Loaded the dataset into Python as the `donors` dataframe.
3. Inspected column datatypes.
4. Segregated data into numerical and categorical subsets.
5. Handled null values and performed data preprocessing.

### Modeling Phase

1. Conducted a comprehensive examination of numerical and categorical column datatypes, making adjustments as required.
2. Reassembled the numerical and categorical data into the X dataframe, designating TargetB as y.
3. Split the data into training and testing sets, further partitioning them into numerical and categorical subsets.
4. Applied feature scaling using either MinMax Scaler or Standard Scaler to train_num and test_num.
5. Employed One-Hot Encoding or Ordinal Encoding to encode categorical features in train_cat and test_cat.
6. Fitted a logistic regression model on the training data and evaluated its accuracy on the test data.

### Handling Data Imbalance

1. Evaluated the extent of class imbalance.
2. Utilized resampling strategies such as upsampling and downsampling to create a balanced representation of both classes.
3. After each resampling iteration, assessed the model's accuracy to gauge its performance improvement.

### Feature Selection

Additionally, feature selection was conducted to identify and retain the most relevant features for modeling. 
