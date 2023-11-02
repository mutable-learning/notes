tags:: Software Development
topic:: [[Programming Concepts]]
softdev:: Unit 3 Outcome 1

-
- software needs to be checked to ensure it works and meets the design specifications
- [[Software Testing]] involves running many different types of testing throughout the development of software, and one process used extensively by developers is *Debugging*
- Debugging
	- a process to test for errors in software
	- includes the use of tools such as a [[Trace Table]] and often requires [[Test Data]]
- three types of error occur in software
	- Syntax Error
	- Runtime Error
	- Logic Error
- Syntax Error
	- occur due to the code containing incorrect syntax the compiler or interpreter can't understand
	- software will not run or compile
	- easy to fix once found
- Runtime Error
	- software will compile and run
	- error occurs during the use of the software and it crashes (unexpected error)
	- dividing by zero or referencing an element in an array at an index that doesn't exist are examples
	- only occurs when certain conditions are met such as unexpected input
	- harder to find
- Logic Error
  id:: 6542ddd0-2ff2-47d2-8719-c312231b6c83
	- software will compile and run
	- software does not work as expected or returns unexpected output
		- the algorithm is not correct
	- can be difficult to find and understand
	- extensive testing with good [[Test Data]] is required to eliminate this type of error
	-