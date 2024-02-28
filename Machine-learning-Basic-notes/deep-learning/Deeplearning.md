# Deep Learning for beginners

## Why deep learning rather than conventional machine learning

Machine learning requires alot of EDA and it cannot process complex information. Deep learning stimulates the working of the human brain, just like a human brain, deep learning provides neurons and collectively they are called a neural network.

Conventional Machine Learning cannot handle complex data. 
For example, in the case of a linear model, we will be unable to draw a best-fit line in the graph below. We can use conventional machine learning when data is not that much complex or the patterns of data are not complex.

<img width="233" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/c3d65f81-f7c1-49cb-8435-8561ee406b51">


Difference between Deep Learning and Machine Learning.

<img width="318" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/045d2944-353f-4129-b36e-4ed11693ae9a">


## Simple Neural Network

Maths functions are called neurons such as Max function. Each neuron even if in the same layer they are responsible for different patterns.
The structure of a simple neural network is as follows: input neuron => hidden layers => output neuron

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/ef62e8b0-d671-4b79-88c6-b01590062e9a">



## Hyper parameters
Hyperparameters are parameters whose values are set before the training and remain constant throughout the training. They are not learned from the data but rather 
they are set using common sense. They are crucial as they control the behavior of the training algorithm and ultimately impact the performance of the model. They are set
by the human himself.

Types of some Hyperparameters
- Learning rate
- Batch Size
- Epochs
- Regularization
- Activation functions

#### Learning Rate
**Learning Rate**: Imagine the blindfolded person descending from a mountain to a valley. The learning rate is like the size of steps the person takes during this descent.

**High Learning Rate**: Taking large steps down the mountain represents a high learning rate. While it helps the person descend quickly, there's a risk of overshooting the valley and ending up on another mountain. Similarly, in machine learning, a high learning rate might cause the model to quickly converge to a solution, but it may also overshoot the optimal solution or fail to converge altogether.

**Low Learning Rate**: Taking small, cautious steps down the mountain represents a low learning rate. The person descends more slowly but is less likely to overshoot the valley and can remember the path. In machine learning, a low learning rate allows the model to make smaller adjustments during training, which can lead to more stable convergence and potentially better performance.

**Finding the right learning rate** is crucial in training machine learning models. Too high, and the model might fail to converge or converge to a suboptimal solution. Too low, and the training process may take an impractical amount of time to reach a satisfactory solution. Techniques like learning rate schedules and adaptive learning rate methods aim to mitigate these challenges by adjusting the learning rate during training based on the model's performance.


<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/9098b3a8-eee3-4e18-ace8-897852afd825">


#### Batch Size
Batch size is like breaking a big problem into smaller pieces. It's similar to studying chapters separately before taking a test on each one, which makes learning easier and quicker for the model.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/ea76eb3d-6847-4e40-a083-ded717ee6aed">

#### Epochs
The number of time the entire training dataset is seen by the model.

<img width="608" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/e83968f1-2b8f-49af-af89-403301ad9173">
