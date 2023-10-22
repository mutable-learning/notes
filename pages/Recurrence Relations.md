tags:: Algorithmics
topic:: [[Algorithm Analysis]]
algo:: Unit 4 Outcome 1

-
- A recurrence relation is an equation that calculates a term by using the previous term(s).
- It uses an initial or seed value(s) to start the recurrence.
- Steps to create a recurrent relation for a recursive algorithm
	- Identify the base case. This is the case where the recursive algorithm does not need to call itself. For example, the base case for the Fibonacci sequence is when the input is 0 or 1.
	- Identify the recursive step. This is the step where the recursive algorithm calls itself. For example, the recursive step for the Fibonacci sequence is to calculate the Fibonacci numbers for the input minus 1 and the input minus 2, and then add the two results together.
	- Write the recurrence relation. The recurrence relation is an expression that describes the running time of the recursive algorithm. It will usually have the following form:
	  T(n) = a * T(n/b) + c  where
		- T(n) is the running time of the recursive algorithm on input n
		- a is a constant that represents the time it takes to do the recursive step
		- c is a constant that represents the time it takes to do the base case
		- b is a constant that represents the size of the input after the recursive step
	- However, for VCE Algorithmics we only are concerned with recurrent relations of the form:
	  
	  T(n) = \sum {^k_{i=1}}\ T(n-a_i)+b\ \text{where}\ a_i\in N
		- T(n) is the running time of the algorithm
		- k is a constant
		- a_i are the set of integers that are not all equal to each other
		- b is a constant that represents the time it takes to do the base case
		- N represents the input size
	- Solve the recurrence relation. There are a few different ways to solve a recurrence relation. One way is to use the Master Theorem. Another way is to use back substitution.
- Here is an example of how to create a recurrent relation for the Fibonacci sequence:
- The base case for the Fibonacci sequence is when the input is 0 or 1. The recursive step is to calculate the Fibonacci numbers for the input minus 1 and the input minus 2, and then add the two results together. So, the recurrence relation for the Fibonacci sequence is:
- T(n) = T(n-1) + T(n-2)
- This recurrence relation can be solved using the Master Theorem. The solution is that T(n) is O(φ^n), where φ is the golden ratio.
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- b