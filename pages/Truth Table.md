tags:: Algorithmics, Software Development
topic:: [[Pseudocode]]
algo:: Unit 3 Outcome 2
softdev:: Unit 3 Outcome 1

-
- use boolean algebra to test and display each combination of values in [[Conditional Expressions]]
- allow for better understanding of how each part of the expression impacts the overall result of the expression
- steps with an expression of $x > 1 \text{ OR } (y = 0 \text{ AND } x = 0)$
	- list all the propositional variables in the expression
		- $x$, $y$, $x > 1$, $y = 0 \text{ AND } x = 0$ along with $x > 1 \text{ OR } (y = 0 \text{ AND } x = 0)$
	- determine the number of rows in the table
		- this is 2 to the power of the number of propositional variables
	- assign truth values (True or False) to each variable in each row
		- alternate True or False for each variable or
		- start with all True and then change one variable to False per subsequent row
	- evaluate all compound statements for each row (AND or OR)
	- tabulate the value of the final compound statement in the last column of the table
		- this will show all possible combinations of truth values for the compound statement
	- | x | y | x > 1 | y = 0 AND x = 0 | x > 1 OR (y = 0 AND x = 0) |
	  |---|---|---|---|---|
	  | 0 | 0 | False | True | True |
	  | 0 | 1 | False | False | False |
	  | 1 | 0 | True | True | True |
	  | 1 | 1 | True | False | True |
	  | 2 | 0 | True | False | True |
	  | 2 | 1 | True | False | True |
	  | 3 | 0 | True | False | True |
	  | 3 | 1 | True | False | True |
		-