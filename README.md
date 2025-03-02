# deep-learning-challenge
# Report on the Neural Network Model

## Overview
The purpose of this analysis was to develop a tool for Alphabet Soup to better select applicants for funding such that the chosen applicants would have the best chance of success in their ventures. This tool was to be developed using machine learning and neural network knowledge, and attempted to use the features in a provided dataset of organizations' features and success outcomes to create a binary classifier that could predict whether applicants would be successful if funded by Alphabet Soup.

## Results
Data Preprocessing
* what variable(s) are the target(s) for your model?
  * the target is the IS_SUCCESSFUL column, a 1 meaning successful and 0 meaning unsuccessful
* what variable(s) are the features for your model?
  * the features for my model are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT columns
* what variable(s) should be removed from the input data because they are neither targets nor features?
  * the EIN and NAME variables should be removed from the input data because they are neither targets nor features.

Compiling, Training, and Evaluating the Model
* how many neurons, layers, and activation functions did you select for your neural network model, and why?
  * in my 3rd attempt to optimize the model, I selected 10 neurons for the 1st hidden layer and 6 neurons for the second hidden layer in an attempt to increase model accuracy
  * I selected 2 hidden layers to simplify the number of neurons involved
  * I selected relu, tanh, and sigmoid activation functions to increase model accuracy, focusing on relu for its simplicity and sigmoid for its value in binary (0 or 1) classification
* were you able to achieve the target model performance?
  * I was not able to achieve the target model performance; my models' accuracies were in the 72-73% range.
* what steps did you take in your attempts to increase model performance?
  * in my attempts to increase model performance, I adjusted neuron numbers, holding some values constant (from the starter code) and increasing/decreasing others.
  * I also adjusted activation functions in an attempt to increase model performance

## Summary
Overall, my deep learning models resulted in 72-73% accuracy in predicting organization success based on the given features. My recommendation would be for a different model that could process text identifiers better, in case the AFFILIATION, CLASSIFICATION, ORGANIZATION TYPE, and NAME columns had weightier data. In general, I would recommend a model that is stronger in binary classification, such as one using the sigmoid activation in the outer layer. I would also recommend dropping the SPECIAL_CONSIDERATIONS and STATUS columns as the data in these columns seemed less helpful than others in determining success outcomes.

