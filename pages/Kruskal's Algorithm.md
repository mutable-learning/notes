tags:: Algorithmics
alias:: Kruskal's
topic:: MST
algo:: Unit 3 Outcome 2

-
- Used to find the [[MST]] for a weighted, connected graph
- Requires the edges to be sorted by weight so using a minimum priority queue works well
- Uses a [[Greedy]] [[Design Pattern]] to find a solution
- When the set of nodes in the new tree is equal to the set of graph nodes the MST is complete
- Steps for the algorithm are
	- Sort all the edges from low weight to high.
	- Take the edge with the lowest weight and add it to the spanning tree. If adding the edge created a cycle, then reject this edge.
	- Keep adding edges until we reach all vertices.
- Pseudocode for the algorithm is
	- ```
	  Algorithm kruskal(graph)
	      MST <-- new graph
	      Sort edges in graph
	      While edge not checked Do
	          Select next unchecked edge
	          If (not creating a cycle) Then
	              Add edge to MST
	          End If
	          Mark edge as checked
	      End While
	      Return MST
	  End
	  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Kruskal's algorithm - Wikipedia](https://en.wikipedia.org/wiki/Kruskal%27s_algorithm)
	- Watch
		- {{video https://www.youtube.com/watch?v=71UQH7Pr9kU&pp=ygUTa3J1c2thbCdzIGFsZ29yaXRobQ%3D%3D}}
		- {{video https://www.youtube.com/watch?v=JZBQLXgSGfs&pp=ygUTa3J1c2thbCdzIGFsZ29yaXRobQ%3D%3D}}
		-