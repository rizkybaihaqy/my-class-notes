# Modifiability

## What is Modifiability?

Modifiability can be defined as the ease with which changes can be made to a system, and the flexibility at which the system adjusts to the changes.

### Modifiability Is About The Following

- Difficulty: The ease with which changes can be made to a system
- Cost: In terms of time and resources required to make the changes
- Risks: Any risk associated with making changes to the system

#### Three Levels of Changes

- Local: A local change only affects a specific  piece of code such as a function, a class, a module, or a configuration. The change __does not cascade__ to the rest of the system.

- Non-Local: For example Modifying a database schema, which then needs to cascade into the model class representing that schema in the application code.

- Global: Involve architectural changes like Changing a system's architecture from RESTful to messaging (SOAP) based web services

## Aspect of Modifiability

- [Readability](readability.md): Readable code written in a specific style, following guidelines adopted for the programming language used, and whose logic uses the features provided by the language in a concise, clear way.

- Modularity: Software system is written in well-encapsulated modules, which do very specific, well-documented functions.

- Reusability: Don't Repeat Yourself.

- Maintainability: Metric, which encompasses the aspects of modifiability.

> There's still a lot to cover on readability. [Read more about Readability on its own pages](readability.md)

## Fundamentals of Modifiability – Cohesion & Coupling

Cohesion How tightly the responsibilities of a module are related to each other. A module which performs a clear specific task or group of related tasks has high cohesion.

Coupling degree to which the functionality of two modules A and B are related. Two modules are strongly coupled if their functionality overlaps strongly at the code level—in terms of function or method calls.

In the nutshell __High Cohesion Good, High Coupling Bad__.

> Other factor like module, team, and dependencies size may take part

### Measuring cohesion and coupling

> TODO

## Exploring Strategies For Modifiability

- Providing explicit interfaces: explicitly tell which the module considers internal.

- Reducing two-way dependencies: can be broken by encapsulate all related functions in the same module.

- Abstract common services: Usage of helper modules which abstract common functions and methods can reduce coupling and increase cohesion between two modules.

- Using inheritance techniques: use class.

- Using late binding techniques: postponing the binding of values to parameters as late as possible in the order of execution of a code
  - Plugin mechanisms
  - Brokers/Registry lookup services
  - Notification services
  - Deployment time binding
  - Using creational patterns

## What are code smells?

Code smells are surface symptoms of deeper problems with your code. Code smells are not bugs themselves, but they are patterns that indicate that the approach to solving problems adopted in the code is not right, and should be fixed by refactoring.

### Some Of The Common Code Smells

- Class Level
  - God Object
  - Constant Class
  - Refused Bequest
  - Freeloader
  - Feature Envy
- Method/ Function Level
  - Long method
  - Parameter Creep
  - Cyclomatic complexity
  - Overly long or short identifiers

## Code Refactoring

1. Fix complex code first
2. Do an analysis of the code
3. Fix code smells next
4. Run checkers
5. Fix low-hanging fruits
6. Perform a final check using the tools
