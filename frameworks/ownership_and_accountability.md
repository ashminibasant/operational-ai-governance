# Ownership and Accountability

AI governance gets weak when everyone is involved but no one is clearly accountable.

A technical team may build the system. A product team may decide how it is used. Compliance may review it. Risk may challenge it. Legal may advise on exposure. Operations may deal with the consequences. Leadership may approve the investment.

That does not automatically tell us who owns the outcome.

## The Ownership Question

For every AI use case, I want to be able to answer:

**Who has the authority and responsibility to accept the operational risk created by using this system?**

That person or function does not have to perform every control. They do need to understand the use case, the material risks, the limits of the system, and what happens when the system fails.

## Five Roles I Separate

### 1. Accountable Business Owner

Owns the business outcome and the decision to use the system.

Questions:

* What business result is this system expected to support?
* What harm could result if the system is wrong, unavailable, manipulated, or misunderstood?
* Who accepts the remaining risk after controls are applied?

### 2. Technical Owner

Owns the technical operation, maintenance, configuration, and reliability of the system.

Questions:

* Who understands how the system is configured?
* Who can investigate technical failure?
* Who can change, restrict, or disable technical functionality?

### 3. Control Owner

Owns the execution and evidence of a specific control.

Questions:

* Who performs the control?
* How often is it performed?
* What evidence shows that it happened?
* Who reviews exceptions?

### 4. Decision Authority

Owns the authority to approve, reject, override, or rely on a system supported decision.

Questions:

* Is the AI providing information, recommending an action, or making a decision?
* When is human approval required?
* Who has authority to override the system?

### 5. Escalation Authority

Owns the authority to respond when the system or its controls fall outside expectations.

Questions:

* Who can pause use?
* Who can restrict the scope?
* Who determines whether an incident requires broader review?
* Who decides when normal use can resume?

## Why This Separation Matters

One person may hold more than one role. The important point is that the roles are explicit.

Without that separation, organizations can end up with technical ownership mistaken for business accountability, control performance mistaken for risk acceptance, or human review that exists without actual authority to intervene.

## Minimum Ownership Record

For a governed AI use case, I would expect a basic ownership record to include:

* Use case name
* Business purpose
* Accountable business owner
* Technical owner
* Control owners
* Decision authority
* Escalation authority
* Date of approval
* Known limitations
* Material risks accepted
* Conditions that require review

The objective is simple. If something goes wrong, the organization should not have to figure out ownership after the fact.
