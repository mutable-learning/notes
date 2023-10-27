tags:: Algorithmics
topic:: [[Advanced Algorithm Design]]
algo:: Unit 4 Outcome 2

-
- is a [[heuristic]] search algorithm that starts with a random solution and then iteratively improves the solution by making small changes
- changes are chosen based on a [[heuristic]] function that evaluates the quality of the solution
	- used to determine the direction in which the solution should be improved
- is a local search algorithm
	- it only considers changes that are close to the current solution
	- can be an advantage, as it can allow the algorithm to find good solutions quickly
	- can also be a disadvantage, as it can get stuck in local optima
- can be used to solve the problem of finding the shortest path between two points on a map
	- the map can be represented as a graph
		- each node represents a point on the map
		- each edge represents a possible path between two points
	- the heuristic function will be used to estimate the distance between two points
	- the algorithm starts with a random path between the two points
	- it iteratively improves the path by making small changes
		- each change would be chosen based on the heuristic function
			- estimating the distance between the current path and the shortest possible path
	- continue to improve the path until improvements could not be made
		- the shortest possible path between the two points has been found
- Hill climbing can be used to find the best way to pack a suitcase
	- start with a random packing arrangement
	- iteratively improve the arrangement by making small changes
		- changes could be made by moving items around in the suitcase
		- or by changing the order in which the items are packed
	- continue to improve the packing arrangement until improvements can't be made
	- the best possible way to pack the suitcase has been found
-
- Further Research
  background-color:: purple
	- Read
		- [Hill climbing - Wikipedia](https://en.wikipedia.org/wiki/Hill_climbing)
		- [AI | Search Algorithms | Hill Climbing | Codecademy](https://www.codecademy.com/resources/docs/ai/search-algorithms/hill-climbing)
	- Watch
		- {{video https://www.youtube.com/watch?v=oSdPmxRCWws&pp=ygUUaGlsbCBjbGltYmluZyBzZWFyY2g%3D}}