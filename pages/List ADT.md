tags:: Algorithmics
alias:: List
topic:: [[Abstract Data Types]]
algo:: Unit 3 Outcome 1

-
- List
  background-color:: yellow
	- are of dynamic size
	- have elements ordered within the list
	- have an index assigned to each element to indicate its position in the array
	- allow elements to be repeated with each having its own unique index value
	- In general, the data in a List is homogeneous, such as a list of integers, or a list of strings. However, a list can also be heterogeneous.
		- It depends on the specific application and whether the List needs to ensure the data is consistent or allow for more flexibility.
- List Definition
  background-color:: red
	- **Name:** $List$
	  **Import:** $element, boolean, integer$
	  
	  Operations:
	  $create: \space\to list$
	  $empty: list \to boolean$
	  $length: list \to integer$
	  $get: list$ x $integer \to element$
	  $set: list$ x $integer$ x $element \to list$
	  $head: list \to element$
	  $tail: list \to list$
	  $prepend: list$ x $element \to list$
	  $append: list$ x $element \to list$