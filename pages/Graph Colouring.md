tags:: Algorithmics
alias:: Graph Coloring
topic:: Problems
algo:: Unit 4 Outcome 2

-
- s a combinatorial optimization problem in graph theory that involves
	- *coloring of the vertices of a graph such that no two adjacent vertices have the same color*
- is both NP-complete and NP-hard
	- NP-complete as it is in NP (it can be verified in polynomial time)
	- NP-hard (at least as hard as any problem in NP).
- The problem is based on the concept of a chromatic number of a graph
	- the minimum number of colours needed to colour the vertices of the graph so that no two adjacent vertices have the same colour
- has many applications in real-world problems such as to schedule tasks, assign resources, and design communication networks
- [[Heuristic]] functions can be used to solve the graph colouring problem but are not guaranteed to find the optimal solution.
	- can often find a good solution in a reasonable amount of time
	- [[Backtracking]]
		- starts with a random colouring of the graph and then iteratively tries to improve it by changing the colour of one vertex at a time.
		- terminates when it cannot find a better colouring.
	- Local search
		- starts with a random colouring of the graph and then iteratively tries to find a neighbouring colouring that has a lower cost (reduced number of colours).
		- terminates when it cannot find a neighbouring colouring with a lower cost.
	- Genetic algorithms
		- uses a population of colourings and iteratively tries to improve the population by crossover and mutation.
		- terminates when it reaches a certain number of iterations or when it finds a colouring that is deemed to be good enough.
-
- Further Research
  background-color:: purple
	- Read
		- [Graph coloring - Wikipedia](https://en.wikipedia.org/wiki/Graph_coloring#Algorithms)
	- Watch
		- {{video https://www.youtube.com/watch?v=y4RAYQjKb5Y&pp=ygUOZ3JhcGggY29sb3Jpbmc%3D}}