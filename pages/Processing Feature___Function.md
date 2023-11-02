tags:: Software Development
topic:: [[Processing Feature]]
softdev:: Unit 3 Outcome 1

-
- a named [[Processing Feature/Sequence]] of  [[Processing Feature/Instruction]]s
- a generic term used by programmers to describe the structure that stores a block of code and can be executed by calling it by name
- can have **parameters** specified in the function declaration which allow for values and objects to be made available to the functions statements when it is executed ( **arguments** )
	- these arguments are assigned to temporary variables when the function is called and are *local* to the function
	- they don't exist outside the function
	- different languages pass data into functions in different ways using as arguments
		- by reference
			- the original data will be modified if it is changed during the function's execution
		- by value
			- the original data is not changed during the function's execution
- languages often allow functions to have access restrictions
	- depends on the language implementation
		- Private
		- Public
		- Protected
- Subroutine
	- a general name for a structure that stores a block of statements and can be executed with a call using its name
- Function
	- a subroutine that returns a value when executed
- Procedure
	- a subroutine that doesn't return a value when executed
- Method
  id:: 65421482-6808-45d6-a8c2-6cf29d278c75
	- a function or procedure that is part of an object ( belongs to a [[Processing Feature/Class]] )
	- Class Method
		- is shared by all objects of the same class
		- can be called without an instance object by using the generic class type object
	- Instance Method
		- is defined in the class type
		- can only be called on an object instance of the class
- {{embed ((6540dff6-8035-491b-a86d-536b2812bfe7))}}
	-