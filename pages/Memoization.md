tags:: Algorithmics
alias:: Top-Down
topic:: Dynamic Programming
algo:: Unit 4 Outcome 2

-
- is a [[Dynamic Programming]] optimization technique used to speed up computer programs by storing the results of expensive function calls and returning the cached result when the same inputs occur again.
- This is a type of caching, distinct from other forms of caching such as buffering and page replacement.
- allows the algorithm to avoid re-solving the same subproblems multiple times, which can significantly improve the running time of an algorithm.
- The memoized version of the [[Fibonacci Numbers]] function
	- would store the results of previous Fibonacci calculations in an ADT.
	- it would first check the ADT to see if the result has already been calculated.
	- if the result has already been calculated, the function would simply return the cached result.
	- if the result has not yet been calculated, the function would calculate the result and store it in the ADT.
- the main differences with a [[Bottom-Up]] approach is that [[Memoization]]
	- uses [[Recursion]]
	- requires a *cache* to store subproblem results the recursive function can reference
	- is good for problems with a small set of inputs