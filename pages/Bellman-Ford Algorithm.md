tags:: Algorithmics
alias:: Bellman-Ford
topic:: Graph Traversal
algo:: Unit 3 Outcome 2

- uses a [[Brute-Force]] approach to check all edges for a vertex and build a solution incrementally
- uses a nested loop process to loop through all the edges (|V|-1) times and update the distances repeatedly
- slower than [[Dijkstra's Algorithm]] but can be used to find graphs with negative cycles, which can be useful
	- it can return a notification if a negative weighted cycle exists in a graph
	- no shortest path can be produced if there is a negative cycle
- Pseudocode
	- ```
	  Algorithm BellmanFord(G, s)
	  	// Input G is a graph
	  	// Input s is the starting vertex
	  	// Output is the graph with each vertex having attributes
	  	// of distance and predecessor
	  	
	  	For each vertex in G Do
	  		vertex.distance <-- ∞
	  		vertex.predecessor <-- undefined
	      End For
	  	
	  	s.distance <-- 0 // the starting node will be the first one chosen below
	  	
	  	For i <-- 1 to (|V| - 1) Do
	  		For each edge (u-v) with weight of w in G.edges Do
	  			If (u.distance + w) < v.distance Then
	  				v.distance <-- u.distance + w
	  				v.predecessor <-- u
	              End If
	          End For
	      End For
	      
	      // Now make sure there are no negative cycles
	      // If one is found return a notification instead of a graph
	  	For each edge (u-v) with weight w in G.edges Do
	  		If v.distance > (u.distance + w) Then
	  			Return "Graph contains a negative cycle"
	          End If
	      End For
	      
	  	Return G // If no negative cycles found
	  End
	  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Bellman–Ford algorithm - Wikipedia](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm)
	- Watch
		- {{video https://www.youtube.com/watch?v=obWXjtg0L64&pp=ygUWYmVsbG1hbi1mb3JkIGFsZ29yaXRobQ%3D%3D}}
		- {{video https://www.youtube.com/watch?v=lyw4FaxrwHg&pp=ygUWYmVsbG1hbi1mb3JkIGFsZ29yaXRobQ%3D%3D}}