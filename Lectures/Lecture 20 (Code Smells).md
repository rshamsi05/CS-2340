Corresponds to a surface indication that there is a deeper problem in the system
Where do they come from?
- usually comes from a rushed design and disregard for technical debt 
	- Doing it the right way: use best practices and develop a design that can scale and grow; takes longer
	- Doing it the fast way: hacked together
Taxonomy of bad code smells
- Bloaters: something that has grown so large that it cant be effectively handled
	- A class contains fields/lines of code that may be duplicated
	- Treatment: extract class, extract subclass, and extract method
- Object orientated abusers: cases where the solution does not fully exploit the possibilities of object orientated design
- Change preventers: smells that hinder changing or further developing software
- Dispensable: somethin unnecessary that should be removed 
- Couplers: a measure of how closely connected two routines or modules are