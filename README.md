# NeuralNetwork

## Overview

The purpose of this module was to use our knowledge of Neural Networks and their associated tools to conduct a risk analysis on loan data. The end goal was to determine if a loan would be successful or not.

## Results

### Data processing
* The target variable was a boolean column called IS_SUCCESSFUL
* The following variables were the features of the model
  * APPLICATION_TYPE
  * AFFILIATION
  * CLASSIFICATION
  * USE_CASE
  * ORGANIZATION
  * STATUS
  * INCOME_AMT
  * SPECIAL_CONSIDERATIONS
  * ASK_AMT
* The following variables are neither targets, nor features, and therefore dropped
  * NAME
  * EIN

### Compiling, training, and evaluating the model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
  * In my first model, I chose to have 8 nodes in the first hidden layer and 5 hidden nodes in the second layer. This gave that first model a total of 923 parameters to work with. The activation method was relu and a sigmoid output. I chose these because it was most similar to most of the examples in class and in the module. I wanted to have a baseline that was like what I had seen most often in previous examples. 
  * I was not able to achieve the target model performance, but I feel like I came rather close. 
  * My first attempt to increaase performance was to increase the number of layers and the number of nodes in each layer to try to cast a wider net at the deeper end of the neural network and work up to a narrower net at the top. My second and third attempts I tried to increase the scope of the entire neural network adding more epochs and more nodes to each layer. Finally I tried a different activation method.
  

## Summary
This model was unable to reach 75% accuracy despite calibrating layers, nodes and activation methods. Another model such as a random forest could solve this as well as revisiting the original features to ensure that none are confusing the model. 
