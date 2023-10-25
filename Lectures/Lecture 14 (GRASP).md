What are design principles
- set of guidelines for designing software using OOP principles
- help developers create software that is easy to understand, maintain, and extend
- 3 Characteristics to avoid
	- 1) Rigidity: hard to change because every change affects too many other things
	- 2) Fragility: when you make a change, unexpected parts of the system break
	- 3) Immobility: hard to reuse in another application because it cannot be disentangled from current apps
- 2 sets of design principles
	- 1) SOLID
		- focuses on design of individual classes and relationships between them
	- 2) GRASP
		- focuses on responsibilities within a system
GRASP
- talks about the responsibility
	- accomplished by a single object
	- or a group of object collaboratively accomplish a responsibility
- 9 patterns
	- 5 basic 
		- 1) creator: who creates an object
		- 2) Information expert: given an object which responsibilities does it have
		- 3) Low coupling: how strongly the objects are connected
		- 4) high cohesion: how to delegate the request from the UI layer objects to domain layer
		- 5) Controller: how are the operations of any element are functionally related
	- 4 advanced

Creator Pattern
- who is responsible for creating a new instance of a class
- Rules: Assign class B to create class A if:
	- B contains or aggregates A
	- B has initializing data for A
	- B records A
	- B closely uses A

Information Expert
- assign responsibility to the class that has the info necessary to fulfill the responsibility
- e.g) Factory method relies on the expertise of the concrete creator to instantiate the appropriate product

Low Coupling
- measure of how strongly one element is connected to 
- assign responsibilities so that coupling remains as low as possible
- Avoid bidirectional relationship between modules
- Interfaces reduce coupling
- Types of coupling(Worst to best)
	- Content: one class modifies another
	- Common: share common data
	- Control: use a method parameter to control a different method
	- Stamp/Data: passing complex data or structures between modules
		- we should aim for this
		- use primitive data types when possible
	- Uncouple: no relationship
		- almost not possible

High Cohesion
- how functionally related the operations of a software elements are
- Types of cohesion(Worst to best)
	- Coincidental: unrelated functions
	- Logical: multiple logic sections
	- Temporal: related by phrases of an operation
	- Procedural: required ordering of tasks
	- Communicational: operates on same data set
	- Functional: all essential elements for a single function are in same module

Controller Pattern
- What is the first object past the UI that receives and coordinates a system operation
- Assign responsibility to a class that:
	- represents the overall system
	- represents a Use Case scenario where event occurs 