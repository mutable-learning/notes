tags:: Software Development
topic:: [[Programming Concepts]]
softdev:: Unit 3 Outcome 1

-
- Validation
	- is the process of checking that input data are reasonable
	- does not and cannot check that inputs are accurate
- input can be validated for
	- Existence
	- Type
	- Range
- Exisitence Check
	- checks whether a value has been entered at all
	- used to check that all required fields in a form have been completed before saving the data to a file
- Type Check
	- confirming that the values entered into fields are of the expected [[Data Type]]
	- consider how inputs from a user are handled by the programming language
		- by default, all inputs in Python are treated as strings, even if they only contain numeric data
- Range Check
  id:: 6542d358-8f3e-4d79-a58e-6f78d0d070a6
	- checks that data are within *acceptable limits* or come from a range of *acceptable values*
		- users must enter a score between 1 and 5 (acceptable limits)
		- the postcode must be a valid Victorian postcode (acceptable values)