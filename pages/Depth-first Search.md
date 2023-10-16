tags:: Algorithmics, Algorithm

- Traversing a tree or graph
- Start at any node, or the root node (in a tree)
- Explore as far along a branch as possible until a leaf node is encountered
- Backtrack up the branch to the previous branch on the path
- Only difference with [[Breadth-first Search]] is using a [[Stack]] instead of a [[Queue]]]
- Steps to follow
	- Start from root node (random for graph)
	- Set node as seen
	- Check each neighbour node
	- If it hasn't been seen, add it to the stack
	- Add node to list of nodes visited
	- Pop next node off the stack and repeat from step 2
- Psuedocode
	- ```
	  Algorithm DFS_recursive(G, v)
	      Label v as discovered
	      For all directed edges from v to w that are in G.adjacentEdges(v) Do
	          If vertex w is not labeled as discovered Then
	              Call DFS_recursive(G, w)
	          End If
	      End For
	  End
	  ```
	- ```
	  Algorithm DFS_iterative(G, v)
	      Let S be a stack
	      S.push(v)
	      While S is not empty Do
	          v ← S.pop()
	          If v is not labeled as discovered Then
	              Label v as discovered
	              For all edges from v to w in G.adjacentEdges(v) Do 
	                  S.push(w)
	              End For
	          End If
	      End While
	  End
	  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Depth-first search - Wikipedia](https://en.wikipedia.org/wiki/Depth-first_search)
	- Watch
		- {{video https://www.youtube.com/watch?v=Urx87-NMm6c&pp=ygUSZGVwdGgtZmlyc3Qgc2VhcmNo}}