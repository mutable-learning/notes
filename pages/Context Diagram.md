tags:: Software Development
topic:: [[Analysis Actions]]
softdev:: Unit 3 Outcome 2

-
- is a high-level graphical representation of a system and its interactions with its external environment
- is a type of [[Data Flow Diagram]] that shows the system as a single process, with its inputs and outputs to and from external entities
	- sometimes referred to as a Level 0 data flow diagram
- is an abstract representations of a system
	- does not include any specific details about the system's implementation or technology
- simple and easy to understand, even for people who are not familiar with the system
	- show limited detail, focussed only on data flowing into and out from the system
- Context Diagram Components
	- Process
		- is an abstract representation of the entire system
		- in most cases only one process will display in a context diagram
		- drawn as a circle with the name of the system inside
	- Entity
		- can be one or more entities shown
		- are the users or external systems that interact with processes (the system)
			- *cannot interact with other entities*
		- drawn as a rectangle with a role label in the same manner as ((654593c7-cf55-4cb3-a175-d21da31fbc49)) in a [[UCD]]
	- Data Flow
		- data or a logical collection of data moving into or out from the system
		- connect entities to the system process
			- *cannot exist between entities*
		- drawn with a solid line connecting an entity with the system process
			- an arrow represents the direction of the flow
			- arrows at both ends to represent bi-directional flow are possible, but rare
- ![Context Diagram](https://venngage-wordpress.s3.amazonaws.com/uploads/2022/04/Business-context-diagram.jpg)
-
- Further Research
  background-color:: purple
	- Read
		- [What is a Context Diagram (and How Can You Create One)? - Venngage](https://venngage.com/blog/context-diagram/)
	- Watch
		- {{video https://www.youtube.com/watch?v=fWNrc6GNK14}}