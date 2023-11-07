tags:: Software Development
topic:: [[Development Techniques]]
softdef:: Unit 4 Outcome 1

-
- [[Storage Media]] use bytes to measure the size of data
- when data is transferred between devices or networks, the speed is usually measured in *bits per second*
	- there are 8 bits of data in every byte stored
- a 1 MB (megabyte) file will require 8 Mb (megabits) of data transfer
	- so if a connection has a speed of 1 Mbit/s it will take 8 seconds to transfer the file
- Transmission Technology considerations
	- Speed
		- how quickly data can be transferred between different systems
		- can be especially important for large datasets or for applications that require real-time data access
			- emergency response systems
	- Latency
		- how long it takes for data to be transferred between different systems
		- can be especially important for applications that require real-time response, such as online gaming or video calls
	- Reliability
		- how often data is lost or corrupted in transit
		- especially important for applications that require high [[Data Integrity]]
	- Security
		- how vulnerable the data is to unauthorised access or modification in transit
			- HTTP vs HTTPS
		- especially important for applications that transmit sensitive data
- types of Transmission Technologies
	- Local Area Networks (LANs)
		- are typically very fast and reliable, with low latency
		- makes them a good choice for applications that require real-time data access or high data integrity
			- can be expensive to setup and maintain
	- Wide Area Networks (WANs)
		- are typically slower and less reliable than LANs, with higher latency
		- makes them a poorer choice for applications that require real-time data access
		- common for projects with systems at multiple company locations
	- Wireless networks
		- can be convenient and flexible
		- can also be less reliable than wired networks
	- Mobile networks
		- can be convenient and flexible, but they can also be slower and less reliable than other transmission technologies
		- makes them a poorer choice for applications that require high [[data integrity]] or real-time data access
		- may be good for regional application where NBN access is unavailable or unreliable
	- Cloud-based storage
		- can be a convenient and scalable way to store data
			- important to choose a cloud provider that offers a reliable and secure service