tags:: Algorithmics
alias:: n-Queens Problem

-
- a classic problem in computer science that asks how to place $n$ queens on an n x n chessboard so that no two queens attack each other.
	- a queen can attack another queen if they are on the same row, column, or diagonal.
- an example of a backtracking algorithm for the n-Queens problem is listed below using a modularised iterative approach
	- ```
	  Algorithm under_attack(col, queens)
	      i <-- 0
	      For x in queens Do
	          If col = x or abs(col - x) = length(queens) - i Then
	              Return True
	          End If
	          i <-- i + 1
	      End For
	      Return false
	  End
	  
	  
	  Algorithm solve(n)
	      solutions = [[]] // empty nested list
	      For row <-- 0 to n-1 Do
	          new_solutions <-- []
	          For solution in solutions Do
	              For i <-- 0 to n-1 Do
	                  If not under_attack(i + 1, solution) Then
	                      new_solutions.append(solution + [i + 1])
	                  End If
	              End For
	          End For
	          solutions <-- new_solutions
	      End For
	      Return solutions
	  End
	  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Eight queens puzzle - Wikipedia](https://en.wikipedia.org/wiki/Eight_queens_puzzle)
	- Watch
		- {{video https://www.youtube.com/watch?v=jPcBU0Z2Hj8&pp=ygUQbi1xdWVlbnMgcHJvYmxlbQ%3D%3D}}