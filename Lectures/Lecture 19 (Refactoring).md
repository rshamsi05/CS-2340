Goal: keep program readable and understandable, not too fix code
Key Feature: behavior pressing- makes sure the program works after each step(small steps)

Preserving the behavior
- cannot guarantee code runs the same before and after
- we run test cases before and after refactoring

Ways to refactor code
- Renaming
- Collapse hierarchy: if super class and subclass are too similar, merge them
- Consolidate conditional: 
	- if there is a cohesive code fragment in large method, create a method with the code fragment and call the method.
	- if there is a set of conditionals with the same result, combine and extract them
- Decompose conditional
	- if a conditional is particularly complex, extract methods from conditions and give the right name to the extracted method 
	- modify the conditional structure
- Extract class
	- if a class is doing the work of two classes. Create a new class and move the relevant fields/methods
	- Complies with high cohesion and low coupling
- Extract method

Industry Standards
- floss refactoring: small scale refactoring, performed by a single developer; manual
- Large Scale refactoring: takes months and sometimes adding new features become priority
- Inspecting code
	- can use SonarQube: code quality control tool before completing pull request
		- min grade of B