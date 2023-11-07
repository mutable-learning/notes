tags:: Software Development
topic:: [[Development Techniques]] 
softdev:: Unit 4 Outcome 1

-
- used to systematically test that code works
- Test Case
	- is a set of steps that a tester uses to determine if the element being tested works correctly
- important to select appropriate test data so that test cases can be run
- four main types of test data
	- Validation test data
		- used to test the validation techniques that have been included in the module
		- if a module requires a valid email address
			- validation test data would include invalid email addresses to check that the module correctly rejects them
	- Boundary test data
		- used to test the module at the edges of its operating range or [[Boundary Values]]
		- if a module calculates the area of a triangle
			- boundary test data would include triangles with zero or negative base or height values
	- Negative test data
		- used to test the module with invalid inputs
		- if a module calculates the square root of a number
			- negative test data would include negative numbers
	- Positive test data
		- used to test the module with valid inputs
		- if a module calculates the square root of a number
			- positive test data would include positive numbers
- good Test Data will
	- make sure the test data is representative of the real-world data that the module will be used with
	- use a variety of test data values to cover all possible scenarios
	- use boundary test data to test the module using [[Boundary Values]]
	- use invalid test data to test the module's ability to handle errors