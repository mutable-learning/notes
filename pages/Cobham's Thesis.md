tags:: Algorithmics
alias:: Cobham-Edmonds Thesis
topic:: [[Computer Science]]
algo:: Unit 4 Outcome 3

-
- named after Alan Cobham and Jack Edmonds, who first proposed it in the early 1960s
- is a statement about the feasibility of computational problems
- asserts that computational problems can be feasibly computed on some computational device only if they can be computed in polynomial time
	- if a problem can be solved by an algorithm that runs in polynomial time, then it is considered to be a feasible problem
- Cobham's Thesis strengths
	- it provides a clear and concise definition of what it means for a problem to be *feasible*
	- it suggests that there is a fundamental limit to what can be computed in practice.
	- it has helped to guide the development of new algorithms and to identify problems that are likely to be intractable
- Cobham's Thesis limitations
	- it does not take into account the constant factors in the running time of algorithms and lower order terms
	- it ignores the size of the exponent
		- an algorithm with a polynomial running time may still be infeasible if the constant factor is large
	- does not apply to problems that are defined over infinite inputs
	- under Cobham's thesis, a problem for which the best algorithm takes $n^{200}$ instructions is considered feasible, and a problem with an algorithm that takes $2^{0.00001 n}$ instructions infeasible—even though one could never solve an instance of size $n = 2$ with the former algorithm, whereas an instance of the latter problem of size $n = 10^6$ could be solved without difficulty
- relationship between the [[Church-Turing Thesis]] and Cobham's thesis
	- the [[Church-Turing Thesis]] establishes a limit on what can be **computed**
		- any [[Algorithm]] that can be executed by a human or another computing device can also be executed by a [[Turing Machine]]
		- it does not say anything about the *feasibility* of computing particular problems
	- Cobham's thesis refines the [[Church-Turing thesis]]
		- only problems that can be computed in polynomial time are **feasible**
			- even if a problem can be solved by a [[Turing Machine]] , it may still be *infeasible* if it takes too long to compute the solution
-
- Further Research
  background-color:: purple
	- Read
		- [Cobham's thesis - Wikipedia](https://en.wikipedia.org/wiki/Cobham's_thesis)