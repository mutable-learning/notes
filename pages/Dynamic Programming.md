tags:: Algorithmics
topic:: [[Advanced Algorithm Design]]
algo:: Unit 4 Outcome 2

-
- an algorithmic technique for solving problems by breaking them down into smaller subproblems and using the solutions to those subproblems to solve the original problem.
- good for solving problems with an [[Optimal Substructure]] or [[Overlapping Subproblems]].
- works by storing the solutions to the subproblems in a table.
	- the table is indexed by the subproblems, and the value in each cell of the table is the solution to the subproblem.
- to solve a problem using dynamic programming
	- we first initialize the table with the solutions to the base cases.
	- we recursively solve the subproblems, using the solutions to the subproblems that we have already solved.
	- the final solution to the problem is the value in the table that corresponds to the original problem.
- it can be difficult to implement.
	- the main difficulty is that we need to identify the subproblems and the base cases.
	- *once we have identified the subproblems and the base cases*, the implementation of dynamic programming is relatively straightforward.
- Here are some examples of problems that can be solved using dynamic programming:
	- **Fibonacci numbers**
		- The Fibonacci numbers are a sequence of numbers where each number is the sum of the two previous numbers.
		- The Fibonacci numbers can be computed recursively, but they can also be computed using dynamic programming.
	- **Longest common subsequence**
		- The longest common subsequence of two strings is the longest sequence of characters that appears in both strings.
	- **Edit distance**
		- The edit distance between two strings is the minimum number of changes that need to be made to one string to make it the same as the other string.
- is a good choice of algorithm if the problem can be solved by solving its subproblems or if the subproblems are used to solve the problem multiple times.
-
- Further Research
  background-color:: purple
	- Read
		- [Dynamic programming - Wikipedia](https://en.wikipedia.org/wiki/Dynamic_programming)
	- Watch
		- {{video https://www.youtube.com/watch?v=P8Xa2BitN3I&pp=ygUTZHluYW1pYyBwcm9ncmFtbWluZw%3D%3D}}
		- {{video https://www.youtube.com/watch?v=aPQY__2H3tE&pp=ygUTZHluYW1pYyBwcm9ncmFtbWluZw%3D%3D}}
-
-