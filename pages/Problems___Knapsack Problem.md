tags:: Algorithmics
alias:: Knapsack Problem, 0-1 Knapsack Problem

-
- *Given a set of items, each with a weight and a value, determine which items to include in the collection so that the total weight is less than or equal to a given limit and the total value is as large as possible.*
	- this is the optimization version of the problem
	- is NP-hard
		- no known algorithm exists to solve this efficiently
- a decision problem version is also common
	- *Can a value of at least *V* be achieved without exceeding the weight *W*?*
	- is NP-complete
		- a solution can be verified in polynomial time but no algorithm can identify a solution efficiently for any input
- the 0-1 means that you can either take an item or leave it, but not take a fraction of it
- usually you cannot take more than one of each item
- one way to formulate the problem
	- is to use a binary variable for each item, indicating whether it is taken or not
	- the objective function is to maximize the sum of the values of the taken items
		- subject to the constraint that the sum of the weights of the taken items does not exceed the capacity
- is intractable because as there is no known polynomial-time algorithm to solve it exactly.
	- the number of possible combinations of items that we can consider is exponential in the number of items.
	- if we have 10 items, there are $2^{10} = 1,024$ possible combinations of items that we could consider.
	- for relatively small problems, the [[0-1 Knapsack Problem]] can be very difficult to solve.
-
- Further Research
  background-color:: purple
	- Read
		- [Knapsack problem - Wikipedia](https://en.wikipedia.org/wiki/Knapsack_problem)
	- Watch
		- {{video https://www.youtube.com/watch?v=cJ21moQpofY}}