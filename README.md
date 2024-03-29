# Neural_Network_Charity_Analysis

## Overview of the Analysis 
Using Machine Learning and Neural Networks for this project, I used the features in the dataset to create a binary classifier that will help to predict if the applicants that will be funded by a Charitable organization called Alphabet Soup will be successful. For this analysis we had a dataset containing various measures on 34,000 organizations that have been funded by Alphabet Soup. This project compromised of the following 3 steps: 
- Preprocessing the data for the neural network 
- Compile, Train and Evaluate the Model 
- Optimizing the model

## Results 

### Data Preprocessing 
- Variable that was considered as the target for my model: IS_SUCCESSFUL Column
- Variables that were considered features for my model: Every Column except for IS_SUCCESSFUL which is our target and the ones we will drop
- Variable that were neither targets or features for the dataset: Columns that I dropeed are EIN, NAME because they will have little to no impact om our outcome

### Compiling, Training and Evaluating the Model

The number of neurons, layers, and activation functions I selected for my neural network model:
- For my neural network model I had 2 hidden layers. My first layer had 80 neurons, the second has 30 there is also an output layer. The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."
![ml1](https://user-images.githubusercontent.com/59430635/156963931-43696c87-999a-454f-b3f5-cb90f57910da.PNG)



Was the model able to achieve the target model performance?
- The model was not able to reach the target 75%. The accuracy for my model was 69%.

![ml2](https://user-images.githubusercontent.com/59430635/156963938-275040d5-9101-4bd0-a632-46ba4b31ca64.PNG)


The steps taken to try and increase model performance

- Attempt 1: Removed additional feature, that is the 'USE_CASE' column. Rest of the model components stayed the same, however model accuracy went down to 63%. 

![ml3](https://user-images.githubusercontent.com/59430635/156963942-165ae575-de89-414c-bde7-a7f043e94a48.PNG)


![ml4](https://user-images.githubusercontent.com/59430635/156963947-6de90237-02a4-4154-87c2-0d9f60e0d73c.PNG)


-  Attempt 2: Adding Additional neurons to hidden layers and additional hidden layers are added. The accuracy went down again, this time it was 53%.

)![ml6](https://user-images.githubusercontent.com/59430635/156963960-e54a79a7-35c9-48a2-9c92-a95b6fd04ae7.PNG)




- Attempt 3: Changing activation function of output layer from "sigmoid" to "tanh." The accuracy of the model went down even more to 50%.

![](Resources/ml7.PNG)
![ml7](https://user-images.githubusercontent.com/59430635/156963966-7a9838fd-f584-4523-9840-53f401e159f9.PNG)


![](Resources/ml8.PNG)

## Summary 

The model ended up with the accuracy score of 50% after optimization. The initial neural network had a accuracy score of 69%. This loss in accuracy can be explained from the fact that the model overfitted. Furthermore, we could further also optimize our neural network by removing more features or simply adding more data to the dataset to increase accuracy.
Since our accuracy score was not particularly up to the standard with neural networks, we could have used the Random Forest classifiers. This is because random forest is a robust and accurate model due to their sufficient number of estimators and tree depth. Also the random forest models have a faster performance than neural networks and could have avoided the data from being overfitted. 
