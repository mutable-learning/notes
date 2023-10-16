tags:: Algorithmics
alias:: Queue

-
- Queue
  background-color:: yellow
	- allow for adding at one end and removing of elements at the other end
	- follow the first in first out rule (FIFO)
	- will have the **front** of the queue containing the oldest element
	- will maintain the order of elements in the order they were added to the queue
- Queue Definition
  background-color:: red
	- **Name:** $Queue$
	  **Import:** $element, boolean$
	   
	  Operations:
	  $create: \space\to queue$
	  $empty: queue \to boolean$
	  $enqueue: queue$ x $element \to queue$
	  $dequeue: queue \to queue$
	  $peek: queue \to element$