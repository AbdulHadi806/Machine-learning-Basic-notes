# Tensorflow and more

## Dense()
A standard connected neuron layer is called Dense. For hidden layer, parameters are Dense(neurons_count, input_size, activation_function) while for output is 
Dense(neurons_count, activation_function).

## Sequential()
One of the first models in tensorflow. It builds a neural network layer by layer by running a command compile.

**model.compile(loss, metrics, optimizer)** is used to create links between layers of neural network and ultimately create a model.

**optimzer used here is sgd** i.e sgd(stotastic gradient descent)

<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/27f9b346-59a7-42b8-8dd1-81e74fd0c218">

## categorical_crossentropy
Used when the model is needed to predict multiple categories i.e more than 2.

<img width="246" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/a70c9c5d-f41b-4d38-8dc3-2c47f88e3da6">

## Binary_crossentropy

Used when the model is needed to predict binary categories i.e only 2.
