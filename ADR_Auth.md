# {ADR-04: Authentication Selection}

## Context and Problem Statement

The complaint management system needs authentication for consumers and helpdesk agents in the proof of concept scope priortises consistency and workflow over production level authentication
## Considered Options

* Email + password hashing
* Session-based authentication
* Token-based aithentication

## Decision Outcome

Chosen option: Email and password hashing, because it demonstrates secure password storage and role based redirection while keeping proof of concept simple.
### Consequences

* Good, because password hashing demonstrates key security control appropriate for the assignment
* Good, because role based behaviuor can be demonstrated without implementing full user state management
* Bad, because hardcoded user/companyIDs reduce realism and would need to be replaced with sessions
