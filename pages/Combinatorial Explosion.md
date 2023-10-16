tags:: Algorithmics, Design Pattern
alias:: Curse of Dimensionality

- a disadvantage of using a [[Brute-Force]] approach for real-world problems is that the number of natural candidates (possible combinations) is prohibitively large.
- for instance, if we are seeking a particular rearrangement of 10 letters, then we have 10! = 3,628,800 candidates to consider, which a typical PC can generate and test in less than one second.
	- adding one more letter, only a 10% increase in the data size, will multiply the number of candidates by 11, a 1000% increase.
	- for 20 letters, the number of candidates is 20!, which is about 2.4×1018 or 2.4 quintillion and the search will take about 10 years.
-
- Further Research
  background-color:: purple
	- Read
		- [Brute-force search - Wikipedia](https://en.wikipedia.org/wiki/Brute-force_search#Combinatorial_explosion)
	- Watch
		- {{video https://www.youtube.com/watch?v=V_-gKrxMUcw&pp=ygUXY29tYmluYXRvcmlhbCBleHBsb3Npb24%3D}}