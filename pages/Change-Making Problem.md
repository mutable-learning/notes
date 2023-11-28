tags:: Algorithmics
alias:: Coin-Change Problem
topic:: [[Problems]]
algo:: Unit 4 Outcome 2

-
- asks you to find the minimum number of coins (of certain denominations) that add up to a given amount of money. It is a special case of the integer knapsack problem.
	- if you need to make change for $1.00 using pennies, nickels, dimes, and quarters, then the minimum number of coins needed is 4, as you could use 4 quarters.
- has both [[Optimal Substructure]] and [[Overlapping Subproblems]] , as you can use the solutions to the subproblems multiple times to solve other problems.
- to solve the problem using [[Dynamic Programming]]
	- first initialize the table with the solutions to the base cases.
	- the base cases are
		- when the amount of change is 0, so the minimum number of coins needed is 0
		- when the amount of change is less than the smallest denomination of coin, so the minimum number of coins needed is infinity.
	- recursively fill in the table by finding the minimum number of coins needed to make the amount of change in the cell, using the solutions to the subproblems that are stored in the table.
		- the final solution to the problem is the value in the table that corresponds to the amount of change that we need to make.
- the dynamic programming solution to the change-making problem is more efficient than the recursive solution because it only solves the subproblems that are actually needed.
- the recursive solution, on the other hand, solves the subproblems for every amount of change, even the amounts of change that are not possible.
- Coin values can be modelled by a set of $n$ distinct positive integer values, arranged in increasing order as $w_1$ through $w_n$.
	- given an amount $W$, also a positive integer, to find a set of non-negative (positive or zero) integers $\{x_1, x_2,\dots, x_n\}$, with each $x_j$ representing how often the coin with value $w_j$ is used, which minimize the total number of coins $f(W)$
	- $$
	  f(W) = \sum^{n}_{j=1}x_j \\
	  \text{subject to} \\
	  \sum^{n}_{j=1}w_jx_j = W
	  $$
-
- Here is a simple algorithm that uses an array to store the answers for each subproblem up to the desired $W$ amount
	- ```
	  Algorithm change_making(amount, denominations):
	      table <-- []
	      table[0] <-- 0
	      For x <-- 1 To amount DO
	          table.append(∞)
	      End For
	      For i <-- 1 To amount DO
	          For each coin in denominations Do
	              If i >= coin Then
	                  table[i]<-- min(table[i], table[i - coin] + 1)
	              End If
	          End For
	      End For
	      return table[amount]
	  End
	  ```
- For each amount from 1 to amount, the minimum number of coins needed is computed by iterating over all denominations and checking if the current denomination can be used to make change for the current amount.
-
- Further Research
  background-color:: purple
	- Read
		- [Find minimum number of coins that make a given value - Rosetta Code](https://www.rosettacode.org/wiki/Find_minimum_number_of_coins_that_make_a_given_value)