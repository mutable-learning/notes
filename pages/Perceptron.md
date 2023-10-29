tags:: Algorithmics
alias:: Multi-layer Perceptron, MLP
topic:: [[Neural Network]]
algo:: Unit 4 Outcome 3

-
- is a feedforward Artificial [[Neural Network]] (ANN) that consists of multiple layers of interconnected nodes
	- nodes in each layer are connected to the nodes in the next layer, and the connections have weights that are adjusted during training along with bias values that are applied
	- inputs travel forward through the layers using [[Forward Propagation]]
- has three main layers
	- input layer
		- receives the input data (features)
	- hidden layer(s)
		- performs the actual computation
		- the number of hidden layers can be one or more
	- output layer
		- produces the output of the network
- nodes in each layer are called neurons
- each neuron has a weighted sum of the inputs from the previous layer, and an activation function that determines the output of the neuron
- the activation function is a non-linear function that allows the MLP to learn more complex relationships between the input and output data
- the MLP is trained in a process described in [[Neural Network/Training]]
- trained by adjusting the weights so that the output of the network is as close as possible to the desired output for the given input
- ![Mult-layer Perceptron](https://i.stack.imgur.com/5SkqL.png)
-
-
- Further Research
  background-color:: purple
	- Read
		- [Perceptron - Wikipedia](https://en.wikipedia.org/wiki/Perceptron)
	- Watch
		- {{video https://www.youtube.com/watch?v=7YaqzpitBXw}}
		- {{video https://www.youtube.com/watch?v=AZEfmoWBXwg}}