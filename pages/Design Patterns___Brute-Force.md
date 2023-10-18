tags:: Algorithmics
alias:: Exhaustive Search, Generate and Test, Brute-Force

-
- a very general [[Design Pattern]] that systematically checks all possible candidates to find a solution
- guaranteed to find a solution if it exists
- may not be feasible due to the number of possible combinations tends to grow very quickly as the size of the problem (size of input) increases, known as [[Combinatorial Explosion]]
- typically used when the problem size is limited and the best solution must be found
- use a [[Heuristic]] to speed up [[Brute-Force]] search and reduce the number of possible candidates
	- for example in the 8-queens problem a queen can be placed on any of the 64 squares ($64^8$ possibilities)
	- however, as no queens can be placed on the same square we are actually choosing a set of 8 squares from a set of 64 (64 choose 8), which is $64!/(56!\times 8!)$
	- also, no two queens can be on the same row or column, further reducing the number of possible candidates
-
-
- Further Research
  background-color:: purple
	- Read
		- [Brute-force search - Wikipedia](https://en.wikipedia.org/wiki/Brute-force_search)
	- Watch
		- {{video https://www.youtube.com/watch?v=hrMgfwi75zY&pp=ygUSYnJ1dGUtZm9yY2Ugc2VhcmNo}}