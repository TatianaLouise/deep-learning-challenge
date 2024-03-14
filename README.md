# Neural Network Model Report

## Overview

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

This dataset contains a CSV with more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

## Data Preprocessing

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

- 'EIN' and 'NAME' columns are removed because they are not necessary to train the model.
- 'IS_SUCCESSFUL' is the target variable used to create a deep learning model and predict the successful campaigns.
- All other columns are the features of the model.

## Compiling, Training, and Evaluating the Model

The initial model is a two-layer neural network model with pre-defined activation functions, neurons, and layers. The first hidden layer had 80 neurons, the second hidden layer had 30 neurons, and both utilized the 'ReLU' activation function. 

This combination produced an accuracy of 72.5%

## Optimization Trials


