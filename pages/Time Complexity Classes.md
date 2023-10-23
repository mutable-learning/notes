tags:: Algorithmics
topic:: [[Algorithm Analysis]]
algo:: Unit 4 Outcome 1

-
- Polynomial time
	- is a measure of how long an algorithm takes to run, as a function of the size of the input data.
	- an algorithm is said to be polynomial-time if its running time is upper bounded by a polynomial expression in the size of the input for the algorithm
		- $T(n) = O(n^k)$ for some positive constant $k$
	- are considered to be efficient, because they can solve problems that grow large in size in a reasonable amount of time.
- P problems
	- can be solved in polynomial time
	- the time it takes to solve the problem grows as a polynomial function of the size of the input data
	- are considered to be "easy" to solve.
	- a problem belongs to class P if it’s easy to find a solution for the problem and can be solved and verified in polynomial time
- NP problems
	- can be verified in polynomial time
	- given a solution to the problem, it can be checked in polynomial time to see if the solution is correct
	- considered to be "hard" to solve, because even though they can be verified quickly, they can be very time-consuming to find a solution for
	- are problems that can be solved by guessing the solution and then verifying it in polynomial time
- NP-hard problems
	- are at least as hard as any NP problem
	- if there is an algorithm that can solve an NP-hard problem in polynomial time, then there would also be an algorithm that can solve any NP problem in polynomial time
	- are considered to be the "hardest" problems to solve
- NP-complete problems
	- are both NP-hard and NP
	- they are at least as hard as any NP problem, and they can also be verified in polynomial time
	- a problem for which any proposed solution can be quickly verified to be correct, but for which finding a solution in the first place is difficult
- ![Time Complexity Classes](https://3.bp.blogspot.com/-XJw7zqa5GTE/T47c0ZmnyJI/AAAAAAAAA5k/JWEc7gNLkkw/s1600/compcomplex.JPG)
-
- Further Research
  background-color:: purple
	- Read
		- [Time complexity - Wikipedia](https://en.wikipedia.org/wiki/Time_complexity)
	- Watch
		- {{video https://www.youtube.com/watch?v=n0zd5hcOSQI&pp=ygUgbnAtaGFyZCBhbmQgbnAtY29tcGxldGUgcHJvYmxlbXM%3D}}
		- {{video https://www.youtube.com/watch?v=YX40hbAHx3s&pp=ygUWbnAgbnAtaGFyZCBucC1jb21wbGV0ZQ%3D%3D}}
		- {{video https://www.youtube.com/watch?v=W9G_1xG77LE&pp=ygUgbnAtaGFyZCBhbmQgbnAtY29tcGxldGUgcHJvYmxlbXM%3D}}