tags:: Algorithmics
alias:: Overlapping Subproblems

-
- a problem has overlapping subproblems if the same subproblems are used to solve multiple instances of the problem.
- if you solve a subproblem for one instance of the problem, you can reuse the solution to that subproblem to solve other instances of the problem.
- [[Dynamic Programming]] can be used to solve problems with overlapping subproblems by storing the solutions to the subproblems in a table.
	- the table is indexed by the subproblems, and the value in each cell of the table is the solution to the subproblem.
	- when a subproblem is encountered, the algorithm first checks the table to see if the solution to the subproblem is already stored.
	- if the solution is already stored, then the algorithm simply uses the stored solution.
	- if the solution is not already stored, then the algorithm solves the subproblem and stores the solution in the table.
- a [[Dynamic Programming]] solution to problems with overlapping subproblems is more efficient than the recursive solution because it only solves the subproblems that are actually needed.
- [[recursion]], on the other hand, solves the subproblems for every instance of the problem, even the ones that have already be solved previously in other recursive step.
- the coin change problem is an example of a problem that can be solved using [[Dynamic Programming]] due to overlapping subproblems.