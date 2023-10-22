tags:: Algorithmics, SoftDev
topic:: Pseudocode
algo:: Unit 3 Outcome 2
softdev:: Unit 3

-
- informal code with a structure and accepted syntax that is used to detail an algorithm in plain English but in a manner similar to code
- useful for developing and defining algorithms before they are implemented in code
- Aims:
	- understanding the intent is most important, not the syntax
	- the reader should be able to understand what each line is doing
	- object names should be consistent throughout the algorithm
	- avoid language specific syntax (such as Python syntax)
	- do one action per line
	- indent statements in blocks to show which statements are grouped together
- Rules:
	- use **Begin** or **Start** to define the start of the algorithm
	- use **End** or **Stop** to denote the end of the algorithm
	- indent each block of code
	- keywords like Read, Open, Print are bold and captilized
	- keywords for loops and conditional statements are bold, capitalized and the block is denoted as finished with a **End If** or **End For** keyword
	- blocks inside keyword structures are indented
	- statements that run as part of the same block are listed at the same indent level
	- variables are defined with a name and the value of a variable is assigned with an arrow
		- for example x <-- 0 is the same as setting x to hold the value of 0
	- '=' is only used to compare a value with another using Boolean algebra.
		- for example x = 1 is a statement that asks if x is equal to 1 and will only result in true or false when the pseudocode is executed.
- Example
	- ```
	  Algorithm direction(n, count)
	      If count > 1
	           If n is divisible by 2
	               Return direction(n + 7, count – 1)
	           Else
	               Return direction((n-1)/2, count – 1)
	           End If
	           If the remainder of dividing n by 4 is 0 Return ‘n’
	           If the remainder of dividing n by 4 is 1 Return ‘e’
	           If the remainder of dividing n by 4 is 2 Return ‘s’
	           If the remainder of dividing n by 4 is 3 Return ‘w’
	      End If
	  End
	  ```