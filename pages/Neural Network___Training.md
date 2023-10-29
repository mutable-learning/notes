tags:: Algorithmics
topic:: [[Neural Network]]
algo:: Unit 4 Outcome 3

-
- the usual process of training neural networks is called [[Supervised Learning]]
	- the neural network is given a set of training data, where each data point consists of an input vector and an output vector
	- it learns to map the input vectors to the output vectors by adjusting the weights between the neurons
- the training process for a neural network is iterative
	- the neural network is presented with a data point from the training set, and the output of the network is compared to the desired output
	- the weights of the network are then adjusted so that the output of the network is closer to the desired output in a process called backward propagation
	- this process is repeated for each data point in the training set
- the training process is typically divided into epochs
	- an epoch is one pass through the entire training set
	- the neural network is trained for a number of epochs, and the weights of the network are adjusted after each epoch
- the training process is complete when the neural network has learned to map the input vectors to the output vectors with a high degree of accuracy
- training can be computationally expensive, especially for large neural networks
	- techniques that can be used to speed up the training process
		- using GPUs
		- using regularization techniques
- training can also be unstable
	- the network may not converge to a good solution, or it may converge to a local minima that is not a good solution
	- techniques that can be used to improve the stability of the training process
		- using dropout
		- early stopping.
- the main steps involved in training a neural network
	- choose the network architecture involves deciding on
		- the number of layers
		- the number of neurons in each layer
		- the activation functions to use
	- initialize the weights
		- weights of the network are randomly initialized
	- choose the loss function
		- a function that measures the difference between the output of the network and the desired output
	- choose the optimizer
		- an algorithm that updates the weights of the network to minimize the loss function
	- train the network
		- repeatedly presenting the network with data from the training set and adjusting the weights of the network to minimize the loss function
	- evaluate the network
		- testing the network on a held-out test set to see how well it performs on unseen data
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- b