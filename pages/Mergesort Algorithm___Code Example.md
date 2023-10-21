tags:: Algorithmics, Python, Code Example
alias:: Mergesort - Python
topic:: Mergesort
algo:: Unit 4 Outcome 2

- ```python
  # mergesort algorithm as a recursive function
  # and with a helper function to do the merge in linear time
  
  
  def mergesort(array):
      if len(array) <= 1:
          return array
      else:
          middle = len(array) // 2 # // is floor division
          left = mergesort(array[:middle])
          right = mergesort(array[middle:])
          return merge(left, right)
  
  
  def merge(left, right):
      result = []
      i = 0
      j = 0
      while i < len(left) and j < len(right):
          if left[i] <= right[j]:
              result.append(left[i])
              i += 1
          else:
              result.append(right[j])
              j += 1
      result += left[i:]
      result += right[j:]
      return result
  
  
  if __name__ == "__main__":
      array = [1, 5, 3, 6, 4, 2]
      print(mergesort(array))
  
  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Sorting algorithms/Merge sort - Rosetta Code](https://www.rosettacode.org/wiki/Sorting_algorithms/Merge_sort)