tags:: Algorithmics
topic:: [[Time Complexity Classes]]
algo:: Unit 4 Outcome 1

-
- NP problems are those that can be verified in polynomial time. This means that the time it takes to verify the correctness of the output o
- f an NP problem grows as a polynomial function of the size of the input.
- Here are some of the characteristics of NP problems:
	- Verifiable
		- NP problems are verifiable, which means that the correctness of the output can be verified in polynomial time. This means that NP problems can be solved by a deterministic algorithm that can check the correctness of the output.
	- NP-hard: NP-hard problems are a subset of NP problems that are at least as hard as any other NP problem. This means that if an NP-hard problem can be solved in polynomial time, then all NP problems can be solved in polynomial time.
	- NP-complete: NP-complete problems are a subset of NP-hard problems that are also in NP. This means that NP-complete problems are both verifiable and at least as hard as any other NP problem.
- Some examples of NP problems include:
	- The traveling salesman problem: The traveling salesman problem is a classic NP-complete problem that asks for the shortest possible route that visits a set of cities.
	- The knapsack problem: The knapsack problem is an NP-complete problem that asks for the most valuable set of items that can fit into a knapsack with a limited weight capacity.
	- The Boolean satisfiability problem: The Boolean satisfiability problem is an NP-complete problem that asks whether a Boolean formula is satisfiable.
- The P versus NP problem is one of the most important unsolved problems in computer science. It asks whether every NP problem can also be solved in polynomial time. If P = NP, then all NP problems can be solved in polynomial time. If P ≠ NP, then there are some NP problems that cannot be solved in polynomial time.