
# Module 21 Challenge

The nonprofit foundation Alphabet Soup wants a tool that can help it select the
applicants for funding with the best chance of success in their ventures. With
your knowledge of machine learning and neural networks, you’ll use the features
in the provided dataset to create a binary classi)er that can predict whether
applicants will be successful if funded by Alphabet Soup.
From Alphabet Soup’s business team, you have received a CSV containing more
than 34,000 organizations that have received funding from Alphabet Soup over
the years. Within this dataset are a number of columns that capture metadata
about each organization, 

such as:


EIN and NAME—Identi)cation columns

APPLICATION_TYPE—Alphabet Soup application type

AFFILIATION—AJliated sector of industry

CLASSIFICATION—Government organization classi)cation

USE_CASE—Use case for funding

ORGANIZATION—Organization type

STATUS—Active status

INCOME_AMT—Income classi)cation

SPECIAL_CONSIDERATIONS—Special considerations for application

ASK_AMT—Funding amount requested

IS_SUCCESSFUL—Was the money used effectively





## Overview:

 The purpose of the charity funding analysis for Alphabet Soup was to predict which investments the company should approve. Our aim was to use machine learning and neural networks to analyze the dataset, applying target and feature variables to create a binary classifier. This classifier would predict the success of investments funded by Alphabet Soup. We started with data from 34,000 organizations, including 12 columns that contained information about each organization and their past funding outcomes.


Steps for the analysis are:

 Step 1: Preprocess the Data

 Step 2: Compile, Train, and Evaluate the Model

 Step 3: Optimize the Model
 
 Step 4: Write a Report on the Neural Network Model
 



## Result
1.Data Preprocessing

What variable(s) are the target(s) for your model?

Answer: The target variable for the model is the binary IS_SUCCESSFUL column, indicating whether a charity donation was successful.



What variable(s) are the features for your model?

Answer:The feature variables include all other columns that provide information about the donations and the organizations.
![image](https://github.com/user-attachments/assets/852dd9dd-1049-4ff2-a07e-2b77fd8cfc04)


What variable(s) should be removed from the input data because they are neither targets nor features?

Answer: Variables that are neither targets nor features, such as EIN and NAME, are removed from the input data to avoid unnecessary noise in the model.


2. Compiling, Training, and Evaluating the Model


How many neurons, layers, and activation functions did you select for your neural network model, and why?

Answer:	Neurons, Layers, and Activation Functions: The neural network model consists of three layers:

o	First hidden layer: 80 neurons, ReLU activation function

o	Second hidden layer: 30 neurons, ReLU activation function

o	Output layer: 1 neuron, Sigmoid activation function

These parameters were chosen to provide sufficient capacity for the model to learn complex patterns in the data while avoiding overfitting.
![image](https://github.com/user-attachments/assets/563b5183-94ce-4921-9da8-3e458e4556e6)



Were you able to achieve the target model performance?

Answer: The target performance of 75% accuracy was not achieved despite various optimization attempts. The highest accuracy obtained was approximately 72.76%.

![image](https://github.com/user-attachments/assets/c915dae3-b458-4fd6-8bcb-cf8e23ef73b5)


What steps did you take in your attempts to increase model performance?
Answer:
•	Adjusting Input Data: Dropped irrelevant columns and binned categorical variables with rare occurrences.
•	Increasing Model Complexity: Added more neurons and hidden layers to the model.
•	Changing Activation Functions: Tested different activation functions for hidden layers.
•	Adjusting Training Parameters: Increased epochs to 300, set batch size to 32, and used a 20% validation split.





## Summary

Despite multiple attempts to optimize the model, the target accuracy of 75% was not achieved. The final model reached an accuracy of approximately 72.76%. To further improve performance, other machine learning models, such as Random Forest or Gradient Boosting, could be explored. These models are often effective in handling complex datasets with many categorical variables and may provide better predictive accuracy.


