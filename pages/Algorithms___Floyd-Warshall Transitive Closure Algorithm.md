tags:: Algorithmics
alias:: Transitive Closure

-
- when we want to know if a path exists between any two nodes
- use Boolean relations to represent paths between nodes
- a connected, undirected graph always has a path between any two nodes
- a connected, directed graph may not have paths between any two nodes
- to work out the transitive closure for all pairs of nodes we can determine if there is a path from A to B, and a path from B to C, then there is also a path from A to C
- this transitive closure algorithm builds a matrix of |V| x |V| size to determine if paths exist between nodes in a directed, connected graph
- ```
  Algorithm FWTransitiveClosure(G)
  	// Create a matrix of |V|x|V| size to store the reachability info
  	T <-- empty Boolean matrix of size |V|x|V|
  	For i <-- 1 to |V| Do 
  		For j <-- 1 to |V| Do
  			If ((i = j) OR (edge(i,j) exists) Then
  				T[i,j] <-- 1 // path exists
  			Else
  				T[i,j] <-- 0 // unsure if path exists
              End If
          End For
      End For
  	
  	// Complete the matrix of reachabilities in T
  	For k <-- 1 to |V| Do
  		For i <-- 1 to |V| Do
  			For j <-- 1 to |V| Do
  				// Boolean test: can you go from i via k to j
  				T[i,j] <-- T[i,j] OR (T[i,k] AND T[k,j])
              End For
          End For
  	End For     
      Return T
  End
  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Transitive closure - Wikipedia](https://en.wikipedia.org/wiki/Transitive_closure#In_graph_theory)
		- [Floyd–Warshall algorithm - Wikipedia](https://en.wikipedia.org/wiki/Floyd%E2%80%93Warshall_algorithm)