tags:: Algorithmics
topic:: [[Time Complexity Classes]]
algo:: Unit 4 Outcome 1

-
- NP-complete problems are a class of decision problems that are both in NP and NP-hard. This means that NP-complete problems are:
	- Verifiable in polynomial time: The correctness of the output of an NP-complete problem can be verified in polynomial time.
	- At least as hard as any other NP problem: If an NP-complete problem can be solved in polynomial time, then all NP problems can be solved in polynomial time.
- In other words, NP-complete problems are the hardest problems in NP. If we can solve any NP-complete problem in polynomial time, then we can solve all NP problems in polynomial time.
- Here are some of the implications of NP-complete problems:
	- NP-complete problems are difficult to solve: NP-complete problems are typically very difficult to solve, even for relatively small inputs. This is because the time it takes to solve an NP-complete problem grows exponentially as the size of the input grows.
	- NP-complete problems are often used as benchmarks: NP-complete problems are often used as benchmarks for the performance of new algorithms. This is because the difficulty of solving an NP-complete problem is well-understood, so it is a good way to compare the performance of different algorithms.
	- NP-complete problems are often used to design approximation algorithms: Approximation algorithms are algorithms that do not find the optimal solution to a problem, but instead find a solution that is close to optimal. NP-complete problems are often used to design approximation algorithms because they provide a good way to measure the quality of the solution.