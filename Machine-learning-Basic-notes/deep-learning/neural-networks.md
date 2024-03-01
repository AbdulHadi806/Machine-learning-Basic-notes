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
An autoencoder is a type of neural network that is trained to copy its input to its output. It consists of two parts: an encoder and a decoder. The encoder transforms the input data into a lower dimensional representation, which is often called the hidden layer, the latent space, or the code. The decoder reconstructs the input data from the hidden layer. The hidden layer is not necessarily in the middle of the encoder and decoder, but it is the layer with the smallest dimensionality. The goal of an autoencoder is to learn an efficient representation of the input data, which can be used for dimensionality reduction, data compression, feature extraction, or generative modeling.

[Autoencoders awesome blog](https://www.geeksforgeeks.org/auto-encoders/)

Some examples of autoencoders are:

•  Sparse autoencoder: This type of autoencoder adds a sparsity constraint to the hidden layer, forcing it to have a small number of active units. This encourages the autoencoder to learn more meaningful and robust features.https://www.geeksforgeeks.org/auto-encoders/

•  Denoising autoencoder: This type of autoencoder adds noise to the input data and trains the autoencoder to recover the original data from the noisy input. This helps the autoencoder to learn more robust and invariant features.
https://www.geeksforgeeks.org/auto-encoders/

•  Variational autoencoder: This type of autoencoder models the hidden layer as a probabilistic distribution and trains the autoencoder to maximize the likelihood of the input data given the hidden layer. This allows the autoencoder to generate new data that is similar to the input data.
https://www.tensorflow.org/tutorials/generative/autoencoderhttps://www.analyticsvidhya.com/blog/2021/06/autoencoders-a-gentle-introduction/

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/0ee350ef-7f31-4ad7-b021-5d7b2bb67f74">

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/0104ea8c-a847-4680-8f5b-196643c7c869">

##### What are encoders and decoders?

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/ab50e3ed-f4b9-4629-bedb-3f2637505df4">

##### Encoding process

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/7e30b19a-dd47-49ca-b276-d2974e8eb8a3">

Why is it important?

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/2642b591-ecbf-4142-84be-02796ee464dd">

##### Decoding process

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/41ddaef7-8ec4-4252-a95b-d178b08bd33c">



<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/7d7e7339-ed1a-4e58-bffe-8aa4c3ec965e">
