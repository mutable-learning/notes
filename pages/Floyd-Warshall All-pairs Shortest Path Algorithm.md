tags:: Algorithmics
alias:: Floyd-Warshall
topic:: Graph Traversal
algo:: Unit 3 Outcome 2

-
- similar to the [[Transitive Closure]] algorithm
- finds the shortest path by creating a matrix to hold the distances between each node
- distances are updated by going through an intermediate node, if the distance can be shortened by doing so
- an example of [[Dynamic Programming]] , where intermediate values are stored on the way to the overall solution
- ```
  Algorithm FWShortestPath(G)
  	// Given a graph as input the output is a matrix
  	// of size |V| x |V| size of the minimum distances
  	// between pairs of nodes
  	D <-- empty integer matrix of size |V| x |V|
  	
  	// Set initial distances to infinity
  	For i <-- 1 to |V| Do
  		For j <-- 1 to |V| Do
  			 D[i,j] <-- ∞
          End For
      End For
  	
  	For i <-- 1 to |V| Do
  		D[i,i] <-- 0 //distance of node to itself
      End For
  	
  	For each edge(u-v) in G Do
  		D[u,v] <-- weigth(u-v) // start with the edge weights
      End For
  	 
  	// Now adjust weights in the matrix using intermediate nodes
  	For k <-- 1 to |V| Do
  		For i <-- 1 to |V| Do
  			For j <-- 1 to |V| Do
  				// is it shorter to go through k to get to j from i
  				If D[i,j] > (D[i,k] + D[k,j]) Then
  					D[i,j] <-- D[i,k] + D[k,j]
                  End If
              End For
          End For
      End For
      Return D
  End
  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Floyd–Warshall algorithm - Wikipedia](https://en.wikipedia.org/wiki/Floyd%E2%80%93Warshall_algorithm)
	- Watch
		- {{video https://www.youtube.com/watch?v=4OQeCuLYj-4&pp=ygUOZmxveWQtd2Fyc2hhbGw%3D}}
		- {{video https://www.youtube.com/watch?v=4NQ3HnhyNfQ&pp=ygUOZmxveWQtd2Fyc2hhbGw%3D}}