### Test Driven Development

> Phani Kandula



### Introduction


About me


About you



## Agenda
- Announcements
- TDD Concept
- Case for Automation
- Tests first or later?
- Related tasks you should consider right away
- More tasks for later
- Resources
- Demo: TDD Bowling game or Checkout?



## Announcements
- Please take survey: https://www.fullstacksoftwareengineer.com/survey
- Speak at this meetup: https://www.fullstacksoftwareengineer.com/speak 
- Silence phones etc.
- Active participation encouraged! Interrupt anytime..



## TDD 

- Test Driven Development by Kent Beck in 1990

Three steps:
- Write failing tests
- Write new code to make tests pass
- Refactor new code with existing code if necessary



## Case for automation
- Used in Continouous Integration
- Test full code base with just one command
- Gives confidence to work on the code because we have safety net of existing tests
- Encourages refactoring
- In theory, tests can be written after code is written.



## Tests first or later?
Tests first:
- Encourages thinking about API
- Sets us up interms of interface/API and injecting depdencies
- Forces good design: smaller classes, SRP (Single Responsibility Principle)
- Automagically gives us self testing code.


Tests later:
- Classes usually become too big -- too many public methods
- Might need mocking tools to mock out all the dependencies.



## Related tasks you should consider right away
- Make everything visible: documentation of API and where everything is in the code.
- Make it easy to write tests: helpers, fixtures
- Share test coverage and get feedback
- Test DB scripts



## More tasks for later
- Silence logs better
- Cycle through different test data
- Split tests into 'slow', 'fast' and run 'fast' first



## Resources
- Michael Feathers - Working effectively with Legacy Code
- Kent Beck - TDD by example, Refactoring (with Martin Fowler)
- Robert C. Martin (Uncle Bob): Clean Code etc
- Mark Seemann, Steven van Deursen - Dependency Injection Principles, Practices and Patterns.
