Decimals don't work in solidity.
While [[Buidling Smart Contracts]] the things you do is 
- name the solidity version.
- name the contracts

State changing function calls are Transactions.


[[Public]] keyword defines the visibility of the variable or the function

Bydefault the visibility is defined as [[Internal]] in Solidity.


There are two keywords that can specified that we are not making tany transactions : 
	- view : It means we are reading something from the blockchain
	- pure :These are funtions that only do some kind of math operations without changing any state of the blockchain.(i.e. not storing/update the value in any way)
These are non state changing functions.
Public variables automatically are "view" functions.

[[Structs]] are ways to define new types in solidity.

Storing variables in solidity always works in the numeric indexing fashion from 0 , 1, 2 ,...

[[Array]] is a way of storing a list of an object or type

[[Mappings]] is a dictionary like data structure with 1 value per key.

[[SPDX]] license are used in the top of the contacts because trust in the smart contract can be better.

All the solidity we write can be compiled and works in the [[EVM]]


[[Project 2]]

[[Project 3]]



Anytime you want to interact with an already deployed smart contract in, you will need an [[ABI]] on that contract.

[[Overflow]] in solidity is a problem which occurs when the value stored in the data type exceeds the value that can be stored, the value wraps around automatically.

A [[Library]] is similar to contracts but their purpose is that thay are deployed only once at a specific address and their code is reused.

When a function call reaches a [[require]] statement it'll check the truthiness of whatever require you have asked.


