tags:: Algorithmics, SoftDev, Python, Code Example
alias:: Quicksort - Python
topic:: Quicksort
algo:: Unit 4 Outcome 2

-
- ```python
  # A recursive function to sort an array using the quicksort algorithm
  # and includes a helper function to do the merge steps in linear time
  
  
  def quicksort(array, low, high):
      if len(array) == 1:
          return array
      if low < high:
          pivot = partition(array, low, high)
          quicksort(array, low, pivot - 1)
          quicksort(array, pivot + 1, high)
      return array
  
  
  def partition(array, low, high):
      pivot = array[high]
      i = low - 1
      for j in range(low, high):
          if array[j] <= pivot:
              i += 1
              array[i], array[j] = array[j], array[i]
      array[i + 1], array[high] = array[high], array[i + 1]
      return i + 1
  
  
  if __name__ == "__main__":
      # array = [1, 5, 3, 2, 4, 6]
      array = [1, 2, 3, 4, 5, 6]
      low = 0
      high = len(array) - 1
      print(quicksort(array, low, high))
  
  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Sorting algorithms/Quicksort - Rosetta Code](https://www.rosettacode.org/wiki/Sorting_algorithms/Quicksort)