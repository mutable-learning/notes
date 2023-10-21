tags:: Algorithmics
topic:: Computer Science
algo:: Unit 4 Outcome 3

-
-
- Are There Problems That Computers Can't Solve? - YouTube
- Lambda Calculus - Computerphile - YouTube
- The halting problem is the problem of determining, from a description of an arbitrary computer program and an input, whether the program will finish running, or continue to run forever.
- This is undecidable because there is no general algorithm that can determine if a given program will halt or not for any possible input.
- The halting problem is a consequence of Gödel's incompleteness theorems where Gödel's theorems show that there are statements that are true but cannot be proven. The halting problem is one such statement.
	- It is true that there is no algorithm that can correctly determine, for any arbitrary program, whether the program will halt.
	- However, this statement cannot be proven.
- It was first posed by Alan Turing in his 1936 paper, "On Computable Numbers, with an Application to the Entscheidungsproblem".
- One way to prove this is by using a contradiction↓
	- Suppose there exists a Turing machine H that can solve the halting problem for any program P and input I.
	- Then we can construct another Turing machine D that uses H to decide the opposite of what H decides, i.e., if H says P halts on I, then D loops forever, and if H says P loops forever on I, then D halts.
	- Now, what happens if we feed D itself as both the program and the input? This leads to a paradox, because D cannot decide correctly what it will do.
	- Therefore, such a Turing machine H cannot exist, and the halting problem is undecidable. Does that make sense?
- The halting problem is significant because it has implications for the limits of what computers can do as it shows that there are some problems that are inherently impossible for computers to solve.
- This has led to the development of new theories of computation, such as complexity theory, which study the difficulty of different problems.
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- b