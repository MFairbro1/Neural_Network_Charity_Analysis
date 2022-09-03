# Neural_Network_Charity_Analysis

## Overview:

### Alphabet Soup, a non-profit which donates to organizations with noble goals, has tasked us with creating a binary classifier to predict whether applicants will be successful if they receive funding. This will be accomplished using a deep learning neural network trained on a dataset with data from more than 34,000 organizations.

## Results:

### Data Processing:

### - The target variable is the "IS_SUCCESSFUL" column

### - The features consist of all other columns except "IS_SUCCESSFUL", "EIN", and "NAME"

### - "EIN" and "NAME" are neither features nor targets and are removed from the dataset

### Compiling, Training, and Evaluating the Model:

### - The initial model consisted of two hidden layers with the first having 90 neurons (around double the number of inputs) and the second having 30
### These both use the ReLU activation function for faster computation time 
### The output layer uses the sigmoid activation function given that we are creating a binary classifier
### This initial model did not yield the target perfomance of higher than 75%

### - Three attempts were made to improve the performance of the model
### The first attempt involved increaing the neurons in the first hidden layer to 100 but this did not yield a higher accuracy score
### The second and third attempts kept 100 neurons for the first hidden layer, but the second hidden layers consisted of 50 and 60 neurons respectively
### None of these new configurations improved on the accuracy

## Summary:

### Overall, the desired accuracy of over 75% was not achieved despite attempts at model optimization. Since this is a binary classification problem there are other machine learning algorithms available such as the random forest classification algorithm since it reduces overfitting and it better at handling outliers.
