tags:: Software Development
topic:: [[Data Structures]]
softdev:: Unit 3 Outcome 1

-
- is a type of [[Data Structure/Associative Array]]
- uses a key-bucket relationship to store data
- uses a hash function to compute an index location to store a value in a one-dimensional [[Data Structure/Array]]  and is called a *bucket*
	- the hash value index is the location of the bucket where the value is stored
	- the key is used to generate the hash value index
		- a key is determined from the value to be stored
- a good hash function will not store multiple values in one bucket, each value will generate a unique index from the key
- when multiple values are stored in the same bucket that is called a *collision* and must be managed by the hash table implementation