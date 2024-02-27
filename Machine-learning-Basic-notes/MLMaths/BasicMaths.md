# Basic Machine Learning Maths


## Loss Function
A loss function quantifies the difference between the predicted value of model and the actual value. It is done through methods such as Mean Squared Error (MSE), Cross-Entropy Loss (or Log Loss), end of thinking capacity of my model 😂😂

### Mean Squared Error (MSE)
Used for regression problems, it calculates the average squared difference between the predicted and actual values.


<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/8064c840-129f-4ca3-b865-4e272c859be8">


### Cross-Entropy Loss (or Log Loss)
Commonly used for classification problems, particularly in logistic regression and neural networks. It measures the difference between predicted probabilities and actual class labels.

### Hinge Loss
Often used for support vector machines (SVMs) and other classifiers. It penalizes misclassifications based on a margin.

### Categorical Cross-Entropy Loss
Similar to cross-entropy loss, but specifically designed for multi-class classification problems.

## Basic Maths/Stats
### Mean
The Mean is the **average** of set of numbers.
For example for dataset[5, 7, 10, 12, 15], the mean is (5 + 7 + 10 + 12 + 15) / 5 = 9.8.
Mean is sensitive to outliers for example if there are 2 software engineers of pay of 1000 USD and 1800 USD there **Mean** will be 1250 that is correct but what if we have a CEO and he earns 1000000 USD than the average will be alot(drastically). We should not use **mean** when data is **Skewed or uneven**. We ML Engineers stay away from Mean as far as we can unless data is not skewed.

### Median
Median is the middle value in a sorted dataset. For example with dataset[3, 5, 6, 8, 9] the median will be 6. Similarly for dataset[2, 4, 6, 8] the median is (4+2) / 2 = 5 
Unlike Mean, Median is usefull for ML because Median is not sensitive towards outliers. Whenever we don't know about data we should always use Median 😂, in other words we should always use Median. Median is used to chopp only 2 times for 4 times we use something that is called ****Quartiles****

### Mode
Mode is the value that appears most frequently in a dataset. A dataset can have one mode, more than one mode(multi-modal) or no mode. We also try to stay away from it 😳 because it **effect compute power** we never know how many mode we have, a data can have many values that are frequently present in the dataset.
Example 1: dataset[3, 4, 4, 6, 8], the mode is **4**.
Example 2: dataset[1,2,3,4,5], there is **no mode**.

## Quartiles and Interquartile Range (IQR)
**Quartiles**: Before understanding the IQR, we need to grasp the concept of quartiles.

**Quartiles** divide a dataset into four equal parts, each representing a quarter **(25%)** of the data. They're useful for understanding the distribution of values within a dataset.
- The first quartiles **(Q1)** is the value below which **25%** of data falls.
- The Second quartile **(Q2)** is the value below which **50** of data falls. It's actually Median.
- The third quartile **(Q3)** is the value below which **75%** of data falls.

#### Interquartile Range 
Interquartile Range is **Q2 - Q1 or Q2 - Q3, etc** meaning number beween Quartiles. E.g how many people there were between 25% and 75% or 25% and 50% is called IQR.
We can also find outliears using IQR.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/3a969b32-67c6-4312-a1d9-62affeb1d218">

Using Prebuild pandas function
```
Q1 = df.quantile(0.25)
Q3 = df.quantile(0.75)
IQR = Q3- Q1
print('IQR: ', IQR)
```

Using Custom code
```
arr = [10, 2000, 3000, 4000, 5000, 6000, 7000, 8000, 9000,10000, 13500, 50000]
arr = pd.Series(arr)
Q1 = arr[arr < 6500].median()
Q3 = arr[arr > 6500].median()
IQR = Q3 - Q1
print("Q1 Median: ", Q1)
print("Q3  Median: ", Q3 )
print("IQR: ", IQR)

lower_bound = Q1 - 1.5 * IQR
upper_bound = Q3 + 1.5 * IQR
print('lower_bound', lower_bound)
print('upper_bound', upper_bound)

outliers = [x for x in arr if x < lower_bound or x > upper_bound]
print("Outliers:", outliers)
```
Finding basic Interquartile Range and outliears.
Output is:

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/17d54d0f-5f03-4a12-9afe-2373bebae9d3">

We can also find the Q1, Q2, Q3 and outlinears using boxplot
```
sns.boxplot(x=df['Engine Size(L)'])
```

## Five Number Summary
Five Number summary is min, max q1, q2, q3

# Scaling data, evaluating models on data

## Min-Max Scaling
Min-Max Scaling is a data **normalization** technique used to **transform data** into a **specific range**. Normalization is a best practice that should be done as it
decreases computation power. Min-Max scaling converts data into 0s and 1s.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/2ef1d08a-0250-4224-8e44-b61650fa0dc0">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/5fbfbe7a-3471-4a20-b3d2-05f4219719ff">


## Z-Score scaling
Z-Score Scaling, also known as **standardization**, is a technique used to **transform data** into a standard normal distribution.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/076007f6-6b9f-49b6-ab1d-751b516d4b2b">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/7a234d06-a66f-4877-8520-c54980ecaf78">

## Accuracy
It only applies to classification. It is the ratio of correct predictions to the total number of input samples.
If target variable is **imbalance** we should not use Accuracy rather there are other techniques for evaluating the classification model i.e **evaluation matrix**

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/8def7ef8-cbbe-491e-a27c-7f43a7744759">


**Note:** It works well only if there are **equal** number of samples belonging to each class/category.

## Imbalance Data/Class Imbalance
Imbalanced data refers to those types of datasets where the target class has an uneven distribution of observations, i.e one class label has a very high number of observations, and the other has a very low number of observations. Imbalance data is always in categories e.g person is human or alien, more persons are human while
less are alien. Let's say 98% of people are human while 2% are aliens this creates a class imbalance.

## Skewed Data 
A training dataset is said to be skewed if the distribution of its target variable is uneven around its mean value. Skewed data is numerical.
