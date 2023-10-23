tags:: Algorithmics
topic:: Problems
algo:: Unit 4 Outcome 2

-
- using [[Recursion]] you can find the Fibonacci number by first finding the previous two Fibonacci numbers
	- ```
	  Algorithm fibonacci_recursive(n)
	  	// Recursive fibonacci algorithm
	      If n = 0 Then
	          Return 0
	      Else If n = 1 Then
	          Return 1
	      Else
	          Return fibonacci(n - 1) + fibonacci(n - 2)
	      End If
	  End
	  ```
- The Fibonacci numbers have [[Optimal Substructure]] because the optimal solution to the Fibonacci number problem can be obtained by combining optimal solutions to the subproblems of the Fibonacci number problem.
- one [[Dynamic Programming]] solution to the Fibonacci number problem works by storing the solutions to the subproblems in a table using a [[Bottom-Up]] approach.
- The table is indexed by the Fibonacci numbers, and the value in each cell of the table is the Fibonacci number itself.
	- ```
	  Algorithm fibonacci_bottom_up(n)
	  	// Dynamic programming version of fibonacci algorithm
	      table <-- dict() // use a dictionary to store the subproblem solutions
	      table[0] <-- 0
	      table[1] <-- 1
	      For i in 2 to n + 1 Do
	          table[i] <-- table[i - 1] + table[i - 2]
	      End For
	      Return table[n]
	  End
	  ```
- The dynamic programming solution to the Fibonacci number problem is more efficient than the recursive solution because it only computes the Fibonacci numbers for the subproblems that are actually needed.
- The recursive solution, on the other hand, computes the Fibonacci numbers for all of the subproblems, even the ones that have been solved in other recursive steps.
- Another solution that makes use of [[Memoization]] uses a recursive function inside the algorithm to allow for the 'cache' of results to exist and be used by the function
	- id:: 6530508e-d044-436e-ad90-48707fd26832
	  ```
	  Algorithm fibonacci_memoization(n)
	  	// Dynamic programming version using memoization
	      
	      // Uses an ADT to create a cache for subproblems
	      cache <-- new dictionary
	      
	      Function fibonacci(n)
	      	If n = 0 or n = 1 Then
	  	        Return n
	      	Else
	          	If n in cache Then
	              	Return cache[n]
	          	Else
	              	result <-- fibonacci(n - 1) + fibonacci(n - 2)
	              	cache[n] <-- result
	              	Return result
	          	End If
	      	End If
	      End Function
	  End
	  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Fibonacci sequence - Rosetta Code](https://www.rosettacode.org/wiki/Fibonacci_sequence)