tags:: Software Development
topic:: [[File Management]]
softdev:: Unit 4 Outcome 1

-
- managing file access is a key part of [[File Management]] and is about more than just [[User Authentication]] and [[User Authorisation]]
- File Access concerns
	- concurrent access
		- does the system need to allow for multiple users or process to access the same files at the same time
			- how will the system handle this if it happens
	- data consistency
		- if one user is writing to a file, other users should not be able to read from the file until the write operation is finished
	- file durability
		- data should not be lost even if the system crashes or loses power
	- performance
		- files need to be read and write quickly, especially for large files or ones accessed frequently
	- security
		- unauthorised access should be prevented
		- [[User Authentication]] and also [[User Authorisation]] are needed to secure file access
		- encryption of files may also be appropriate
	- interoperability
		- multiple different systems may be accessing files and data, and they all need to work
		- which file format is the best to use for all systems to function ([[XML file]], [[CSV file]] or [[Text file]] )