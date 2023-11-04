tags:: Software Development
alias:: UCD
topic:: [[Analysis Actions]]
softdev:: Unit 3 Outcome 2

-
- is a visual representation of the interactions between a system and its users
- is used to capture the functional requirements of a system and to communicate them to stakeholders
- usually completed before any [[Context Diagram]] or [[Data Flow Diagram]] is created
- Use Case
  id:: 654593c7-6dc7-41eb-9f9e-1e01c35fde80
	- describe interactions or functions a user can complete in the system
- are created using the Unified Modelling Language (UML)
	- a standard notation for modelling software systems
- UCD components
	- Actors
	  id:: 654593c7-cf55-4cb3-a175-d21da31fbc49
		- represent the users of the system
		- other external systems that interact with it
		- is a role, not an actual person or system's name
		- represented with a stick figure
	- Use cases
		- represent the different ways that users interact with the system to achieve their goals
		- broad, simple name to represent functionality within the system
			- should begin with a verb
			- should be short, two or three words
		- can be connected to other use cases or actors with relationships
	- Relationships
		- Associations
			- show a relationships between actors and use cases or between two use cases
			- drawn with a solid line and is the default relationship
		- Generalisations
			- a type of relationship between two use cases in a use case diagram indicating inheritance
			- indicates that the child use case inherits the behaviour and structure of the parent use case
				- the child may have additional behaviour or structure of its own
			- often used to model common functionality that is shared by multiple use cases
				- for example a parent case might be *Withdraw Money* and the child cases are *Withdraw Money from EFTPOS*, *Withdraw Money from ATM*, and *Withdraw Money Online*
			- drawn with a solid line and a closed arrow at the parent end
		- Include
			- indicates that one use case is completely included in another
				- when the use case is run all the functions of the included use case are also run at least once
				- it is required that they work together, such as you must *log in* before you can *update your account*
			- shown with a dashed line and arrow head pointing toward the use case that will be included
				- surround the word 'include' <--<< include >> -- in double angle brackets
		- Extend
			- indicates that one use case may sometimes be used by another
				- it is an optional extension that can be accessed
			- shown with a dashed line and arrow head pointing toward the use case that will be extended by the functionality of the other use case
				- surround the word 'extend' <--<< extend >> -- in double angle brackets
	- System Boundary
		- shows a 'boundary' around the use cases that make up a system
		- actors exist outside the boundary and relationships between actors and use cases are shown across the boundary
		- drawn as a solid rectangle around the use cases
- ![Use Case Diagram - wikipedia](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1d/Use_case_restaurant_model.svg/1280px-Use_case_restaurant_model.svg.png){:height 856, :width 848}
-
- Further Research
  background-color:: purple
	- Read
		- [Use case diagram - Wikipedia](https://en.wikipedia.org/wiki/Use_case_diagram)
	- Watch
		- {{video https://www.youtube.com/watch?v=uNtoyXJ1VDc}}
		  id:: 4dc136c4-724b-47a4-a158-b619598f88e7