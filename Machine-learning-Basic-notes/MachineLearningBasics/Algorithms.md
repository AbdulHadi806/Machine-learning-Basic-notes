# Algorithms

## Logistic Regression
Logistic Regression is a type of classification algorithm. Logistic Regression is a type of analysis for predicting binary outcomes. E.g predicting whether a student 
will pass(1) or fail(0) based on study hours. Logistic Regression works on the probability for example in the graph below, we can see that threshold value is set at the center.
This value is a probability that whether the dependent variable value we get due to independent variables, the value will be according to the threshold e.g if the value
is below threshold than the student has failed and if it is above it than it would mean that the student has passed.

### Finding probability of each class

```
probabilities = model.predict_proba(x_test)[:, 1]
```

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/cb6bb37d-aaf5-4a47-837e-92db735f44a1">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/801b7946-35f8-432f-80a6-543e6c919f9f">


## Linear Regression
It finds the best fitting line that represents the relationship between X and Y.


<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/eb7c0bd5-a47c-486d-ac9d-539b9723d7a1">
