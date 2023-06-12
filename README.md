## Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

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


# Overview of the analysis: 
The purpose of the analysis is to  predict if applicants for the nonprofit foundation Alphabet Soup will be successful or notfind. The goal for the model was to reacah a 75% or higher to consider the model viable. 


# Results:

Data Preprocessing

What variable(s) are the target(s) for your model?
The target variable was "IS_SUCCESSFUL" for this model.

What variable(s) are the features for your model?
The feature variables were "ORGANIZATION", "ASK_AMT", "SPECIAL_CONSIDERATIONS", "INCOME_AMT", "STATUS", "USE_CASE", "CLASSIFICATION", "AFFILIATION", and "APPLICATION_TYPE" for this model.

What variable(s) should be removed from the input data because they are neither targets nor features?
The EIN and NAME - Identification columns variables should be removed.

# Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
I tested 3 hidden layers of Neurons with counts of 160,70,60 with activation fuction of relu for all. the reasons being that relu is a faster function than sigmoid with its ability to compute faster. 

Were you able to achieve the target model performance?
I was not able to achieve the goal, the closest was 72.47%. 

What steps did you take in your attempts to increase model performance?
The steps I took to increase the model was to change the amount of neurons per layer as well as change the activation functions . Lastly, even changing the number of epochs.

# Summary: 
After attempting multiple optimizations, including adjusting the number of neurons, adding extra hidden layers, and increasing the number of epochs, the desired accuracy score of 75% or higher was not achieved. To further improve the deep learning model, the following steps could be taken ,Increase the number of neurons, Add an additional hidden layer, Increase the number of epochs and Experiment with activation functions. An alternative approach could be to use a logistic regression. This type of model is suitable for categorical outcome variables like the "is_successful" label. By separating the outcome variable from the features, splitting the data into training and testing sets, fitting the logistic regression model, making predictions on the test set, and evaluating the accuracy score, confusion matrix, and classification report, it is possible to assess the model's performance and determine if it provides a better solution.
