# Evidence and Auditability

A control is not the same thing as evidence that the control operated.

That distinction matters because organizations often describe a process as governed when they can explain what should happen, but cannot reconstruct what actually happened in a specific case.

## The Evidence Question

For every material control, I want to be able to answer:

**What would we show later to prove this control operated as intended?**

If the answer is unclear, the control may be difficult to test, audit, challenge, or defend.

## Four Evidence Questions

### 1. What happened?

The organization should be able to reconstruct the relevant event or decision.

Useful evidence may include:

* System logs
* Decision records
* Review records
* Approval records
* Exception records
* Version information
* Input and output records where appropriate

### 2. Which control was supposed to operate?

Evidence should connect the event to a defined control rather than exist as disconnected data.

Questions:

* What control applied?
* What risk was the control intended to address?
* Who owned the control?
* When was the control expected to occur?

### 3. Did the control actually operate?

A policy stating that review is required is not evidence that review occurred.

Questions:

* Is there a timestamp?
* Is there a reviewer or system identity?
* Is there a recorded result?
* Is there evidence of any exception or override?
* Can the record be connected to the underlying case?

### 4. Can the organization explain the result later?

Auditability is not only about storing data. It is also about preserving enough context to understand what the data means.

Questions:

* Which version of the system was used?
* Which policy or control standard was in effect?
* What inputs were relevant?
* What human intervention occurred?
* What changed after the event?

## Evidence Quality

I think about governance evidence across five qualities:

1. **Traceable:** The evidence can be connected to the relevant event, control, and owner.
2. **Timely:** The evidence reflects when the control actually occurred.
3. **Complete:** The record contains enough information to understand the event.
4. **Reliable:** The organization has a reason to trust the evidence source.
5. **Retained:** The evidence remains available for the period in which the organization may need to investigate, audit, or defend the decision.

## Evidence Gaps

Common gaps include:

* A required review with no record of who completed it
* A model output with no record of the version that produced it
* An override with no reason captured
* An exception with no documented disposition
* A control dashboard that shows current status but cannot reconstruct historical status
* A policy requirement that is not connected to an operational record

## Minimum Evidence Record

For a material control, I would expect the organization to define:

* Control name
* Risk addressed
* Control owner
* Trigger or frequency
* Evidence produced
* Evidence location
* Reviewer or approver where applicable
* Exception handling process
* Retention expectation
* Testing or validation method

The goal is not to collect evidence for its own sake. The goal is to make governance reconstructable.
