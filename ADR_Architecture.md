# {ADR-01: Architecture Style Selection}

## Context and Problem Statement

The complaint management system proof of concept requires an arhitecture that is simple to implement, easy to demonstrate and consistent. the system must support role based access and a multi tenant data model. 

## Considered Options

* Monolithic web application
* Service oriented
* Serverless functions

## Decision Outcome

Chosen option: Monolithic web architecture, because it is the most suitable for a proof of concept due to reduced deployment complexity, a single codebase and simpler testing and debugging
### Consequences

* Good, because it reduces complexity and speeds up development
* Good, because it is easier to test end to end in proof of concept
* Bad, because scalability is limited compared to other architectures
