tags:: Algorithmics, Algorithm

- Traversing a tree or graph
- Start at any node, or the root node (in a tree)
- Explore all neighbours of a node before moving to their neighbours
- Only difference with [[Depth-first Search]] is a [[Queue]] instead of a [[Stack]]
- Steps to follow
	- Start from root node (random for graph)
	- Set node as seen
	- Check each neighbour node
	- If it hasn't been seen, enqueue the node
	- Add node to list of nodes visited
	- dequeue the next node and repeat from step 2
- **Pseudocode**:
	- ```
	  Algorithm BFS(G, root)
	      Let Q be a queue
	      Label root as explored
	      Q.enqueue(root)
	      While Q is not empty Do
	          v <-- Q.dequeue()
	          If v is the goal Then
	              Return v
	          End If
	          For all edges from v to w in G.adjacentEdges(v) Do
	              If w is not labeled as explored Then
	                  Label w as explored
	                  w.parent <-- v
	                  Q.enqueue(w)
	              End If
	          End For
	      End While
	  End
	  ```
	-
-
- Further Research
  background-color:: purple
	- Read
		- [Breadth-first search - Wikipedia](https://en.wikipedia.org/wiki/Breadth-first_search)
	- Watch
		- {{video https://www.youtube.com/watch?v=HZ5YTanv5QE&pp=ygUUYnJlYWR0aC1maXJzdCBzZWFyY2g%3D}}