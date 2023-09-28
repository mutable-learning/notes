alias:: Graph
tags:: Algorithmics

- Graph
  background-color:: yellow
	- are made up of vertices (nodes, points) that represent entities on the graph
	- can have edges (lines, links, arcs or branches) that connect two vertices to show a relationship or connection
	- can store data with each vertex such as a number, a label or another object
	- can store data with each edge such as a direction, a weight or distance
	- can be traversed using the edges to create paths through the graph
	- can be represented as an adjacency list, where each vertex stores a list of the vertices it is connected to
	- can be represented as an adjacency matrix, where each element of the matrix indicates whether the two vertices are connected with an edge
	- [[Graph Properties]] contains all the properties that are used to describe a graph
- Graph Definition
  background-color:: red
	- **Name:** $Graph$
	  **Import:** $element, boolean$
	   
	  Operations:
	  $create: \space\to graph$
	  $add\_vertex: graph$ x $element \to graph$
	  $remove\_vertex: graph$ x $element \to graph$
	  $add\_edge: graph$ x $element$ x $element \to graph$
	  $remove\_edge: graph$ x $element$ x $element \to graph$
	  $adjacent: graph$ x $element \to boolean$
	  $neighbours: graph$ x $element \to element$
	  $set\_edge\_value: graph$ x $element$ x $element$ x $element \to graph$
	  $get\_edge\_value: graph$ x $element$ x $element \to element$