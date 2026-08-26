# Escalation and Human Oversight

Human oversight only matters if the human has enough information, enough authority, and a clear reason to intervene.

Putting a person somewhere in the process does not automatically create meaningful oversight.

## The Oversight Question

For every AI supported process, I want to be able to answer:

**When should a person step in, what are they expected to do, and do they actually have the authority to change the outcome?**

## Four Parts of Meaningful Oversight

### 1. Visibility

The reviewer needs enough information to understand what happened.

Questions:

* What did the system produce or recommend?
* What information was used?
* What limitations or warnings are visible?
* What prior actions or exceptions are relevant?

### 2. Decision Authority

The reviewer needs clear authority.

Questions:

* Can the person approve or reject the recommendation?
* Can the person override the system?
* Can the person pause the process?
* Can the person require additional review?

### 3. Trigger

The organization needs to define when human involvement is required.

Possible triggers may include:

* A high impact decision
* Low confidence or inconsistent output
* Missing or conflicting evidence
* A policy exception
* Material drift from expected behavior
* Repeated override activity
* A complaint or adverse outcome
* A control failure
* A new or changed use case

### 4. Escalation Path

The reviewer needs to know what happens next when normal review is not enough.

Questions:

* Who receives the escalation?
* What information must be included?
* How quickly should the issue be addressed?
* Who can restrict or stop use?
* What conditions must be met before normal operation resumes?

## Oversight Levels

Not every use case requires the same level of human involvement.

I think about oversight as a spectrum:

1. **Observe:** A person monitors outcomes but does not approve each action.
2. **Review:** A person reviews selected outputs or exceptions.
3. **Approve:** A person must approve before the action continues.
4. **Override:** A person can replace or reverse the system supported outcome.
5. **Stop:** A person has authority to pause or disable use when risk becomes unacceptable.

The appropriate level depends on the impact of the decision, the reliability of the system, the strength of controls, and the consequences of error.

## Escalation Should Be Defined Before Failure

A weak governance process decides how to respond after something goes wrong.

A stronger process defines escalation conditions in advance.

A basic escalation record should identify:

* Trigger condition
* Initial reviewer
* Escalation owner
* Required evidence
* Required response time
* Available actions
* Decision authority
* Documentation requirement
* Conditions for return to normal use

## The Practical Test

If a reviewer sees something concerning, ask three questions:

1. Do they know it is concerning?
2. Do they know what they are supposed to do?
3. Do they have the authority to do it?

If the answer to any of those is no, the organization may have human involvement without meaningful human oversight.
