tags:: Software Development
alias:: DFD
topic:: [[Analysis Actions]]
softdev:: Unit 3 Outcome 2

-
- is a graphical representation of the flow of information through a system
	- uses standardised symbols and notation to show the system's inputs, outputs, processes, and data stores
- DFDs can be used to model both existing and proposed systems
- focus on the logical flow of information through a system, rather than the physical implementation of the system
- can be decomposed into lower-level diagrams that show more detail about the system's processes
- can be used to model complex systems by breaking them down into smaller, more manageable modules
- DFD components
	- Process
		- not the same as a ((654594d6-e82f-40c5-a48c-92e493238fa6)) in a [[Context Diagram]]
		- represents a whole function within a system
		- usually at least one process for each ((654593c7-6dc7-41eb-9f9e-1e01c35fde80)) in the [[UCD]]
		- **must have at least one input data flow and one output data flow**
		- drawn with a circle and a label
			- process names begin with a verb and are short (they are a function)
			- *validate user*, *calculate order* or *export report*
		- can be connected to entities, other processes or data stores
	- Entity
		- can only be connected to processes
			- **cannot directly interact with data stores or other entities**
		- the rules and use are the same as an ((654595db-8475-4cc4-916f-98b37a4f423b)) in a [[Context Diagram]]
		- entities can be drawn repeatedly to make the diagram easier to understand
	- Data Flow
		- must always be coming from or going to a process
		- the rules and use are the same as a ((6545970c-4d59-4796-8831-73ef8b34caf8)) in a [[Context Diagram]]
		- cannot directly connect data stores together
			- a process must always be at least at one end of a data flow
		- should be drawn so that no flows cross over the top of other flows
	- Data Store
		- represents a collection of data that is stored in some way
			- a file, database, storage media
		- data is stored in a data flow when a data flow directs into it
		- data is retrieved from a data store when a data flow directs out from it
		- drawn with two parallel lines and a label between them (usually)
			- some other symbols are also used but they are similar
		- can only connect to processes with a data flow
		- almost always will have at least one input and one output data flows
	- ![Data Flow Diagram](https://i.pinimg.com/originals/13/1a/1f/131a1f3085c2e9c1452214f4d4ae501e.png)
- ![Data Flow Diagram](https://sparxsystems.com/enterprise_architect_user_guide/15.0/images/title-order-to-delivery-level-one-5830.png)
-
- Further Research
  background-color:: purple
	- Read
		- [Data-flow diagram - Wikipedia](https://en.wikipedia.org/wiki/Data-flow_diagram#See_also)
	- Watch
		- {{video https://www.youtube.com/watch?v=YbD3oy181s8}}