Design Tradeoffs
- with inheritance
	- code reuse
	- common behavior
- with Interfaces
	- specificity
	- no code reuse

Design Principles(3 patterns)
- Protected Variations
	- identify the aspects of your application that vary and separate them from what stays the same
- Program to an interface not an implementation
	- Program to a supertype
- Favor composition/aggregation over inheritance

Strategy Pattern
- defines family of algorithms, encapsulates each one, and makes them interchangeable
- Strategy lets the algorithm vary independently from clients that use it
- Structure
	- Algorithm is pulled out of client Client only makes use of the public interface of Algorithm and is not tied to concrete subclasses
	- Client can change its behavior by switching among the various concrete algorithms 
- Splits the different strategies from the context
- code in the context is unchanged if 
	- a strategy contains a bug and si fixed
	- 