tags:: Algorithmics
alias:: PageRank
topic:: Graph Traversal
algo:: Unit 3 Outcome 2

-
- gives each page a rating of its importance
- uses [[Recursion]] to define a measure whereby a page becomes important if important pages link to it
	- is recursive because the importance of a page refers back to the importance of other pages that link to it
- imagine a random surfer on the web, following links from page to page
	- the page rank of any page is roughly the probability that the random surfer will land on a particular page
	- since more links go to the important pages, the surfer is more likely to end up there
- is an example of a Markov process
	- any random evolutionary process that depends only of the current state of a system and not on its history
- the page rank process follows these steps
	- start with a set of nodes in a directed [[Graph]]
	- determine the links (edges) out and in for all nodes
	- assign each page an initial rank of $1/N$
	- successively update the rank of each node
		- adding up the weight of every node that links to it divided by the number of links coming from the referring page
		- $PR(A) = \frac {PR(B)} 2 + \frac {PR(C)} 1 + \frac {PR(D)} 3$
			- or if we use L() to represent the number of outbound edges (links) for a node
			- $PR(A) = \frac {PR(B)} {L(B)} + \frac {PR(C)} {L(C)} + \frac {PR(D)} {L(D)}$
	- if a node has no outward links, redistribute its rank equally among the other nodes in the graph
	- apply this redistribution to every node in the graph
	- repeat this process until the page ranks stabilize
	- a damping factor is added at each stage to model the idea that users stop searching
- PageRank pseudocode
	- ```
	  Algorithm PageRank(G)
	  	// Input is a directed graph
	  	N <-- |V| // the number of nodes
	  	D <-- 0.85 // damping factor 
	  	
	  	For each node of G Do
	  		node.PageRank <-- 1/N
	      End For
	  	
	  	// Distribute the probability for nodes that have no out edges (sink nodes)
	  	For each node of G Do
	  		If count of node outgoing edges = 0 Then
	  			For each node2 in G Do
	  				Add edge node to node2
	              End For
	          End If
	      End For
	  	
	  	Repeat
	  		For each node of G Do
	  			total <-- 0
	  			For each incoming edge of node Do
	  				from_node <-- from node on incoming edge to node
	  				total <-- from_node.PageRank / (count of from_node outgoing edges)
	              End For
	  			node.PageRank <-- (1-D)/N + (D*total)
	          End For
	  	Until PageRank values converge
	  End
	  ```
-
- Further Research
  background-color:: purple
	- Read
		- [PageRank - Wikipedia](https://en.wikipedia.org/wiki/PageRank)
	- Watch
		- {{video https://www.youtube.com/watch?v=qxEkY8OScYY&pp=ygUIcGFnZXJhbms%3D}}
		- {{video https://www.youtube.com/watch?v=v7n7wZhHJj8&pp=ygUIcGFnZXJhbms%3D}}