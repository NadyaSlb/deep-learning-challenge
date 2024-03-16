# deep-learning-challenge

# Analysis

## Overview
The purpose of the analysis is to create a binary classifier using machine learning and neural networks to predict whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing

* The target variable for the model is IS_SUCCESSFUL, which indicates whether the funding provided to an organization was used effectively (1) or not (0).
* Within this dataset are a number of columns that capture metadata about each organization, such as:
EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively
* The EIN and NAME columns should be removed from the input data because they are neither targets nor features. 

### Compiling, Training, and Evaluating the Model

* The model in starter code has two hidden layers with 80 and 30 neurons, respectively, and uses the ReLU activation function for both hidden layers. The choice of the number of neurons in each layer is typically based on the complexity of the problem and the size of the dataset. The decision to use two hidden layers is common in neural network architectures. Adding more layers increases the risk of overfitting. 
The ReLU activation function is a popular choice for hidden layers.
* I wasn't able to achieve a target predictive accuracy higher than 75%.
* I took next steps to increase model performance:
- changed "cut_off" value for application types from 500 to 1000
- changed "hidden_nodes_layer1" from 80 to 50
- changed number of epochs from 100 to 50

## Summary

The deep learning model achieved an accuracy of approximately 72.66%, which did not meet the target of 72.36%. Despite making adjustments to the model's architecture, such as changing the cutoff value for application types and adjusting the number of neurons and epochs, the performance improvement was limited. Probably, additional experimenting with different activation functions, adding more layers, or increasing the size of the hidden layers would help to improve the model.