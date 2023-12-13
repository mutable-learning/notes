tags:: Software Development
topic:: [[Security Strategies]]
softdev:: Unit 4 Outcome 2

-
- securing software is hard
- a balance between security and usability is determined
- verify all users and systems using [[User Authentication]] and ensure they have permissions to work with any data or system using [[User Authorisation]]
	- ensure users are always logged out of a system and that they cannot maintain indefinite login connections
- assume all sources of data are untrusted, even after [[User Authentication]]
- assume all data received is untrusted, files, images, data, cookies, emails etc
- all data inputs must be validated ([[Validation Techniques]])
- encrypt all data and communications
- use a firewall, antivirus software and adopt practices aimed at [[Minimising Security Vulnerabilities]]
- implement secure [[Software Development Practices]]
- audit and test software effectively ([[Software Auditing and Testing]])
- implement resilient [[Backup and Recovery]] strategies