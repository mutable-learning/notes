tags:: Software Development
topic:: [[Development Techniques]]
softdev:: Unit 4 Outcome 1

-
- a software development practice in which individual units or components of a software system are tested separately to verify that they work as intended
	- a unit can be a small piece of code, such as a [[Processing Feature/Function]] or a [[Processing Feature/Class]] , or it can be a larger component, such as a module or a service
- helps to ensure that the individual components of the software work as expected before they are integrated into the larger system
- can help to prevent problems from being introduced into the system later, which can be costly and time-consuming to fix
- Unit Testing characteristics
	- tests are isolated
		- isolated from each other and from the rest of the system
			- each unit test should test a single component of the system
			- the results of one unit test should not affect the results of another unit test
	- tests are repeatable
		- can be run over and over again as needed, especially when code changes are made
	- tests are automated
		- can be run by a process making it possible to run a large number of unit tests quickly and easily
-