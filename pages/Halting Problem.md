tags:: Algorithmics
topic:: [[Computer Science]]
algo:: Unit 4 Outcome 3

-
- is the problem of determining, *"from a description of an arbitrary computer program and an input, will the program finish running or continue to run forever"*
- is [undecidable]([[Decidability]])
	- there is no general algorithm that can determine if a given program will halt or not for any possible input
- is a consequence of Gödel's incompleteness theorems which show that there are statements that are true but cannot be proven
	- the halting problem is one such statement
		- it is true that there is no algorithm that can correctly determine, for any arbitrary program, whether the program will halt
		- but this statement cannot be proven
- was first posed by Alan Turing in his 1936 paper, "On Computable Numbers, with an Application to the Entscheidungsproblem"
- One way to prove this is by using a [[Contradiction]]
	- suppose there exists a [[Turing Machine]] $H$ that can solve the halting problem for any program $P$ and input $I$
	- we can construct another [[Turing machine]] $D$ that uses $H$ to decide the opposite of what $H$ decides
		- if $H$ says $P$ halts on $I$, then $D$ loops forever
		- if $H$ says $P$ loops forever on $I$, then $D$ halts
	- what happens if we feed $D$ itself as both the program and the input?
		- this leads to a paradox, because $D$ cannot decide correctly what it will do
	- therefore, $H$ cannot exist, and the halting problem is [undecidable]([[Decidability]])
- is significant because it has implications for the limits of what computers can do
	- it shows that there are some problems that are inherently impossible for computers to solve
- has led to the development of new theories of computation, such as [complexity theory]([[Algorithm Analysis]]), which study the difficulty of different problems
-
- Further Research
  background-color:: purple
	- Read
		- [Halting problem - Wikipedia](https://en.wikipedia.org/wiki/Halting_problem)
		- [Halting Problem | Brilliant Math & Science Wiki](https://brilliant.org/wiki/halting-problem/)
	- Watch
		- {{video https://www.youtube.com/watch?v=t37GQgUPa6k&pp=ygUPaGFsdGluZyBwcm9ibGVt}}
		- {{video https://www.youtube.com/watch?v=sG0obNcgNJM&pp=ygUPaGFsdGluZyBwcm9ibGVt}}