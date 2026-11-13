
.. _chapter-scope:

Scope
=====

Problem
-------

Agents act across services and organizational boundaries. When an act is questioned afterwards, the party asking was
usually not there, and what that party can establish depends on what was recorded at the moment of the act and on the
properties of that record. FG-TIDA/themes#1 cites evaluation work by the UK AI Security Institute in which, where agents
took unsanctioned actions, establishing what had happened "required an investigation rather than a lookup"
(@OlehVasylenko2000, 10 August 2026). That evaluation ran with safeguards disabled, so the point is reconstruction, not
the level of risk. The question is asked afterwards, but the requirement binds when the act happens
(@OlehVasylenko2000, 15 August 2026). No persistent logical-agent identity is assumed.

What the work item covers
-------------------------

Requirements on the record, and on what a relying party reports from it: what an action-time record must be able to
carry about the act (the execution that performed it and, where one exists, its supported relation to a logical agent;
the delegated authority and declared scope; observed content, and a conformance verdict where one exists; a reference
to the provenance of authority); the rejection classes a relying party reports (R1–R4); the properties of carried
claims (R5–R7); absence and silence; lineage from representation to action; and identity continuity and effective
state (R8).

Out of scope
------------

Protocol specification: encodings, schemas, field names, media types, test vectors and expected-outcome files. How a
relying party reaches a class, and how an execution, an identity, a state or a derivation relation is named. Model
internals, and how any value in a record is computed. Replacing logging and audit practice. Legal liability. What a
conformance verdict asserts and how it is checked (FG-TIDA/themes#6, task 3). Where authority originates and what may
be conferred (FG-TIDA/themes#5).
