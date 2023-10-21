tags:: Algorithmics
alias:: Mergesort
topic:: Advanced Algorithm Design
algo:: Unit 4 Outcome 2

-
- uses divide and conquer [[Recursion]] for sorting arrays.
- works by recursively dividing the array into two halves, sorting each half, and then merging the two sorted halves back together.
- key aspects of the mergesort algorithm are:
	- Divide: The array is divided into two halves.
	- Conquer: The two halves are sorted recursively.
	- Combine: The two sorted halves are merged back together.
- \very efficient algorithm for sorting arrays.
	- Its time complexity is $O(n \log n)$, where n is the number of elements in the array.
	- time complexity grows logarithmically with the size of the problem.
- the merge function takes two sorted arrays as input and merges them back together into a single sorted array.
	- works by iterating through the two arrays and adding the smaller element from each array to the result array.
	- continues iterating until both arrays have been exhausted or, if one of the arrays is empty, the remaining items in the other array will be added to the end of the result in one operation.
	- the merge function has a linear time complexity
- The time complexity for merge sort is
	- best case: $O(n \log n)$
	- average case: $O(n \log n)$
	- worst case: $O(n \log n)$
-
- Further Research
  background-color:: purple
	- Read
		- [Merge sort - Wikipedia](https://en.wikipedia.org/wiki/Merge_sort)
	- Watch
		- {{video https://www.youtube.com/watch?v=4VqmGXwpLqc&pp=ygUJbWVyZ2Vzb3J0}}
		- {{video https://www.youtube.com/watch?v=3j0SWDX4AtU&pp=ygUJbWVyZ2Vzb3J0}}