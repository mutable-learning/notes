tags:: Algorithmics
topic:: [[Dynamic Programming]] 
algo:: Unit 4 Outcome 2

-
- the bottom-up approach in [[Dynamic Programming]] is an algorithmic technique for solving problems by solving smaller subproblems first and then using the solutions to the subproblems to solve the larger problem.
- is an iterative approach
- is often easy to implement because it does not require recursion. However, it can be less efficient than a top-down approach or a Memoization approach because it may require more calculations.
- an example can be see in the algorithm to solve the [[Fibonacci Numbers]]
	- it first stores the Fibonacci numbers for $0$ and $1$
	- for each Fibonacci number from $2$ to $n$, the code calculates the value of the Fibonacci number by adding the values of the two previous Fibonacci numbers stored previously in the list.
	- The code then returns the value of the Fibonacci number for $n$ using the list index.