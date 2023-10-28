tags:: Algorithmics
topic:: [[Computer Science]]
algo:: Unit 4 Outcome 3

-
- Tractable problems are problems that can be solved in a reasonable amount of [time]([[Time Complexity]]) and [space]([[Space Complexity]])
- Tractable problems have a [[Time Complexity]] of one of
	- $O(1)$
	- $O(\log n)$
	- $O(n)$
	- $O(n \log n)$
	- $O(n^2)$
- Intractable problems are problems that cannot be solved in a reasonable amount of [time]([[Time Complexity]]) and [space]([[Space Complexity]])
- Intractable problems have a [[time complexity]] of one of
	- $O(2^n)$
	- $O(n!)$
	- $O(n^n)$
- a tractable problem example
	- finding the shortest path between two points in a grid graph is tractable
	- there is an algorithm, called [[Dijkstra's]] algorithm, that can solve the problem in polynomial time
- an intractable problem example
	- determining whether a given graph is 3-colorable is intractable
	- there is no algorithm that can solve the problem in polynomial time
- Intractable problems are important because they arise in many different areas of computer science
	- they are used in cryptography, scheduling, and artificial intelligence
- Intractable problems also have implications for the future of computing
	- if we cannot find efficient ways to solve intractable problems, then there are some problems that will never be solved by computers
- ((653c7158-e777-4d2d-9319-534352db9ea6))
- Tractability is different from the [[Decidability]]
-
-
- Further Research
  background-color:: purple
	- Read
		- [Intractability - Wikipedia](https://en.wikipedia.org/wiki/Computational_complexity_theory#Intractability)
		- https://theory.stanford.edu/~trevisan/cs170/notes/lecture21.pdf