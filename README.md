# <font color=#6495ED>Neural Network Charity Analysis/font>

## <font color=#6495ED>Project Overview</font>

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. With the knowledge of machine learning and neural networks, we will use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

### <font color=#6495D>Purposes</font>

- Preprocessing Data for a Neural Network Model

- Compile, Train, and Evaluate the Model

- Optimize the Model

## <font color=#6495ED>Resources</font>

### <font color=#6495D>Data Source: </font>
charity_data.csv

### <font color=#6495D>Software:</font> 
- Anaconda with python 3.9
- Jupyter Notebook
- tensorflow(2.6.5)
- scikit-learn library (1.1.1)

## <font color=#6495ED>Results</font> 
### 1. Data Preprocessing
- The "IS_SUCCESSFUL"  variable is considered the target for your model.

- The following variable(s) should be considered on features model: 
  * APPLICATION_TYPE, 
  * AFFILIATION, 
  * CLASSIFICATION, 
  * USE_CASE, 
  * ORGANIZATION, 
  * STATUS, 
  * INCOME_AMT, 
  * SPECIAL_CONSIDERATIONS, 
  * ASK_AMT

-  The EIN and NAME cvariables should be removed from the input data

### 2. Compiling, Training, and Evaluating the Model

- There are 2 hidden layers with 80 neurons in the first layer,  and 30 neurons in the second layer . Each of the hidden layers has an activation function "relu" and the output layer has "sigmoid".

![Compiling_Training_Evaluating_the_Model](https://github.com/NingYang2022/Neural_Network_Charity_Analysis/blob/main/Images/Compiling_Training_Evaluating_the_Model.png?raw=true)

- I was not able to achieve the target model performance which is 75%. The Accuracy is 72.583% with Loss of 56.139%

![A_L_D2](https://github.com/NingYang2022/Neural_Network_Charity_Analysis/blob/main/Images/A_L_D2.png?raw=true)

### 3. Optimize the Model, 3 steps to try to increase model performance

  1. Added 40 more neurons to the first hidden layer.
![A_L_more_neurons](https://github.com/NingYang2022/Neural_Network_Charity_Analysis/blob/main/Images/A_L_more_neurons.png?raw=true)

  2. Added one more hidden layer with 30 neurons.             
![A_L_more_layer](https://github.com/NingYang2022/Neural_Network_Charity_Analysis/blob/main/Images/A_L_more_layer.png?raw=true)

  3. changed the activation type to sigmoid for hidden layers and reLU for output layer
![A_L_diff_actType](https://github.com/NingYang2022/Neural_Network_Charity_Analysis/blob/main/Images/A_L_diff_actType.png?raw=true)



## <font color=#6495ED>Summary</font>

The deep learning model and attempts for tuning-up were not able to reach its target accuracy of 75%. We recommend to try using a different model, such as random forest, to solve the problem
