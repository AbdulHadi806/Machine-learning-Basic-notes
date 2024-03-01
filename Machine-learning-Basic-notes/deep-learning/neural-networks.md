# Neural Networks

# Regular Neural Network(ANN)
Regular Neural Network also known as ANN(Artificial Neural Network) is the most common type of neural network. It has three types of layers: input, hidden, and output. In ANN
units from one layer are connected to another. Each connection has weights that determine the influence of one unit on another unit. As the data transfers from one
unit to another, the neural network learns more and more about the data which eventually results in an output from the output layer.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/47b0bfe0-9043-474a-8080-0e693ce806c7">

The input layer in ANN receives the input from external sources and releases it to the hidden layer, which is the second layer. In the hidden layer, each neuron receives input from prev layer neurons, computes the weighted sum, and sends it to the neurons in the next layer.

### CNN(convolution neural network)

CNN, or Convolutional Neural Network, is primarily used for computer vision tasks. It operates similarly to our brain: imagine encountering a new object like a bottle. 
Like our brain, CNN first examines simple features like color, weight, and shape to understand it. Then, it progressively analyzes more complex details, 
identifying patterns along the way. In simple terms, CNN creates a basic image, gradually adding layers of complexity to recognize and understand visual information.

**CNN** has **four layers** input layer => convolutional layer => Pooling layer => connected layer

[CNN awesome blog](https://www.geeksforgeeks.org/introduction-convolution-neural-network/)

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/f9ff45a7-e3c3-49bb-80b5-609eccdc5153">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/3d1eac22-1c70-4fbc-a66c-d6c936fbd598">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/edf015cd-6c30-4915-ab7e-33c46169e7f4">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/f474ddcc-8a09-4b94-a38a-9d4dd30d9f5b">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/2ba94d6c-f226-4d9e-b494-b85487bd0a43">

##### Pooling

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/637724c3-ef62-4036-91bf-a6822a432168">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/c0604d83-90dc-4ca5-9305-b0eb3eb30f80">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/1b3e03b2-eb6e-4532-825f-0dc347df9602">


### Autoencoders
AutoEncoders has two main parts encoder and decoder. The encoder part compresses the input data into lower-dimensional 
representation, typically using convolutional layers to capture important features. The **decoder** part reconstructs the original input from the compressed representation,
often employing transposed convolutional layer or upsampleing layers.

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/0ee350ef-7f31-4ad7-b021-5d7b2bb67f74">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/0104ea8c-a847-4680-8f5b-196643c7c869">

###### What are encoders and decoders?

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/ab50e3ed-f4b9-4629-bedb-3f2637505df4">

