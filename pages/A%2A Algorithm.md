tags:: Algorithmics
topic:: [[Advanced Algorithm Design]]
algo:: Unit 4 Outcome 2

-
- is a graph traversal and path search algorithm used to find the shortest path between two nodes in a weighted [[Graph]]
- is an informed search algorithm
	- it uses a [[heuristic]] function to estimate the cost of the remaining path from a given node to the goal node
	- this [[Heuristic]] helps A* to focus its search on the most promising nodes
	- using the [[Heuristic]] can significantly improve performance
- A* can be used to find the shortest path from the start node (A) to the goal node (B) in a maze by
	- adding the start node to a priority queue
	  logseq.order-list-type:: number
	- remove the node with the lowest estimated cost from the priority queue
	  logseq.order-list-type:: number
		- the current node
		  logseq.order-list-type:: number
	- expands the current node
	  logseq.order-list-type:: number
		- it adds all of its unvisited neighbours to the priority queue
		  logseq.order-list-type:: number
			- unvisited nodes are added by the result of the heuristic function that checks if the node is *getting the algorithm closer to the end goal*
			  logseq.order-list-type:: number
			- for example, edge weight + the result of a [[Heuristic]] function that returns a value indicating the distance from the goal
			  logseq.order-list-type:: number
	- The algorithm repeats steps 2 - 3 until the goal node is reached
	  logseq.order-list-type:: number
- characteristics of A*
	- uses a heuristic function to estimate the cost of the remaining path from a given node to the goal node
	- is a complete algorithm
		- will always find a path to the goal node if one exists
	- is an optimal algorithm
		- will find the shortest path to the goal node if one exists
	- is a relatively efficient algorithm, especially for large graphs
- [[Dijkstra's algorithm]] is another graph traversal algorithm that is often used to find the shortest path between two nodes in a weighted graph
	- [[Dijkstra's Algorithm]] does not use a heuristic function, making it is not as efficient as A*
	- in general, A* will find the shortest path to the goal node faster than Dijkstra's algorithm
		- especially for large graphs.
-
- Further Research
  background-color:: purple
	- Read
		- [A* search algorithm - Wikipedia](https://en.wikipedia.org/wiki/A*_search_algorithm)
		- [Introduction to A*](https://theory.stanford.edu/~amitp/GameProgramming/AStarComparison.html)
	- Watch
		- {{video https://www.youtube.com/watch?v=ySN5Wnu88nE&pp=ygUMYSogYWxnb3JpdGht}}
		- {{video https://www.youtube.com/watch?v=A60q6dcoCjw&pp=ygUMYSogYWxnb3JpdGht}}