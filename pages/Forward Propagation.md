tags:: Algorithmics
topic:: [[Neural Network]]
algo:: Unit 4 Outcome3

-
- is the process of passing data through each [[Perceptron]] that makes up a [[neural network]] from the input layer to the output layer
- is a feedforward process, which means that the data flows in one direction only
- forward propagation steps
	- multiply the input data by the weights of the connections between the input layer and the first hidden layer (weighted sum)
	- pass the weighted sum through an activation function, which determines the output of the neuron
	- the activation function is usually a non-linear function, such as the sigmoid function or the ReLU function
	- the output of the first hidden layer is then multiplied by the weights of the connections between the first hidden layer and the second hidden layer
	- repeat for each hidden layer.
	- the output of the last hidden layer is then multiplied by the weights of the connections between the last hidden layer and the output layer
		- this is the final output of the neural network
- the process is repeated for each epoch
	- an epoch is one pass through the entire training dataset
- each [[neural network]] is trained by adjusting the weights of the connections between the neurons so that the output of the network is as close as possible to the desired output for the given input
- works in conjunction with backward propagation during the [[Neural Network/Training]] process before accurate predictions can be made (inferred) on test and novel data sets
- is used in both training and inference
-
- Further Research
  background-color:: purple
	- Read
		- [Feedforward neural network - Wikipedia](https://en.wikipedia.org/wiki/Feedforward_neural_network)
	- Watch
		- {{video https://www.youtube.com/watch?v=sNTtUV9yE_M}}