- Focuses on design of individual classes and relationships
- Acronym
	- S: single responsibility principle
	- O: open closed principle
	- L: Liskov substitution principle
	- I: Interface segregation principle
	- D: Dependency inversion principle
- Purpose
	- make code more maintainable

Single responsibility
- one class should be responsible for only one task
- all other classes have their own individual tasks and work together to form high cohesion
- Benefits
	- interface has smaller number of methods
	- changes related to class responsibility are fairly isolated

Open Closed principle
- software entity should be open to extension but should not open to modification or changes in purpose

Liskov Substitution Principle
- objects of a super class should be replaceable with objects of a subclass without breaking the application
	- all objects of the subclass should be able to logically perform the same methods in the superclass

Interface Segregation Principle
- do not make large multipurpose interfaces, instead use smaller focused intefaces

Dependency Inversion Principle
- High levels modules should not depend on low level modules, both should depend on abstractions
- Details should depend on abstractions, but not the other way around

Note: do not get trapped by SOLID and over fragment code for the sake of the design pattern