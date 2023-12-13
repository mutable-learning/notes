tags:: Algorithmics
topic:: [[Algorithm Analysis]]
algo:: Unit 4 Outcome 1

-
- ```
  Algorithm bubble_sort(arr):
    // indexes start from 0
    n <-- length(arr) - 1
    For i <-- 0 to n Do
        For j  <-- 0 to n-i-1 Do
            If arr[j] > arr[j+1] Then
                arr[j], arr[j+1] <-- arr[j+1], arr[j]
            End If
        End For
     End For   
  End
  ```
- Some techniques for determining time complexity of iterative algorithms:
	- identify the basic operations
		- the operations that take time to execute
		- for example, the basic operations in the algorithm bubble sort are
			- comparing two elements
			- swapping two elements.
	- Count the number of times each operation is performed
		- for example, the algorithm bubble sort compares each element in the array with the next element
		- it performs n-1 comparisons
	- Find the dominant term
		- Dominant Term
			- is the term that grows the fastest as the size of the input grows
		- for example, the dominant term in the [[Time Complexity]] of bubble sort is $n^2$
			- the number of comparisons grows quadratically as the size of the input grows
	- Use Big $O$ notation to express the [[Time Complexity]]
		- use Big $O$ notation to express the time complexity of the algorithm
		- for example, the time complexity of bubble sort is $O(n^2)$
- Here are some additional tips for determining time complexity of iterative algorithms:
	- look for patterns
		- often, you can find patterns in the way that an algorithm works that can help you to determine its time complexity
		- for example, many sorting algorithms work by comparing pairs of elements, so the number of comparisons is often the dominant term in their time complexity
	- use a calculator
		- if you are having trouble determining the dominant term, you can use a calculator to estimate the number of times each operation is performed
		- this can help you to identify the term that grows the fastest as the size of the input grows
-
- Further Research
  background-color:: purple
	- Read
		- [How to Analyse Loops for Complexity Analysis of Algorithms - GeeksforGeeks](https://www.geeksforgeeks.org/how-to-analyse-loops-for-complexity-analysis-of-algorithms/)
		- [SI335: Analyzing simple iterative algorithms](https://www.usna.edu/Users/cs/wcbrown/courses/S18SI335/lec/l03/lec.html)
	- Watch
		- {{video https://www.youtube.com/watch?v=TshlVlvU1TY&pp=ygUUaXRlcmF0aXZlIGFsZ29yaXRobXM%3D}}