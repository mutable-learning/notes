tags:: Algorithmics, Software Development, Python, Code Example
topic:: Python Implementations
algo:: Unit 4 Outcome 2

-
- an implementation of [[Binary Search]]
- ```python
  def binary_search(l, value):
  	"""Iterative version of Binary Search"""
      low = 0
      high = len(l)-1
      while low <= high: 
          mid = (low+high)//2
          if l[mid] > value: high = mid-1
          elif l[mid] < value: low = mid+1
          else: return mid
      return -1
  ```
- ```python
  def binary_search(l, value, low = 0, high = -1):
  	"""Recursive version of Binary Search"""
      if not l: return -1
      if(high == -1): high = len(l)-1
      if low >= high:
          if l[low] == value: return low
          else: return -1
      mid = (low+high)//2
      if l[mid] > value: return binary_search(l, value, low, mid-1)
      elif l[mid] < value: return binary_search(l, value, mid+1, high)
      else: return mid
  ```
-
- Further Research
  background-color:: purple
	- Read
		- [Binary search - Rosetta Code](https://www.rosettacode.org/wiki/Binary_search)