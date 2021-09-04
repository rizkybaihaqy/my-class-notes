# Software Architecture

## Software Architecture vs Software Design

### Architecture

Architecture is involved with the higher level of description structures and interactions in a system. It is concerned with those questions that entail decision making about the skeleton of the system.

In other words: __Whole system design__

### Design

Design is all about the organization of parts or components of the system and the subsystems.

The key here is: __Closer to the code or modules__

## Aspect of Software Architecture

- System: Collection of component
- Structure: Set of elements that are grouped together according to a guideline
- Environment: The circumstances in which a software system is built
- Stakeholder: Anyone involved

## An Architecture Is

### Defines a structure

Structures provide insight into architectures, and provide a unique perspective to analyze the architecture with respect to its quality attributes. for example:

- The runtime structures, in terms of the objects created at runtime, and how they interact often determine the deployment architecture
- The module structures, in terms of how the code is broken down and organized into modules and packages for task breakdown

### Picks a core set of elements

Captures only the core set of structural elements required to build the core functionality of the system

For example, an architect describing the  client/server architecture. The system may have other components such as multiple caching proxies in the path from the server to the client, or a remote cache on the server which speeds up web page delivery. However, this is not the focus of the architecture description.

### Captures Early Design Decisions

The first decision freezes the deployment choices of the system to a large extent to a specific OS and system architecture. The next two decisions have a lot of weight in implementing the backend APIs. The last decision freezes the programming language choices for the system.

### Manages Stakeholder Requirements

Balance out these requirements by making trade-offs

### Influences The Organizational Structure

For example, an architecture may have a frontend web app, backend web server, and master DB. It is best to split the team to their functionality.

### Influenced By Its Environment

- Quality attribute requirements
- Standards conformance
- Organizational constraints
- Professional context

### Documents The System

Properly documented architectures can function as an effective documentation for the system.

### Often Conforms To A Pattern

Examples of such patterns are Client-Server, Pipes and Filters, Data-based architectures, and others.

In modern day architectures, the job of the architect comes down to mixing and matching existing sets of such readily
available patterns to solve the problem at hand.

## Importance of Software Architecture

- Architecture Selects Quality Attributes To Be Optimized For A System.
- Architecture facilitates early - Modiprototyping.
- Architecture allows a system to be built component-wise.
- Architecture helps to manage changes to the system.

### Why not build a system without a formal software architecture?

You may be still able to work and build a functional system without a formal architecture, but it would not produce a system which is extensible and modifiable, and would most likely produce a system with a set of quality attributes quite far away from the original requirements

## Architect Roles

- Technical: concerned with the core technology (hardware/software/network) used
- Security: creates or tunes the security strategy
- Information: comes up with architectural solutions to make information available to/from applications
- Infrastructure
- Enterprise:  concerned with how the different elements in an organization and their interplay is tuned towards achieving the goals
- Systems: combines the different systems to create a solution for a specific client.
- Solution: middle man when it comes to strategy vs technology focus and organizational vs project scope.

## Architectural Quality Attributes

- Modifiability
- Testability
- Scalability
- Performance
- Availability
- Security
- Deployability
