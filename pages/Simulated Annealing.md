tags:: Algorithmics
topic:: Advanced Algorithm Design
algo:: Unit 4 Outcome 2

-
- Simulated annealing is a heuristic optimization algorithm that is inspired by the annealing process in metallurgy. In metallurgy, annealing is a process of heating a metal to a high temperature and then slowly cooling it down. This process allows the metal to reach a more stable state with fewer defects.
- The algorithm starts with a random solution to a problem and then iteratively improves the solution by making small changes.
- However, unlike other optimization algorithms, simulated annealing also allows the solution to get worse at some points. This is done with a probability that decreases as the algorithm progresses.
- The idea is that by allowing the solution to get worse at some points, the algorithm is more likely to find a Global Optimum rather than a Local Optimum.
- Here is an example of how simulated annealing can be used to solve a problem
	- Let's say we want to find the shortest path between two points on a map. We can represent the map as a graph, where each node represents a point on the map and each edge represents a connection between two points.
	- The algorithm would start with a random path between the two points.
	- It would then iteratively improve the path by making small changes. For example, it might swap two edges in the path or add a new edge.
	- However, the algorithm would also allow the path to get worse at some points.
		- This is done with a probability that decreases as the algorithm progresses.
		- The probability of allowing the path to get worse is initially high, but it decreases as the algorithm gets closer to the global optimum.
	- The algorithm would continue to improve the path until it reaches a point where it is very unlikely to find a better path.
	- At this point, the algorithm would stop and return the path.
- The reason probability of accepting a worse solution decreases as the algorithm progresses is because the algorithm is more likely to be near the Global Optimum as it progresses, and therefore less likely to find a better solution by accepting a worse solution.
- The probability of accepting a worse solution is usually defined as a function of the temperature of the system.
	- The temperature of the system is a measure of how likely the algorithm is to accept a worse solution.
	- The temperature is initially high, which means that the algorithm is more likely to accept worse solutions.
	- As the algorithm progresses, the temperature decreases, which means that the algorithm is less likely to accept worse solutions.
	- The temperature of the system is usually decreased exponentially. The temperature decreases by a constant factor at each step.
	- The constant factor is usually chosen to be between 0.5 and 0.9.
- The decreasing probability of accepting a worse solution helps to ensure that the algorithm does not get stuck in a local optimum. If the probability of accepting a worse solution was always high, the algorithm would be more likely to get stuck in a local optimum.
- The decreasing probability of accepting a worse solution also helps to ensure that the algorithm terminates in a reasonable amount of time. If the probability of accepting a worse solution was always high, the algorithm could potentially continue to run forever, searching for a better solution that does not exist.
-
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- b