tags:: Algorithmics
topic:: [[Algorithm Analysis]]
algo:: Unit 4 Outcome 1

-
- ```
  Algorithm bubble_sort(arr):
    \\ indexes start from 0
    n \leftarrow length(arr) - 1
    For i \leftarrow 0 to n Do
        For j  \leftarrow 0 to n-i-1 Do
            If arr[j] > arr[j+1] Then
                arr[j], arr[j+1] \leftarrow arr[j+1], arr[j]
            End If
        End For
     End For   
  End
  ```
- Some techniques for determining time complexity of iterative algorithms:
	- Identify the basic operations. The first step is to identify the basic operations that the algorithm performs. These are the operations that take time to execute. For example, the basic operations in the algorithm bubble sort are comparing two elements and swapping two elements.
	- Count the number of times each operation is performed. Once you have identified the basic operations, you need to count the number of times each operation is performed. For example, the algorithm bubble sort compares each element in the array with the next element, so it performs n-1 comparisons.
	- Find the dominant term. The dominant term is the term that grows the fastest as the size of the input grows. For example, the dominant term in the time complexity of bubble sort is n^2, because the number of comparisons grows quadratically as the size of the input grows.
	- Use Big O notation to express the time complexity. Once you have identified the dominant term, you can use Big O notation to express the time complexity of the algorithm. For example, the time complexity of bubble sort is O(n^2).
- Here are some additional tips for determining time complexity of iterative algorithms:
	- Look for patterns. Often, you can find patterns in the way that an algorithm works that can help you to determine its time complexity. For example, many sorting algorithms work by comparing pairs of elements, so the number of comparisons is often the dominant term in their time complexity.
	- Use a calculator. If you are having trouble determining the dominant term, you can use a calculator to estimate the number of times each operation is performed. This can help you to identify the term that grows the fastest as the size of the input grows.