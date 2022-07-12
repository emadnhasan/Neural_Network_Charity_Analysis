# Neural_Network_Charity_Analysis

# Overview
Alphabet Soup would like to predict what applicants to invest in. This will be done by analyzing applicants and predicting which are stable investments and which are high risk. Using machine learning and neural networks, I applied features and created a binary classifier to help predict if the applicants will be successful. This was done by:
* Preprocessing the data
* Compiling and trianing the model
* Optimizing the model

# Results
## Data Processing
* For our model, the IS_SUCCESSFUL column was the variable that was considered the target.
* The EIN and NAME columns offer no relevant data so they were removed from the model.
* All other columns were considered features for the model.

## Compiling, Training, and Evaluating the Model
* For my neural network model I had 3 hidden layers. My first layer had 55 neurons, the second has 30, the third has 15 and there is also an output layer. All three layers had relu activation functions and the output layer had a sigmoid activation function.
![Screenshot (156)](https://user-images.githubusercontent.com/100659114/178500053-b285e1c9-251d-43be-a0be-c8b39c4810f5.png)
* The target accuracy being set at 75%, I was only able to achieve 53%
![Screenshot (157)](https://user-images.githubusercontent.com/100659114/178500095-6fbd7ac2-f3a2-4065-8955-60f89242f049.png)
* Removing columns that did not offer data that was needed (AFFILIATION, CLASSIFICATION, SPECIAL_CONSIDERATIONS) and adjusting the nerons did not raise the accuracy score.

# Summary
Despite removing features and adding neurons, the model was not able to meet the target accuracy of 75%. Some recommendations to reach the target:
* Remove more features.
* Use a Random Forest Classifier. This could provide a more accurate model since it has a larger number of estimators and due to the tree depth.
* The addition of more data.
