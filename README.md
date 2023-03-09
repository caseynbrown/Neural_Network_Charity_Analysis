# Neural_Network_Charity_Analysis

## Overview of the Analysis
The purpose of this analysis was to assist Alphabet Soup successfully predict whether applicants will be successful if funded by Alphabet Soup. 

## Results
Data Preprocessing
1. What variable(s) are considered the target(s) for your model?
Verifying if the target is marked as successful in the Dataframe, indicating that it was successfully funded by Alphabet Soup. 
2. What variable(s) are considered to be the features for your model?
The "IS_SUCCESSFUL" data references whether or not the charity donation was used effctively, so this is the feature for our model. 

![image](https://user-images.githubusercontent.com/115745142/224176579-8b013192-5928-41b3-b511-84765f406c6a.png)

3. What variable(s) are neither targets nor features, and should be removed from the input data?
The EIN and NAME columns were not applicable as targets or features, so they were removed from the data. 

![image](https://user-images.githubusercontent.com/115745142/224176815-264de0d5-e419-4141-8ba6-c7107ece337e.png)


Compiling, Training and Evaluating the Model
1. How many neurons, layers and activation functions did you select for your neural network model, and why?
I madde 3 separate attempts to optimize the data, using 4 hidden layers and one output layer, using relu, sigmoid and linear as the activation functions, and the following breakdown of neurons: 
1st attempt: 110, 80, 40, 20 & 1

![image](https://user-images.githubusercontent.com/115745142/224177828-c2ae50d5-cbbf-4de8-b019-752106558c85.png)


2nd attempt: 80, 50, 30, 20 & 1

![image](https://user-images.githubusercontent.com/115745142/224177860-927eec1b-32a1-40ca-90ca-83dc296ad79d.png)


3rd attempt: 100, 75, 50, 25 & 1

![image](https://user-images.githubusercontent.com/115745142/224177901-a87117fa-82ee-44c5-aad6-322fcaebcc73.png)


The initial request used relu and sigmoid, with 2 hidden layers and one output layer, with these units: 110, 80 & 1. 

2. Were you able to achieve the target model performance?
I was not able to achieve the target model performance of 75% accuracy. I was close, at 72% from my 2nd attempt. 

3. What steps did you take to try and increase model performance?
I hoped to increase performance by decreasing the number of neurons on the 2nd attempt and use a model with more hidden layers, even using the linear output but that did not work. 

## Summary
The deep learning neural network model did not reach the target of 75% accuracy. The target seems reasonable, so there is additional work that needs to be done here to achieve the desired results. 
Since both the sigmoid and linear activations did not achieve the desired result, I would suggest trying a Random Forest Classifier in order to remove the impact of any remaining outliers that could cause the accuracy result to sway. 
