tags:: Algorithmics, Algorithm

- Used to find the [[MST]] for a weighted, connected graph
- Uses a minimum [[Priority Queue]] to hold the possible edges (with the weight as the priority)
- When the set of nodes in the tree is equal to the set of graph nodes the MST is complete
- Steps to follow using a priority queue
	- Create a new tree with any node from the graph to start
	- Add all edges incident to the tree node to the priority queue
	- Dequeue the edge with the minimum weight from the queue (min priority)
	- Make sure the nodes in the edge are not already in the set of tree nodes
	- Add the edge to the tree
	- Repeat from step 2 until the set of tree nodes is the equal to the set of graph nodes
- Pseudocode
	- ```
	  Algorithm prim(G, v0)
	  	// G is a weighted graph with vertices (V) and edges (E)
	      // v0 is any random vertice in V
	      // Output will be an MST
	      
	      T ← new empty Graph
	      Add v0 to T
	      While T.vertices does not equal G.vertices Do
	      	Choose minimal weighted edge u-v where u is in T and v is not
	          Add u-v to T
	      End While
	  End
	  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Prim's algorithm - Wikipedia](https://en.wikipedia.org/wiki/Prim%27s_algorithm)
	- Watch
		- {{video https://www.youtube.com/watch?v=cplfcGZmX7I&pp=ygUQcHJpbSdzIGFsZ29yaXRobQ%3D%3D}}
		- {{video https://www.youtube.com/watch?v=jsmMtJpPnhU&pp=ygUQcHJpbSdzIGFsZ29yaXRobQ%3D%3D}}