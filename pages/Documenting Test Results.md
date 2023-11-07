tags:: Software Development
topic:: [[Development Techniques]]
softdev:: Unit 4 Outcome 1

-
- when any type of testing is carried out it is important to document the results of the testing
- the process for this documentation should be part of the [[Testing Strategy]] documentation
- Test Report
	- a document that presents the results from conducting a test as part of the [[Testing Strategy]]
- steps to create a Test Report
	- follow the process for [[File Organisation]] and [[File Naming Conventions]] to create a new file for any test report
	- use a consistent structure, theme and formatting for all test reports
		- aim for ease of reading and accessing test results and findings
	- include clear and concise descriptions
		- descriptions of the testing, test cases and test data
		- any defects found
	- use screenshots and recordings
		- provide evidence of defects and testing visually for stakeholders
	- share the report
		- stakeholders should have access to testing reports
- Testing Table
	- a commonly used way to record evidence of testing
	- typically contains
		- test case ID
			- the identifier of this test case so more details about it can be found in the [[Testing Strategy]] documentation
		- test case description
			- purpose of the test case and short details
		- expected result
			- what the solution is expected to output
		- actual result
			- what the solution's result was
		- status
			- PASS, FAIL, WAITING etc
		- notes
			- additional info related to the test case and the status produced
	- | Test Case ID | Test Case Description | Expected Result | Actual Result | Status | Notes |
	  |---|---|---|---|----|---|
	  | TC-1 | Login to the application | The user should be able to login to the application successfully. | The user is able to login to the application successfully. | PASS | |
	  | TC-2 | Add a new user | The user should be able to add a new user successfully. | The user is able to add a new user successfully. | PASS | |
	  | TC-3 | Edit an existing user | The user should be able to edit an existing user successfully. | The user is unable to edit an existing user successfully. | FAIL | user's name is not saved. |
	  | TC-4 | Delete a user | The user should be able to delete a user successfully. | The user is able to delete a user successfully. | PASS | |
	-