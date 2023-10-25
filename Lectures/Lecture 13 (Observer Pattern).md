Observer Pattern
- behavioral design pattern that lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they are observing
- allows objects to keep other objects informed about events occurring within a software system(across multiple systems)
- Dynamic in that an object can choose to receive or not receive notifications at run-time
- Behavioral Design Pattern

Nomenclature
- publisher
	- issues events of interests to other objects
	- events occur when the publisher changes its state or executes some behaviors
- Subscriber
	- gets updated whenever the publisher makes events
- Issues
	- wouldn't want to couple all observables to those observable classes
	- have to implement both an observer interface and observable interface

Applicability
- when changes to one state may require changes to other states
- when some objects in app must observe others, only for a limited time however

Strategy vs Observer
- Strategy is about performing a task in different ways without changing client code
- Observer pattern is about keeping multiple objects in sync when one of them changes


