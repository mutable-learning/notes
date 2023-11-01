tags:: Software Development
topic:: Search Algorithms
softdev:: Unit 3 Outcome 1

-
- the simplest type of search
- checks every element of the input for a match in order until a match is found of the end of the input is reached
- usually completed using [[Iteration]] with a For loop style of [[Processing Feature/Iteration]]
- inefficient as the size of the input grows
	- can be useful when input sizes are known to be small
- unlike [[Binary Search]], the input is not required to be sorted first before searching
- ```
  Algorithm LinearSearch(input, item)
  	// input is an ordered collection of elements such as a list or array
      // item is the data we wish to find in the input
      // returns the index number of the item if found or -1 if not found
      
      found <-- -1
      For i in Length(input) - 1 Do
      	If input[i] = item Then
          	found <-- i
              Break
          End If
      End For
      Return found
  End
  ```