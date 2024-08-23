## Optimization Report

**Overview of the analysis**: The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. This proesses uses machine learning and neural networks to assit with this. From the features provided in the dataset, I used these to create a binary classifier that could help predict whether applicants will be successful if funded by Alphabet Soup. 

### Results

**Data Preprocessing**
The following questions with answers are below. 
- What variable(s) are the target(s) for your model?: 
    -  Target variables: "IS_SUCCESSFULL
- What variable(s) are the features for your model?: 
    - APPLICATION_TYPE
    - AFFILIATION
    - CLASSIFICATION
    - USE_CASE
    - ORGANIZATION
    - STATUS
    - INCOME_AMT
    - SPECIAL_CONSIDERATIONS
    - ASK_AMT
- What variable(s) should be removed from the input data because they are neither targets nor features?: 
    -  EIN
    - NAME

### Compiling, Training, and Evaluating the Model

I used various number of neurons within my layers (i.e. 80, 30, 15 ,10), with activations of "relu" or "tanh" for my hidden layers and "sigmoid for my outter layer.
 
**Alphabet Soup Charity**

I started with 2 hidden layers on my oiginal model that used the activation function "relu" with outter layer activation of "sigmoid". This one did not achieve a perfomrmance accuracy of 75% or better. It achieved accuracy of 72.85%

**Alphabet Soup Charity Optimization**

I started with 2 hidden layers on my oiginal optimization model that used the activation function "relu" with outter layer activation of "sigmoid". This one did not achieve a perfomrmance accuracy of 75% or better. It achieved accuracy of 72.96%

In my second attempt I used 3 hidden layers on model that used the activation function "relu" with outter layer activation of "sigmoid". This one did not achieve a perfomrmance accuracy of 75% or better. It achieved accuracy of 72.97%

In my third attempt I used 4 hidden layers on the model that used the activation function "relu" and "tanh". First and third layer used "relu" while second and third used "tanh" with outter layer activation of "sigmoid". This one did not achieve a perfomrmance accuracy of 75% or better. It achieved accuracy of 72.94%

Unfortunately with the model I used with optimizaton I was not able to achieve a performance accuracy of 75% or higher.


**Summary**: The model used for Alphabet Soup has dececent accuracy in predicting results for succes of funded applicants. However it has not been perfected and still needs to be trained more efficently. It could be recommend that other models like Gradient Boosting or Random Forrest be used to help acchieve the desired results. 
- Gradient Boosting: technique that combines the predictions from several models to improve the overall predictive accuracy. 
- Random Forrest: made up of a large number of small decision trees, called estimators, which each produce their own predictions. The random forest model combines the predictions of the estimators to produce a more accurate prediction.
