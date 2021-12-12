# Neural_Network_Charity_Analysis

## Overview of the Analysis

The purpose of this analysis is to build the machine learning and neural network models to create binary classification model to predict if Alphabet Soup funding charitable organization is successful or not.

## Results

**Data Processing**

What variable(s) are considered the target(s) for your model?

- The target variable is the IS_SUCCESSFUL column. It has binary data to show if a charity is successful or not. 

What variable(s) are considered to be the features for your model?

- All the column values in the dataset except for the IS_SUCCESSFUL are features, because they describe about the charity.

What variable(s) are neither targets nor features, and should be removed from the input data?

- The EIN and NAME columns in the dataset are neither features nor targets, so we dropped the columns before we setup the ML model.


**Compiling, Training, and Evaluating the Model**

How many neurons, layers, and activation functions did you select for your neural network model, and why?

- On the initial model, i have 44 features, selected 80 neurons in the first hidden layer and second hidden layer with 30 neurons.

Were you able to achieve the target model performance?

- The target performance is 75% but the model has an accuracy of 72%.

What steps did you take to try and increase model performance?

- I have tried various method to increase the performance,

    1. Changed the standard scalar to robust scalar, because there are many outliers in the data.
    
    2. Changed the activation in the first hidden layer to "tanh".
    
    3. Dropped 2 more columns (STATUS and SPECIAL_CONSIDERATIONS) in the inital dataset.
    
    4. Added another hidden layer.
    
    5. Changed the model to run the data directly instead of getting the saved weights.

## Summary

The model has the overall performance of 72%, even after tweaking the model with various methods the performance has marginally increased to 72.5%.

Using the random forest model might be an effective approach here.
