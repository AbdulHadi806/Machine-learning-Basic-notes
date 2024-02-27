# Algorithms and Related Topics

## Logistic Regression
Logistic Regression is a type of classification algorithm. Logistic Regression is a type of analysis for predicting binary outcomes. E.g predicting whether a student 
will pass(1) or fail(0) based on study hours. Logistic Regression works on the probability for example in the graph below, we can see that the threshold value is set at the center.
This value is a probability that whether the dependent variable value we get due to independent variables, the value will be according to the threshold e.g if the value
is below the threshold then the student has failed and if it is above it then it would mean that the student has passed.

### Finding the probability of each class

```
probabilities = model.predict_proba(x_test)[:, 1]
```

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/cb6bb37d-aaf5-4a47-837e-92db735f44a1">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/801b7946-35f8-432f-80a6-543e6c919f9f">


## Linear Regression
It finds the best-fitting line that represents the relationship between X and Y.


<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/eb7c0bd5-a47c-486d-ac9d-539b9723d7a1">


## Decision Tree Regressor
Decision tree regressor involves **partitioning the data into subsets** based on the values of **independent variables** and predicting the average of the target
variable for each subset.
**Fun Fact** A Decision tree can do both classification and regression.

<img width="389" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/b4824102-2112-4ae7-86ef-4ac4e74850e0">


## Random Forest Regressor
Random Forest is a learning method that creates **multiple decision trees** during training and outputs the **average prediction**(for regression) from all individual trees.


<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/14066147-7985-45ab-8b2f-66e663ca4a03">


## Gradient Boosting Regressor
Gradient Boosting Regressor is a learning technique that builds multiple trees sequentially, each one correcting the errors of its predecessor.


<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/948e06ca-d1e7-482c-abab-14cba39deef4">

## Entropy
In Machine Learning, entropy measures the level of disorder or uncertainty in a given dataset or system. It is a metric that quantifies the amount of information in a dataset, and it is commonly used to evaluate the quality of a model and its ability to make accurate predictions.

In the context of **Decision Trees**, entropy is a measure of disorder or impurity in a node. Thus, a node with more variable composition, such as 2Pass and 2 Fail would be considered to have higher Entropy than a node which has only pass or only fail.
