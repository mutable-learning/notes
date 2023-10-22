tags:: Algorithmics
topic:: [[Neural Network]]
algo:: Unit 4 Outcome 3

-
- The process of training neural networks is called supervised learning.
- In supervised learning, the neural network is given a set of training data, where each data point consists of an input vector and an output vector.
- It learns to map the input vectors to the output vectors by adjusting the weights between the neurons.
- The training process for a neural network is iterative↓
	- The neural network is presented with a data point from the training set, and the output of the network is compared to the desired output.
	- The weights of the network are then adjusted so that the output of the network is closer to the desired output.
	- This process is repeated for each data point in the training set.
- The training process is typically divided into epochs. An epoch is one pass through the entire training set. The neural network is trained for a number of epochs, and the weights of the network are adjusted after each epoch.
- The training process is complete when the neural network has learned to map the input vectors to the output vectors with a high degree of accuracy.
- Here are the main steps involved in training a neural network:
	- Choose the network architecture: This involves deciding the number of layers, the number of neurons in each layer, and the activation functions to use.
	- Initialize the weights: The weights of the network are randomly initialized.
	- Choose the loss function: This is a function that measures the difference between the output of the network and the desired output.
	- Choose the optimizer: This is an algorithm that updates the weights of the network to minimize the loss function.
	- Train the network: This involves repeatedly presenting the network with data from the training set and adjusting the weights of the network to minimize the loss function.
	- Evaluate the network: This involves testing the network on a held-out test set to see how well it performs on unseen data.
- The training process can be computationally expensive, especially for large neural networks. There are a number of techniques that can be used to speed up the training process, such as using GPUs and using regularization techniques.
- The training process can also be unstable. This means that the network may not converge to a good solution, or it may converge to a local minima that is not a good solution. There are a number of techniques that can be used to improve the stability of the training process, such as using dropout and early stopping.
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- b