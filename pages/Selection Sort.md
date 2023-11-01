tags:: Software Development
topic:: Sorting Algorithms
softdev:: Unit 3 Outcome 1

-
- a simple and relatively inefficient sorting algorithm
- input elements are searched repeatedly and the smallest element is moved to the front each time
	- any smaller element is swapped with the initial element each iteration
	- the initial element index increments by one each time the swapping operation reaches the end of the input elements
	- the process repeats until the initial element index is the last element
- ```
  Algorithm SelectionSort(input)
  	// input is a collection of unsorted elements such as an array or list
      
      Function Swap(x, y)
      	temp <-- x
          x <-- y
          y <-- temp
      End Function
      
      n <-- Length(input)
      For i <-- 0 to (n - 1) Do
      	small <-- i
          For j <-- (i + 1) to (n - 1) Do
          	If input[i] > input[j] Then
              	small <-- j
              End If
          End For
          Swap(input[i], input[small])
      End For
      Return input
  End
              
  ```