Decorator Pattern
- Structural pattern
- attach new behaviors to objects dynamically without altering structure
	- done by using special wrapper objects that encapsulate the added functionalities

Problem with inheritance
- extending a class has several serious issues 
	- it is static: can not alter the behavior of an existing object at runtime
	- subclasses can only have one parent class 
- One way to overcome this is Aggregation or Composition

Base Decorator
- abstract class that also implements the interface

Key Objectives
- Maintain Interface Compatibility
	- base decorator implements the component interface to ensure that it is compatible with the concrete components and other decorators 
	- allows decorator to be interchangeable and stackable
- Wrap and Delegate Functionality
	- composition relationship between the base decorator and the component allows the decorator to wrap the component and delegate method calls to the wrapped object
	- enables decorator to add, modify or extend the behavior of the component without altering the components structure or implementation