tags:: Algorithmics
topic:: [[Algorithm Analysis]]
algo:: Unit 4 Outcome 1

-
- is a measure of how long it takes an algorithm to run as a function of the size of the input
- Big O, Big \Theta, and Big \Omega are three notations used in computer science to describe the asymptotic behaviour of algorithms.
	- used to classify algorithms based on their time complexity
- Big O notation is used to describe the upper bound of an algorithm's time complexity
	- the running time of the algorithm will never be more than the expression in Big \O notation
	- for example, the algorithm bubble sort has a time complexity of $O(n^2)$
		- the running time of bubble sort will never be more than $n^2$
		- the function grows no faster than $n^2$
- Big \Theta notation is used to describe both the upper bound and the lower bound of an algorithm's time complexity
	- the running time of the algorithm will always be between the expressions in Big \Theta notation
	- for example, the algorithm [[Binary Search]] has a time complexity of $\Theta(log\ n)$
		- the running time of binary search will always be between $\log n$ and $2\ log\ n$
		- the function grows as fast as $\log n$
- Big \Omega notation is used to describe the lower bound of an algorithm's time complexity
	- the running time of the algorithm will never be less than the expression in Big Omega notation
	- for example, the algorithm [[Mergesort]] has a time complexity of $\Omega(n log\ n)$
		- the running time of merge sort will never be less than $n \log n$
		- the function grows no slower than $n \log n$
- Here are some examples of how $Big\ O,\ Big\ \Theta\ and\ Big\ \Omega$ are used:
	- bubble sort has a time complexity of $O(n^2)$
		- the running time of bubble sort will never be more than $n^2$
	- [[Binary Search]] has a time complexity of $\Theta(log\ n)$
		- the running time of binary search will always be between $\log n$ and $2 \log n$
	- [[Mergesort]] has a time complexity of $\Omega(n\ log\ n)$
		- the running time of merge sort will never be less than $n \log n$
	- Big $O$
		- worst-case time complexity
		- describes the upper bound
	- Big $\Theta$
		- average-case time complexity
		- describes both the lower bound and upper bound
	- Big $\Omega$
		- best-case time complexity
		- describes the lower bound
-
- Further Research
  background-color:: purple
	- Read
		- a
	- Watch
		- {{video https://www.youtube.com/watch?v=g2o22C3CRfU&pp=ygUWYW5hbHlzaXMgb2YgYWxnb3JpdGhtcw%3D%3D}}
		- {{video https://www.youtube.com/watch?v=__vX2sjlpXU&pp=ygUWYW5hbHlzaXMgb2YgYWxnb3JpdGhtcw%3D%3D}}
		- {{video https://www.youtube.com/watch?v=0oDAlMwTrLo&pp=ygUTYXN5bXB0b3RpYyBhbmFseXNpcw%3D%3D}}