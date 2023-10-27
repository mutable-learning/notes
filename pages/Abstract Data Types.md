alias:: ADT 
tags:: Algorithmics
topic:: Abstract Data Types
algo:: Unit 3 Outcome 1

-
- Why create ADTs
	- Safe from bugs
		- correct today and in the future
	- Easy to understand
		- communicating clearly with other programmers and future you
	- Ready for change
		- can accommodate change without rewriting
- Key idea of ADTs
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2023-10-26T13:00:00.000Z
  card-last-reviewed:: 2023-10-25T22:19:49.357Z
  card-last-score:: 1
	- **An [[ADT]] is characterized by the operations you can perform on it**
	- The operations of the type constitute its [[Abstraction]]. This is the public part, visible to clients who use the type.
- ADTs help us to
	- separate how we use a data structure in a program from the particular form of the data structure itself
	- address the problem of clients making assumptions about the type’s internal representation
- Principles of ADTs
	- {{embed [[Abstraction]]}}
	- {{embed [[Modularity]]}}
	- {{embed [[Encapsulation]]}}
	- {{embed [[Information Hiding]]}}
	- {{embed [[Separation of Concerns]]}}
- Classifying ADTs
	- Types, whether built-in or user-defined, can be classified as
	- {{embed [[mutable]]}}
	- {{embed [[immutable]]}}
- Classifying ADT Operations
	- {{embed [[Creators]]}}
	- {{embed [[Producers]]}}
	- {{embed [[Observers]]}}
	- {{embed [[Mutators]]}}
- Designing an ADT
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
	- Abstract data types are characterised by their operations.
	  id:: 6514064f-c5ad-4873-85bc-4602ac6f5289
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