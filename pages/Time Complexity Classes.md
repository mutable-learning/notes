tags:: Algorithmics
topic:: [[Algorithm Analysis]]
algo:: Unit 4 Outcome 1

-
- Polynomial time↓
	- is a measure of how long an algorithm takes to run, as a function of the size of the input data. An algorithm is said to be polynomial-time if its running time is upper bounded by a polynomial expression in the size of the input for the algorithm, that is, T(n) = O(nk) for some positive constant k.
	- Polynomial-time algorithms are considered to be efficient, because they can solve problems that grow large in size in a reasonable amount of time.
- P problems
	- Problems that can be solved in polynomial time. This means that the time it takes to solve the problem grows as a polynomial function of the size of the input data. Polynomial time problems are considered to be "easy" to solve.
	- A problem belongs to class P if it’s easy to find a solution for the problem and can be solved and verified in polynomial time
- NP problems↓
	- Problems that can be verified in polynomial time. This means that given a solution to the problem, it can be checked in polynomial time to see if the solution is correct. NP problems are considered to be "hard" to solve, because even though they can be verified quickly, they can be very time-consuming to find a solution for.
	- In simple terms, NP problems are problems that can be solved by guessing the solution and then verifying it in polynomial time.
- NP-hard problems↓
	- Problems that are at least as hard as any NP problem. This means that if there is an algorithm that can solve an NP-hard problem in polynomial time, then there would also be an algorithm that can solve any NP problem in polynomial time. NP-hard problems are considered to be the "hardest" problems to solve.
- NP-complete problems
	- Problems are both NP-hard and NP. This means that they are at least as hard as any NP problem, and they can also be verified in polynomial time .
	- In simple terms, a problem for which any proposed solution can be quickly verified to be correct, but for which finding a solution in the first place is difficult.
- ![Time Complexity Classes](https://3.bp.blogspot.com/-XJw7zqa5GTE/T47c0ZmnyJI/AAAAAAAAA5k/JWEc7gNLkkw/s1600/compcomplex.JPG)
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- b