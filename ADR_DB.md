# {ADR-03: Database Management System Selection}

## Context and Problem Statement

The complaint management system requires persistent storage for users, companies, categories and complaints. the database must support relational integrity.

## Considered Options

* MySQL
* PostgreSQL
* MongoDB

## Decision Outcome

Chosen option: MySQL, because it aligns well with the relational structure of the system and supports foreign keys well for the proof of concept
### Consequence

* Good, because relational modelling supports data integrity and clear relationships
* Good, because multi tenancy can be enforced reliably using CompanyID in queries
* Bad, because schema changes require migrations and are less flexible than document based databases for eveloving data models
