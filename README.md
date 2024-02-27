# deep_learning_challenge
## Write a Report on the Neural Network Model

For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.

### Overview of the analysis
1. Explain the purpose of this analysis: 

Maching learning & neural networks are a powerful tool for predicting outcomes. In this case, I am trying to use the features in the provided dataset to creat a binary classifier that can predict whether applicants will be succesful if funded by Alphabet Soup. The goal is to identify applicants that are most likely to be successful if funded by Alphabet Soup.

### Results
2. Using bulleted lists and images to support your answers, address the following questions:
    * Data Preprocessing
        * What variable(s) are the target(s) for your model?
            * The target variable is the 'IS_SUCCESSFUL' column.
        * What variable(s) are the features for your model?
            * The feature variables are all the columns except for 'IS_SUCCESSFUL'; those columns are:
                * "APPLICATION_TYPE" 
                * "AFFILIATION"
                * "CLASSIFICATION"
                * "USE_CASE"
                * "ORGANIZATION"
                * "STATUS"
                * "INCOME_AMT"
                * "SPECIAL_CONSIDERATIONS"
                * "ASK_AMT"
        * What variable(s) should be removed from the input data because they are neither targets nor features?
        * The variableS 'EIN' AND 'NAME' were removed from the input data because they are not features or targets.
    * Compiling, Training, and Evaluating the Model
        * How many neurons, layers, and activation functions did you select for your neural network model, and why?
            * FIRST ATTEMPT: 3 hidden layers and Outer layer. First hidden layer has 80 hidden nodes and an activation function of 'tanh'. Second hidden layer has 30 hidden nodes and an activation function of'sigmoid'. Third hidden layer has 1 hidden nodes and an activation of 'relu'. 72.5% accuracy was achieved.
            * SECOND ATTEMPT: 3 hidden layers and Outer layer. First hidden layer has 100 hidden nodes and an activation function of 'relu'. Second hidden layer has 30 hidden nodes and an activation function of'sigmoid'. Third hidden layer has 1 hidden nodes and an activation of 'relu'. 72.1% accuracy was achieved.
            * THIRD ATTEMPT: 3 hidden layers and Outer layer. First hidden layer has 80 hidden nodes and an activation function of 'relu'. Second hidden layer has 25 hidden nodes and an activation function of'sigmoid'. Third hidden layer has 2 hidden nodes and an activation of 'relu'. 72.2% accuracy was achieved.
        * Were you able to achieve the target model performance?
            * No, I was not able to achieve the target model performance within my three attempts, because I was not able to achieve 75% accuracy or higher. 
        * What steps did you take in your attempts to increase model performance?
            * I tried to increase the number of hidden nodes in the first hidden layer and the number of hidden nodes in the second hidden layer in order to increase the accuracy of the model. I also tried to change the activation functions in the hidden layers to see if that would increase the accuracy of the model. Unfortunately, I would need more time and more attempts to achieve a higher accuracy.

### Summary
3. Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.