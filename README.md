# deep-learning-challenge

Final Report

Overview of the analysis: 
    This analysis developed a deep learning model using the 'application_df' dataset. The goal of the model is to use features from the dataset to predict whether or not the application ask is successful or not. 

Results

Data Preprocessing

What variable(s) are the target(s) for your model?
    The target variable for the model is the "IS_SUCCESSFUL" column.

What variable(s) are the features for your model?
    The features for the model are represented by the columns - "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "STATUS",
    "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT".

What variable(s) should be removed from the input data because they are neither targets nor features?
    The variables "NAME" and "EIN" are removed from teh dataset.

Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
    In the initial model, I chose to use 2 hidden layers with 80 and 30 neurons, and used relu as the activation function. I chose relu for the ability to work with non-linear data. 

Were you able to achieve the target model performance?
    I was not able to achieve over 75% accuracy.

What steps did you take in your attempts to increase model performance?
    In attempts to optimize, I changed the first layer's activation function to tahn but increased the neurons in each layer (asde from the output layer)to 90 and 50). In the next attempt I added a 3rd hidden layer and included 64 additional neurons, and in the 3rd and final attempt I chose to lower the cutoff number for the application_type and classification columns, adding more bins containing rare occurances. 

Summary:
    The most effective model in my trials was optimization attempt #2 with 72.62% accuracy, though all attempts were within decimals of that value. The changes I made to optimize didn't seem to impact the results much. A recommendation for a different model: the Random Forest algorithm could capture more of the interactions betweek all variables and potentially lead to a more accurate prediction for the target. Random Forest can work with the numerical and categorical data, and would categorize feature importance to identify the most relevant feature variables to work with.