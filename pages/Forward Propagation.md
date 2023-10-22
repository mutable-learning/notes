tags:: Algorithmics
topic:: [[Neural Network]]
algo:: Unit 4 Outcome3

-
- Forward propagation is the process of passing data through a neural network from the input layer to the output layer. It is a feedforward process, which means that the data flows in one direction only.
- The steps in forward propagation are↓
	- multiply the input data by the weights of the connections between the input layer and the first hidden layer (weighted sum)
	- pass the weighted sum through an activation function, which determines the output of the neuron (the activation function is usually a non-linear function, such as the sigmoid function or the ReLU function)
	- the output of the first hidden layer is then multiplied by the weights of the connections between the first hidden layer and the second hidden layer.
	- This process is repeated for each hidden layer.
	- The output of the last hidden layer is then multiplied by the weights of the connections between the last hidden layer and the output layer. This is the final output of the neural network.
- The forward propagation process is repeated for each epoch. An epoch is one pass through the entire training dataset. The neural network is trained by adjusting the weights of the connections between the neurons so that the output of the network is as close as possible to the desired output for the given input.
- Forward propagation is a fundamental process in neural networks. It is used to pass data through the network and to calculate the output of the network. Forward propagation is used in both training and inference.
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- b