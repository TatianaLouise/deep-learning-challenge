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
<img width="1167" alt="Screenshot 2024-03-14 at 10 35 30 AM" src="https://github.com/TatianaLouise/deep-learning-challenge/assets/143769037/b9d70a4a-289c-4185-8cc4-9441d214c750">

The initial model is a two-layer neural network model with pre-defined activation functions, neurons, and layers. The first hidden layer had 80 neurons, the second hidden layer had 30 neurons, and both utilized the 'ReLU' activation function. 

This combination produced an accuracy of 72.5%

## Optimization Trials

# Optimization Trial 1 - Dramatically reduce hidden layer nodes to 10 for the first layer, and 5 to the second layer.
<img width="974" alt="Screenshot 2024-03-14 at 10 44 37 AM" src="https://github.com/TatianaLouise/deep-learning-challenge/assets/143769037/656faa1b-a92b-4e98-9b96-904934eae0b6">

<img width="1069" alt="Screenshot 2024-03-14 at 10 46 53 AM" src="https://github.com/TatianaLouise/deep-learning-challenge/assets/143769037/76e58be7-fa86-458d-896c-45c5e93bf861">

- Optimization trial 1 produced an accuracy score of - 72.8% (Almost no change)

# Optimization Trial 2 - Add 2 more layers. The first layer has 80 nodes, the second layer has 50 nodes, and the third layer has 10 nodes with an activation 'sigmoid'.
<img width="1080" alt="Screenshot 2024-03-14 at 10 45 07 AM" src="https://github.com/TatianaLouise/deep-learning-challenge/assets/143769037/946ae5ea-4920-4d23-bdae-6b8c8ed603d1">

<img width="766" alt="Screenshot 2024-03-14 at 10 51 04 AM" src="https://github.com/TatianaLouise/deep-learning-challenge/assets/143769037/ae293f78-e960-434e-a0e8-e07b13962eaa">

- Optimization trial 2 produced an accuracy score of - 72.6% (Almost no change)

# Optimization Trial 3 - Increase the numbe of values in each bin during preprocessing and include a third hidden layer.
<img width="1069" alt="Screenshot 2024-03-14 at 10 46 53 AM" src="https://github.com/TatianaLouise/deep-learning-challenge/assets/143769037/082cf30f-bf17-4864-a791-c983b05e35d6">
