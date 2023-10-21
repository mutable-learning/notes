tags:: Algorithmics
topic:: Advanced Algorithm Design
algo:: Unit 4 Outcome 2

-
- Hill climbing is a heuristic search algorithm that starts with a random solution and then iteratively improves the solution by making small changes.
- The changes are chosen based on a heuristic function that evaluates the quality of the solution. This function is used to determine the direction in which the solution should be improved.
- Hill climbing is a local search algorithm, which means that it only considers changes that are close to the current solution.
- This can be an advantage, as it can allow the algorithm to find good solutions quickly. However, it can also be a disadvantage, as it can get stuck in local optima.
- Hill climbing can be used to solve the problem of finding the shortest path between two points on a map
	- The map can be represented as a graph, where each node represents a point on the map and each edge represents a possible path between two points.
	- The heuristic function can be used to estimate the distance between two points.
	- The hill climbing algorithm would start with a random path between the two points.
	- Then, it would iteratively improve the path by making small changes. The changes would be chosen based on the heuristic function, which would estimate the distance between the current path and the shortest possible path.
	- The hill climbing algorithm would continue to improve the path until it could no longer make any improvements.
	- At this point, the algorithm would have found the shortest possible path between the two points.
- Hill climbing can be used to find the best way to pack a suitcase
	- Start with a random packing arrangement
	- Then iteratively improve the arrangement by making small changes.
	- The changes could be made by moving items around in the suitcase or by changing the order in which the items are packed.
	- Continue to improve the packing arrangement until it could no longer make any improvements.
	- At this point, the algorithm would have found the best possible way to pack the suitcase.
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- b