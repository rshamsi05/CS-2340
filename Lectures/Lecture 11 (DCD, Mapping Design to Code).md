Design Class Diagram(DCD)
- shows software entities rather than real world concepts
- Diagram of one class
	- class name in top of box
		- writes interface on top of interfaces names
		- use italics for an abstract class name
	- attributes(optional)
		- should include all fields of object
	- operations
		- may omit trivial methods
		- but don't omit any methods from an interface
		- should not include inherited methods

Class attributes
- attributes(fields, instance variables)
- visibility:
	- public(+)
	- protected(#)
	- private(default)
	- derived (/)
- derived attribute: not stored but can be computed from other attributes
- attribute example: -balance: double = 0.00

Class operations/methods
- operations/methods
	- visibility name(parameters): return type
- Same visibility as attributes, but default is public
- parameter types listed as (name: type)
- omit: return type is void
- method example: +distance(p1: Point, p2: Point): double

Comments/Note
- note symbol attached to the appropriate class by a dashed line may represent several things
	- UML note or comment
	- UML constraint 
	- Method body

Relationships in DCD
- Generalization: X is a Y(Straight arrow)
	- inheritance between classes or interface
- Realization: X is a Y(dotted arrow)
	- interface implementation
- Associations: X and Y are related(has, straight arrow that does not have triangle end)
	- can be dependency, aggregation, or composition
	- can be unidirectional
- Dependencies: X uses Y(dotted arrow with filled triangle head)
	- methods of a class that uses another class's object as a parameter
- Aggregations: X has a Y(arrow with square hollow head)
	- relations between the whole and the part(parent and child), but the part can exist independent of the whole system
- Composition: X has a Y(arrow with square filled head)
	- part cannot exist independent of the whole system

Generalizations
- hierarchies drawn top-down
- arrows point upward to parent
- line/arrow styles indicate whether parent is:
	- class:
		- solid line, black arrow
	- interface:
		- dashed line, white arrow(also called realization, relationship)
- often omit trivial / obvious generalization relationships, such as drawing the Object class

Association types
- aggregation: is part of
	- child can exist independently of the parent
- composition: is entirely made of
	- stronger version of aggregation
	- the parts live and die with the whole
	- child cannot exist independent of the parent
	- symbolized by a black diamond
- dependency: "uses temporarily"
	- symbolized by dotted line
	- often is an implementation detail, not an intrinsic part of that object state

Mapping Design to Code
- Creating Class definition from DCD
- 