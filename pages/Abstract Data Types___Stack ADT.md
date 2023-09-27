tags:: Algorithmics

- Stack
  background-color:: yellow
	- allow for adding and removing of elements to one end only
	- will have the most recently added item also being the one removed first (LIFO)
	- will have the **top** of the stack containing the most recently added item
	- will maintain the order of elements in the order they were added to the stack
	- will have a limited capacity
- Stack Definition
  background-color:: red
	- **Name:** $Stack$
	  **Import:** $element, boolean$
	   
	  Operations:
	  $newStack:    \space\to stack$
	  $empty:  stack \to boolean$
	  $push:   stack$ x $element \to stack$
	  $pop:    stack \to stack$
	  $top:    stack \to element$