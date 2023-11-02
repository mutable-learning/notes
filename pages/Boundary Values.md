tags:: Software Development
topic:: [[Software Errors]]
softdev:: Unit 3 Outcome 1

-
- Boundary Value Analysis (BVA)
	- a software testing technique that tests the boundaries of a software program's input and output values
	- based on the principle that software programs are most likely to fail at the edges of their input and output ranges
		- because the code that handles these values is often the most complex and difficult to test
- first identify the input and output ranges of the software program
- then test the program with values at the edges of these ranges, as well as slightly inside and outside of the ranges
	- these are the *Boundary Values*
	- the maximum and minimum values
- if a software program has an input range of 1 to 100, the tester would test the program with the values 1, 100, 101, and 0
	- maximum and minimum acceptable values
	- closest invalid values
- particularly useful for testing software programs with complex input and output requirements that require extensive use of {{embed ((6542d358-8f3e-4d79-a58e-6f78d0d070a6)) }}
- tips to perform BVA
	- identify the input and output ranges of the software program
	- use [[Test Data]] to test the program with values at the edges of these ranges
		- as well as outside of the ranges
	- test the program with valid and invalid values
	- test the program with combinations of valid and invalid values