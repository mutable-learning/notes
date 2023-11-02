tags:: Software Development
topic:: [[Programming Concepts]]
softdev:: Unit 3 Outcome 1

-
- a set of rules followed when creating variables and objects in source code
- provides consistency and clarity to developers
- can add meaning to objects not instantly identifiable otherwise
	- often used to provide information about the purpose of the object
	- can be used to inform about the object's data type or structure
- many programming languages have conventions about naming conventions
	- how to use them for various different objects
	- Python's naming conventions are listed in [PEP 8](https://peps.python.org/pep-0008/#naming-conventions)
- aim is to make code easier to read and understand
- Camel Case
	- words are combined without spaces
	- each word after the first is capitalized
	- long names should be avoided
	- allows for some meaning to be provided to the object with its name
	- readInputFromFile
- Snake Case
	- words are combined with an underscore (_)
	- all lowercase and underscores instead of spaces
	- may be easier for humans to read the words
	- read_input_from_file
- Hungarian Notation
	- words are combined without spaces
	- each word after the first is capitalized
	- adds a *prefix* to the beginning of the name
		- a combination of lowercase letters
		- indicate the [[Data Type]] or [[Data Structure]] of the object
	- fnReadInputFromFile returns a value to strFileContents
	- can lead to inconsistency when code is changed (refactored)
	- not as commonly used in modern software development