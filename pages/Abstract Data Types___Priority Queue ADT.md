tags:: Algorithmics

- Priority Queue
  background-color:: yellow
	- allow for adding elements with a priority
	- will return the element with the *highest* priority first (priority order)
	- priority values can be either min or max to determine the *highest*
	- must have items that are comparable to determine which one has a higher priority
- Priority Queue Definition
  background-color:: red
	- **Name:** $Priority Queue$
	  **Import:** $element, boolean, integer$
	   
	  Operations:
	  $create: \space\to pqueue$
	  $empty: pqueue \to boolean$
	  $insertWithPriority: pqueue$ x $element$ x $integer \to pqueue$
	  $getMinElement: pqueue \to pqueue$
	  $findMin: pqueue \to element$