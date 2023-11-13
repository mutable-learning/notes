tags:: Algorithmics, Software Development
alias:: Quicksort
topic:: [[Advanced Algorithm Design]]
algo:: Unit 4 Outcome 2

-
- uses [[Divide and Conquer]] [[Recursion]] for sorting arrays.
- works by recursively partitioning the array around a Pivot element.
- the Pivot element is then placed in its correct position in the array, and the two halves of the array are recursively sorted.
- key aspects of the quicksort:
	- **Pivot selection**: The Pivot element is selected randomly or using a deterministic [[Heuristic]] .
	- **Partitioning**: The array is partitioned around the pivot element, such that all elements smaller than the pivot element are placed before the pivot element, and all elements larger than the pivot element are placed after the pivot element.
	- Recursive sorting: The two halves of the array are recursively sorted.
- is a very efficient algorithm for sorting arrays.
	- Its time complexity is $O(n \log n)$ on average and $O(n^2)$ in the worst case, where $n$ is the number of elements in the array.
	- the time complexity grows logarithmically with the size of the problem in the average case, *but it can grow quadratically in the worst case*.
- the partition function in quicksort can run in linear time, but it does not always run in linear time.
	- the partition function works by comparing each element in the array to the Pivot.
	- if the element is smaller than the pivot, then it is placed in the left subarray.
	- if the element is larger than the Pivot, then it is placed in the right subarray.
- the partition function can run in linear time if the Pivot is chosen carefully.
	- if the Pivot is chosen randomly, then the partition function is likely to run in linear time.
	- if the Pivot is chosen poorly, then the partition function can run in quadratic time.
- the worst-case time complexity for the partition function occurs when the Pivot is the smallest or largest element in the array.
	- all of the elements smaller than the Pivot will be placed in the left subarray, and all of the elements larger than the Pivot will be placed in the right subarray.
	- this results in two subproblems with very different sizes, which can lead to a quadratic running time for the partition function.
- the best-case time complexity for the partition function occurs when the Pivot is the median of the array.
	- the median of the array will divide the array into two subproblems with equal sizes.
	- this results in a linear running time for the partition function.
- the best way to ensure that the partition function runs in linear time is to choose the Pivot randomly.
- The time complexity for quick sort is
	- best case:  $O(n \log n)$
	- average case: $O(n \log n)$
	- worst case: $\Theta(n^2)$
- ```
  Algorithm Quicksort(array, low, high):
  	If low < high Then
  		pivot <-- Partition(array, low, high)
      	Quicksort(array, low, pivot - 1)
      	Quicksort(array, pivot + 1, high)
     	End If
  End
  
  Algorithm Partition(array, low, high)
  	pivot = array[high]
  	i = low - 1
  	For j <-- low to high Do
  		If array[j] <= pivot Then
  			i <-- i + 1
  			Swap(array[i], array[j])
  		End If
      End For
  	Swap(array[i + 1], array[high])
  	Return i + 1
  
  	Function Swap(x, y)
      	temp <-- x
      	x <-- y
      	y <-- temp
      End Function
  End
  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Quicksort - Wikipedia](https://en.wikipedia.org/wiki/Quicksort)
	- Watch
		- {{video https://www.youtube.com/watch?v=Hoixgm4-P4M&pp=ygUJbWVyZ2Vzb3J0}}
		- {{video https://www.youtube.com/watch?v=Vtckgz38QHs&pp=ygUJcXVpY2tzb3J0}}