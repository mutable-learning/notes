tags:: Algorithmics
topic:: [[Advanced Algorithm Design]]
algo:: Unit 4 Outcome 2

-
- A* is a graph traversal and path search algorithm used to find the shortest path between two nodes in a weighted graph.
- It is an informed search algorithm, which means that it uses a heuristic function to estimate the cost of the remaining path from a given node to the goal node.
- This heuristic function helps A* to focus its search on the most promising nodes, which can significantly improve its performance.
- Here is an example of how A* can be used to find the shortest path from the start node (A) to the goal node (B) in a maze:
	- The algorithm starts by adding the start node to a priority queue.
	- It removes the node with the lowest estimated cost from the priority queue. This node is now the current node.
	- It expands the current node, which means that it adds all of its unvisited neighbours to the priority queue.
	- The unvisited nodes are added by the result of the heuristic function that checks if the node is getting the algorithm closer to the end goal (such as edge weight + the result of a function that returns a value indicating the distance from the goal)
	- The algorithm repeats steps 2 -4 until the goal node is reached.
- The main characteristics of A* are:
	- It uses a heuristic function to estimate the cost of the remaining path from a given node to the goal node.
	- It is a complete algorithm. It will always find a path to the goal node if one exists.
	- It is an optimal algorithm. It will find the shortest path to the goal node if one exists.
	- It is a relatively efficient algorithm, especially for large graphs.
- Dijkstra's algorithm is another graph traversal algorithm that is often used to find the shortest path between two nodes in a weighted graph. However, Dijkstra's algorithm does not use a heuristic function, which means that it is not as efficient as A*. In general, A* will find the shortest path to the goal node faster than Dijkstra's algorithm, especially for large graphs.
-
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- b