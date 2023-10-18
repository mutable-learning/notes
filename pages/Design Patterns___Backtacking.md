tags:: Algorithmics
alias:: Backtracking

-
- an algorithmic technique for solving problems recursively or iteratively by trying to build a solution incrementally, one piece at a time, removing those solutions that fail to satisfy the constraints of the problem at any point in time.
- can also be viewed as an improvement to the [[Brute-Force]] approach
	- it searches for a solution to a problem among all the available options
	- it reduces the number of candidates once it reaches a state where they fail to satisfy constraints
- Backtracking can be applied to [[Tree]] searching
	- starting from the root node, the [[Tree]] is traversed using [[Recursion]]
	- at each node, the algorithm checks if the node is a solution
		- if it is, the solution is found
		- if the node is not a solution, the algorithm recursively explores all of the node's children
		- if none of the children are solutions, the algorithm backtracks to the previous node and tries a different child
	- this process continues until a solution is found or the entire [[tree]] has been explored
- Backtracking can also be applied to problems such as
	- [[n-Queens Problem]]
	- [[Knapsack Problem]]
- Advantages
	- simple and intuitive technique
	- can be used to solve a wide variety of problems
	- guaranteed to find a solution if one exists
- Disadvantages
	- can be inefficient, as it may explore many different paths that do not lead to a solution
	- can be difficult to implement in some cases
	- may not be able to find *all* solutions if the problem has multiple solutions
-
- Further Research
  background-color:: purple
	- Read
		- [Backtracking - Wikipedia](https://en.wikipedia.org/wiki/Backtracking)
	- Watch
		- {{video https://www.youtube.com/watch?v=RnlHPR0lyOE&pp=ygUMYmFja3RyYWNraW5n}}
		- {{video https://www.youtube.com/watch?v=G_UYXzGuqvM&pp=ygUMYmFja3RyYWNraW5n}}