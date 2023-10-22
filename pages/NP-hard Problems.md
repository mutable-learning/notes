tags:: Algorithmics
topic:: [[Time Complexity Classes]]
algo:: Unit 4 Outcome 1

-
- NP-hard problems are a class of decision problems that are at least as hard as any other problem in NP. This means that if an NP-hard problem can be solved in polynomial time, then all NP problems can be solved in polynomial time.
- Here are some of the characteristics of NP-hard problems:
	- Hard to solve
		- NP-hard problems are typically very difficult to solve, even for relatively small inputs. This is because the time it takes to solve an NP-hard problem grows exponentially as the size of the input grows.
	- Verifiable
		- NP-hard problems are verifiable, which means that the correctness of the output can be verified in polynomial time if you have an algorithm that can check the solutions and run in polynomial time. This means that NP-hard problems can be solved by a deterministic algorithm that can check the correctness of the output in polynomial time, but no such algorithm currently exists. Therefore, NP-hard problems can't have solutions verified for correctness in polynomial time.
	- NP-complete↓
		- NP-hard problems are a subset of NP problems that are also in NP. This means that NP-hard problems are both verifiable and at least as hard as any other NP problem.
		- Not all NP-hard problems are in NP-complete, as some are undecidable such as the halting problem.
		- All NP-complete problems are in NP-hard though.