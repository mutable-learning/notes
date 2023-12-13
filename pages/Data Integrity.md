tags:: Software Development
topic:: [[Security Strategies]]
softdev:: Unit 4 Outcome 2

-
- secure systems ensure that confidentiality, integrity and availability are maintained
- Threats to Data Integrity
  id:: 65718797-21ee-420b-b49d-befd0c9e975f
	- Accidental
	  id:: 65718797-7672-45da-bb63-2c6c4aa27597
		- users accidentally damage systems
		  id:: 65718797-df32-4efc-a1ef-5f2494f66da5
			- poor interfaces
			- lack of training
		- inappropriate permissions
		- user inattention or carelessness
		- modifications of data are too easy to make
	- Event-based
	  id:: 65718797-1f10-4fb9-898b-05d0fe33150a
		- hardware failure, such as storage
		- power failure
		- file corruption
		- third-party software issues
		- acts of nature such as fire, floods or a lightning strike
	- Deliberate
	  id:: 65718797-cd9d-42f0-8279-a3ee06ce164b
		- an attack is made on the system or data through [[Malware]], [[Social Engineering]] or other [[Security Vulnerabilities]]
- Characteristics of Data Integrity
	- Accuracy
		- Content
			- Correctness
				- data is entered correctly, such as correct birthdate, name spellings
			- Completeness
				- the entire data set is intact
		- Form
			- Clarity
				- data is formatted to avoid misinterpretation
				- using ISO date formats, for example
			- Consistency
				- data within a system and the same data stored in multiple systems is consistent
				- if not consistent, which data is 'accurate'?
	- Authenticity
		- comes from the source it is known to be from
		- has not been corrupted or changed
		- is not faked or disguised as something else
	- Reasonableness
		- the data meaning is consistent with the values
		- meaning is determined by understanding the acceptable extent of the data
			- dates are within a range
			- ages are consistent
			- possibility of data occurring, such as playing so many games within a time period
	- Relevance
		- data is appropriate for the use it is being applied
	- Timeliness
		- data must be processed while it is current
		- processing must complete before the data is actually needed
			- a machine alerts that the patient's heartbeat has stopped five minutes after it actually stopped
- Failure to protect Data Integrity
	- can result in prosecution and/or penalties
	- loss of business and reputation
	- normal business can be seriously disrupted
	- trade secrets can be stolen and sensitive information, such as encryption keys, may be stolen
	- business severely impacted may no longer be able to operate