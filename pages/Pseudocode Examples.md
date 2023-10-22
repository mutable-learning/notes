tags:: Algorithmics, SoftDev
topic:: [[Pseudocode]]
algo:: Unit 3 Outcome 2
softdev:: Unit 3

-
- Variables
	- to store a value for use in statements, assign it to a variable
	- use a left arrow ($\leftarrow$) to *assign* the value to the variable
	- variable names should be simple to understand and consistent in the algorithm
	- ```
	  Begin
	  	a <-- 0
	      name <-- "Alan Turing"
	      Print name
	  End
	  ```
- Sequence
	- each line of pseudocode runs in order from top to bottom unless it is part of a control structure
	- each line should have only one purpose or action
	- each line belongs to a block of code and blocks are represented by an indentation level
	- ```
	  Begin
	  	x <-- 0
	      x <-- x + 1
	      Print x
	  End
	  ```
- Iteration
	- to repeat parts of an algorithm a number of times, use iteration
	- run the lines
		- a number of times with a For loop
		- as long as a condition is true with a While loop
		- until a condition is true with a Repeat loop
	- ```
	  Begin
	  	x <-- 0
	      For i <-- 1 to 3 Do
	      	// For loop runs three times
	          x <-- x + i
	      End For
	      While x < 10 Do
	      	// While loop runs whilst x is less than 10
	          Print x
	          x <-- x + 2
	     	End While
	      Repeat
	      	x <-- x - 1
	          Print x
	      Until x = 0 Do
	  End
	  ```
- Conditionals
	- use boolean expressions to test for conditions and run different *branches* of algorithms based on the results of the expressions
		- use If, Else If and Else conditions
		- use AND, OR and NOT in expressions
		- ```
		  Begin
		  	x <-- Create a random number between 1 and 100
		      If x > 50 Then
		      	Print x is big
		      Else If x < 50 AND x > 25 Then
		      	Print x is medium
		      Else
		      	Print x is small
		      End If
		  End
		  ```
- Functions
	- use **Algorithm** or **Function** to name blocks of code as functions
	- *Call* a function from inside a function or an algorithm
	-