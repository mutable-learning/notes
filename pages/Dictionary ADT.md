tags:: Algorithmics
alias:: Associative Array, Dictionary
topic:: Abstract Data Types
algo:: Unit 3 Outcome 1

-
- Dictionary:
  background-color:: yellow
	- have a key and a value associated with the key
	- keys are unique
	- values are not unique
	- keys and values can be of any type
	- the ordering of data is not maintained
- Dictionary Definition
  background-color:: red
	- **Name:** $Dictionary$
	  **Import:** $element, boolean, integer, iterator$
	   
	  Operations:
	  $create: \space\to dictionary$
	  $empty: dictionary \to boolean$
	  $length: dictionary \to integer$
	  $get: dictionary$ x $element \to element$
	  $insert: dictionary$ x $element$ x $element \to dictionary$
	  $remove: dictionary$ x $element \to dictionary$
	  $keys: dictionary \to iterator$
	  $values: dictionary \to iterator$