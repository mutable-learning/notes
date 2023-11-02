tags:: Algorithmics, Software Development
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
  id:: 6540dff6-43ad-4642-80ce-9ed133538ba2
	- to repeat parts of an algorithm a number of times, use iteration and [[Conditional Expressions]]
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
  id:: 6540dff6-c83f-4ca5-893e-e8e22a996848
	- use [[Conditional Expressions]] to test for conditions and run different *branches* of algorithms based on the results of the expressions
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
		- ```
		  Begin
		  	x <-- Create a random number between 1 and 5
		      Switch x
		          Case 1
		          	Print "average"
		          Case 2
		          	Print "good"
		          Case 3
		          	print "excellent"
		          Case 4
		          	Print "outstanding"
		          Case 5
		          	Print "five out of five"
		          Default
		          	Print "not a number between 1 and 5"
		  	End Switch
		  End
		  ```
- Functions
  id:: 6540dff6-8035-491b-a86d-536b2812bfe7
	- use **Algorithm** or **Function** to name blocks of code as functions
	  id:: 6540dff6-9f69-4945-971c-23e8b27ccf13
	- *Call* a function from inside a function or an algorithm
	  id:: 6540dff6-712f-4f55-b0ff-9538d78b25a9
	- ((6530508e-d044-436e-ad90-48707fd26832))
-
- Further Research
  background-color:: purple
	- Read
		- [Pseudocode - Wikipedia](https://en.wikipedia.org/wiki/Pseudocode)
	- Watch
		- {{video https://www.youtube.com/watch?v=eSYeHlwDCNA&pp=ygUTaXRlcmF0aXZlIGFsZ29yaXRobQ%3D%3D}}
		-