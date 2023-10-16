tags:: Algorithmics, Algorithm, Design Pattern

-
- refers to algorithms that are self-referencing
- the algorithm calls itself one or more times
- many iterative algorithms can be implemented as recursive algorithms
- **Base case** is the condition that stops the recursion from continuing endlessly
	- **Terminating condition** is another name for a base case
- once the base case is reached and the simplest version of the problem is solved, all previous versions can be assembled by passing the values back up the stack to the initial call of the algorithm, and the full solution is reached
- *useful when a problem can be broken up into smaller and smaller pieces all of the same problem*
- **Decrease and conquer** algorithms reduce the size of the input data at each step of the solution process. The technique is used when it's easier to solve a smaller version of the problem, and the solution to the smaller problem can be used to find the solution to the original problem.
	- One subproblem is generated each recursion with the input reduced each time
	- [[Binary Search]] is an example of a decrease and conquer recursive algorithm
- **Divide and conquer** algorithms divide the input data into smaller subproblems at each step of the solution process. The technique is used when the problem can be naturally divided into smaller subproblems that are independent of each other.
	- Two or more subproblems are generated each recursion
	- Input size reflects the number of divisions
	- [[Mergesort]] is an example of a divide and conquer algorithm
-
- Further Research
  background-color:: purple
	- Read
		- [Divide-and-conquer algorithm - Wikipedia](https://en.wikipedia.org/wiki/Divide-and-conquer_algorithm)
		- [Decrease and Conquer - GeeksforGeeks](https://www.geeksforgeeks.org/decrease-and-conquer/)
	- Watch
		- {{video https://www.youtube.com/watch?v=rf60MejMz3E&pp=ygUUcmVjdXJzaXZlIGFsZ29yaXRobXM%3D}}
		- {{video https://www.youtube.com/watch?v=KEEKn7Me-ms&pp=ygUUcmVjdXJzaXZlIGFsZ29yaXRobXM%3D}}
		-