tags:: Algorithmics, SoftDev
alias:: Binary Search
topic:: Advanced Algorithm Design
algo:: Unit 4 Outcome 2

-
- is a decrease and conquer [[Recursion]] algorithm that works on sorted arrays.
- is a very efficient algorithm for searching ***sorted*** arrays.
	- In terms of iterations, no search algorithm that works only by comparing elements can exhibit better average and worst-case performance than binary search.
- works by
	- comparing an element in the middle of the array with the target value.
	- if the target value matches the element, its position in the array is returned.
	- if the target value is less than the element, the search continues in the lower half of the array.
	- if the target value is greater than the element, the search continues in the upper half of the array.
	- *the algorithm eliminates the half in which the target value cannot lie in each iteration.*
- key aspects of the binary search
	- ***the input array must be sorted***
	- the algorithm compares the target value to the *middle* element of the array.
	- if the target value is equal to the middle element, the algorithm returns the *index* of the middle element.
	- if the target value is less than the middle element, the algorithm searches the lower half of the array.
	- if the target value is greater than the middle element, the algorithm searches the upper half of the array.
	- the algorithm continues searching until the target value is found or the entire array has been searched.
- Binary search has a worst-case time complexity of $O(log n)$, where n is the number of elements in the array.
	- the algorithm will always terminate in a logarithmic number of steps, regardless of the size of the array.
- Time complexities for Binary Search are
	- $\Omega(1)$
	- $\Theta(\log n)$
	- $O(\log n)$
- Use the Master Theorem to verify the time complexity
- Pseudocode
	- ```
	  
	  BinarySearch(array, value)
	  	// Iterative version of Binary Search algorithm
	  	low <-- 0
	      high <-- Length(array) - 1
	      While low <= high Do
	          mid <-- low + high / 2
	          If (array[mid] > value) Then
	              high <-- mid - 1
	          Else If array[mid] < value Then
	              low <-- mid + 1
	          Else
	              Return mid
	          End If
	      End While
	      Return "not found" // value would be inserted at index "low"
	  End
	  ```
-
-
- Further Research
  background-color:: purple
	- Read
		- [Binary search algorithm - Wikipedia](https://en.wikipedia.org/wiki/Binary_search_algorithm)
	- Watch
		- {{video https://www.youtube.com/watch?v=MFhxShGxHWc&pp=ygUNYmluYXJ5IHNlYXJjaA%3D%3D}}
		- {{video https://www.youtube.com/watch?v=KXJSjte_OAI&pp=ygUNYmluYXJ5IHNlYXJjaA%3D%3D}}