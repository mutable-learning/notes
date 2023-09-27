alias:: ADT 
tags:: Algorithmics, ADT

- Why create ADTs
  background-color:: yellow
	- Safe from bugs :  correct today and in the future
	- Easy to understand : communicating clearly with other programmers and future you
	- Ready for change : Can accommodate change without rewriting
- Key Idea of ADTs
  background-color:: yellow
	- **An [[ADT]] is characterized by the operations you can perform on it**
	- The operations of the type constitute its [[Abstraction]]. This is the public part, visible to clients who use the type.
- ADTs help us to
  background-color:: yellow
	- separate how we use a data structure in a program from the particular form of the data structure itself
	- address the problem of clients making assumptions about the type’s internal representation
- Principles of ADTs
  background-color:: yellow
	- [[Abstraction]]
		- omitting or hiding low-level details with a simpler, higher-level idea.
	- [[Modularity]]
		- dividing a system into components or modules, each of which can be designed, implemented, tested, reasoned about, and reused separately from the rest of the system.
	- [[Encapsulation]]
		- building a wall around a module so that the module is responsible for its own internal behaviour, and bugs in other parts of the system can’t damage its integrity.
	- [[Information Hiding]]
		- hiding details of a module’s implementation from the rest of the system, so that those details can be changed later without changing the rest of the system.
	- [[Separation of Concerns]]
		- making a feature (or “concern”) the responsibility of a single module, rather than spreading it across multiple modules.
- Classifying ADTs
  background-color:: yellow
	- Types, whether built-in or user-defined, can be classified as [[mutable]] or [[immutable]]
	- [[mutable]] types
		- can be changed
			- they provide operations which when executed cause the results of other operations on the same object to give different results
	- [[immutable]] types
		- can't be changed
			- their operations create new objects rather than changing existing ones
- Classifying ADT Operations
  background-color:: yellow
	- [[Creators]]
		- create new objects of the type.
		- A creator may take values of other types as arguments, but not an object of the type being constructed.
	- [[Producers]]
		- create new objects of the type from one or more existing objects of the same type.
	- [[Observers]]
		- take objects of the abstract type and return objects of a different type. The size operation of List, for example, returns an integer.
	- [[Mutators]]
		- change objects. The add operation of List, for example, mutates a list by adding an element to the end.
- Designing an abstract type
  background-color:: yellow
	- aim for a few, simple operations
	- aim for operations to be combined in powerful ways
	- avoid lots of complex operations.
	- each operation should have a well-defined purpose
		- We probably shouldn’t add a sum operation to List, for example. It might help clients who work with lists of integers, but what about lists of strings? Or nested lists? All these special cases would make sum a hard operation to understand and use.
	- each operation should have a coherent behaviour rather than a collection of special cases.
	- The set of operations should be adequate in the sense that there must be enough to do the kinds of computations clients are likely to want to do.
	- The type may be generic: a list or a set, or a graph, for example. Or it may be domain-specific: a street map, an employee database, a phone book, etc.
		- It should not mix generic and domain-specific features.
	- Representation independent.
		- Use of an abstract type is independent of its representation (the actual data structure or data fields used to implement it), so that changes in representation have no effect on code outside the abstract type itself
- Summary
  background-color:: yellow
	- Abstract data types are characterised by their operations.
	- Operations can be classified into creators, producers, observers, and mutators.
	- An ADT’s specification is its set of operations and their specs.
	- A good ADT is simple, coherent, adequate, and representation independent.
	- An ADT is tested by generating tests for each of its operations, but using the creators, producers, mutators, and observers together in the same tests.
-
- Further Research
  background-color:: purple
	- Read
		- [Abstract data type - Wikipedia](https://en.wikipedia.org/wiki/Abstract_data_type)
		- [Abstract Data Types | Brilliant Math & Science Wiki](https://brilliant.org/wiki/abstract-data-types/)
		- [Abstract Data Types (ADT): Defining 'What' not 'How' - αlphαrithms](https://www.alpharithms.com/abstract-data-types-adt-495117/)
		- [MIT: Abstract Data Types](https://ocw.mit.edu/ans7870/6/6.005/s16/classes/12-abstract-data-types/)
		- [Abstract data types — Object-oriented Programming  documentation](https://object-oriented-python.github.io/5_abstract_data_types.html)
	- Watch
		- {{video https://www.youtube.com/watch?v=SFEROgwxicA}}