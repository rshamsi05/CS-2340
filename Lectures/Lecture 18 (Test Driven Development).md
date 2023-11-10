Verification: checking implementation
Validation: checking implementation against client's needs

Approaches to verification
- Testing: exercising software to try and generate failures 
	- Pro: no false positive
	- Con: highly incomplete
- Static Analysis: identify problem statically(consider all possible executions)
	- Pro: Consider all program behaviors complete
	- Con: False Positives, and is expensive
- Inspection: systematic group review of program 
	- Pro: Systematic, thorough
	- Con: Informal subjective
- Formal Verification: proving that the program implements the program specification
	- Pro: Strong guarantees
	- Con: Complex and expensive

Testing levels
- Unit Testing -> Integration -> System Testing -> Acceptance Testing -> Regression Testing

Testing Stages
1) Developer Testing
2) Alpha Testing: Different group tests the program that is not the dev but still in org
3) Beta Testing: Release software to few people
4) Product Release

BlackBox vs Whitebox testing
- Blackbox: don't know about the code
- Whitebox: we know about the code

Test Driven Development
- tests written before the class to be tested, and the dev writes unit testing for nearly all production code
- Write test code
- Write functional code
- 