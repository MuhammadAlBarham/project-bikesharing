# project-bikesharing



# Description: 

This project use a neural network method to predict daily bike rental rideship Which is use [Bike Sharing Dataset Data Set](https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset).

This considered a simple regression problem which use simple neural network. The netwroks consists of 2 layers ( 1 hidden layer and 1 output layer). Example netwrok as below: 


![assets/neural_network.png](assets/neural_network.png)




The main goal is to find the count of total daily rental bikes including both casual and registered. Original features and target numbers in dataset is 17 (16 features and 1 target).

# Data Processing

## Converting Categorical Data to numerical numbers: 

----
(This dataset contains categrical inputs like season, weather, month. So, they need to be convertd to numerical values. This can be done using [get_dummies](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.get_dummies.html) which Convert categorical variable into dummy/indicator variables.

----

## Scalling variables: 

The aim of this scaling is to make the training of the netowork easier. So, continues variables should be standaries to have  Zero mean and a standard deviation of 1.

# Data Slpitting:

The dataset is splitted ino training, validation and testing as below: 

- Training dataset: 89% 
- Validation dataset: 8%
- Testing dataset: 3% 


## Hyperparameter Tuning: 

You can tune the the following hyperparamters: 

- Number of iterations
- Choosing the learning rate 
- choosing the number of hidden nodes

## Results: 

Using the following hyperparamter: 

`iterations = 5000 , learning_rate = 0.1 ,hidden_nodes = 5, output_nodes = 1`

- The results are : 

Training loss: 0.230 ... Validation loss: 0.388




