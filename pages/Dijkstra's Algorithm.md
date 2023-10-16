tags:: Algorithmics, Algorithm

- finds the shortest path from a start vertex to all other vertices
- can be used on weighted graphs and directed graphs
- **will not work if there is a negative weight cycle**
- uses a greedy approach to select vertices with minimum weights
- same algorithm but can have different approaches, such as a lazy or eager approach
- can use a [[Priority Queue]] to make implementation easier
- can be used to find the shortest path between vertices if the previous vertex info is stored as the shortest path is determined
- a common modification is to have the algorithm find the longest path length instead of the shortest
- Pseudocode
	- ```
	  Algorithm Dijsktra(G, s)
	  	// Input G is a graph
	  	// Input s is the starting vertex
	  	// Output is the graph with each vertex having attributes
	  	// of distance and predecessor
	  	
	  	For each vertex in G Do
	  		vertex.distance <-- ∞
	  		vertex.predecessor <-- undefined
	  		visited <-- false
	      End For
	   
	  	s.distance <-- 0 // the starting node will be the first one chosen below
	  	
	  	While (there are vertices with visited = False) Do
	  		v <-- vertex with smallest distance and visited = False
	  		For each neighbour of v as u Do
	  			If (v.distance + v-u.weight) < u.distance Then
	  				u.distance <-- v.distance + v-u.weight
	  				u.predecessor <-- v
	              End If
	  			v.visited <-- true
	          End For
	      End While
	  End
	  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Dijkstra's algorithm - Wikipedia](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm)
	- Watch
		- {{video https://www.youtube.com/watch?v=_lHSawdgXpI&pp=ygUUZGlqa3N0cmEncyBhbGdvcml0aG0%3D}}
		- {{video https://www.youtube.com/watch?v=pSqmAO-m7Lk&pp=ygUUZGlqa3N0cmEncyBhbGdvcml0aG0%3D}}