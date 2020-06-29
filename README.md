# Machine-Learning-Assignment
# Machine Learning End Semester Assignment

## Problem Statement
This is a multi-class Classification Problem , with  4 classes
A three layered Multi-Perceptron has been trained, with 11 input features and 'quality' as  target.
Dataset is split into test and train in 7:3 ratio respectively. 
I have taken 13 tuples in total and 10 fold Cross validation algorithm for training.
Box Plot for each pair of tuple has been plotted and the model which performed the best was used to obatin final accuracy. Later on CMC curve was plotted to check improvement in test accuracy.

### Dataset

The dataset used in this experiment is the Wine Quality  dataset (hhttps://archive.ics.uci.edu/ml/datasets/wine+quality)<br/>

It contains the following real-valued attributes:

Input variables (based on physicochemical tests):
1 - fixed acidity
2 - volatile acidity
3 - citric acid
4 - residual sugar
5 - chlorides
6 - free sulfur dioxide
7 - total sulfur dioxide
8 - density
9 - pH
10 - sulphates
11 - alcohol
Output variable (based on sensory data):
12 - quality (score between 0 and 10)

30 % of the dataset at random is taken as the held-out test dataset and all the experiments have been done on the remaining 70% dataset as the training dataset.

### Cross-validation scores for different sets of hyperparameters

13 tuples has been randomly selected and for each of the model has been trained and 10-fold cross validation has been used . For each of them the accuracy of te model was stored.


### Boxplot Analysis of the results

Box Plots of cross validation scores are drawn for accuracy obtained  for each pair of tuple and were compared to obtain the best fit set of hyperparameters.
Ideally, those hyperparameter should be  chosen  which have highest mean accuracy , least oultiers, and least inter-quartile distance.


Thus, taking that into consideration, tuple 13 was chosen as the best set of hyperparameters, because it had the highest mean cross validation score, has no outlier and the quartile distance of the scores is also moderate.

### Result on the test dataset

The hyperparameters used in the final model are :
* Learning Rate = 0.03
* Number of hidden nodes = 50

The model had an accuracy of 72.2222208 % on the test dataset.

### Cumulative Match Characteristic (CMC) curve


As can be observed from the CMC curve, the model has a considerably higher last accuracy on the test dataset.

### Author

* Name:- Rishika Rathore
* Roll Number:- 17045084
* Branch:- Chemical Eng.
