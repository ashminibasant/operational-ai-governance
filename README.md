# Operational AI Governance

Practical frameworks and proof of work for governing AI through ownership, controls, evaluation, evidence, human oversight, escalation, and accountability.

## Why I Built This

A lot of AI governance conversations start with policies, frameworks, or technical safeguards. Those things matter, but they do not answer the full operational question.

Once an AI system is being used inside a real organization, someone still has to own the outcome.

The questions I care about are practical:

* Who is accountable for what the system does?
* What decisions can the system make on its own?
* What requires human review?
* What controls exist before, during, and after use?
* What evidence is created when a control is performed?
* What happens when the system behaves outside expectations?
* Who has the authority to stop, restrict, override, or escalate it?
* What can the organization prove later?

## The Core Model

I treat operational AI governance as a connected system of responsibility rather than a collection of policies.

A governed AI use case should be able to answer eight basic questions:

1. **Purpose:** What is the system being used to do?
2. **Accountable Owner:** Who owns the business outcome and resulting risk?
3. **Decision Authority:** What decisions can the system influence or make?
4. **Controls:** What prevents, detects, or limits unacceptable outcomes?
5. **Evidence:** What proves those controls actually happened?
6. **Human Oversight:** Where can a person review, intervene, override, or stop the process?
7. **Escalation:** What happens when behavior, evidence, or outcomes fall outside expectations?
8. **Claim Boundary:** What can the organization responsibly say the governance process proves?

If one of those pieces is missing, governance may exist on paper without being operationally defensible.

## Frameworks

### [Ownership and Accountability](frameworks/ownership_and_accountability.md)
A structure for separating business ownership, technical responsibility, control ownership, decision authority, and escalation authority.

### [Evidence and Auditability](frameworks/evidence_and_auditability.md)
A practical way to think about the difference between having a control and being able to prove that the control operated.

### [Escalation and Human Oversight](frameworks/escalation_and_human_oversight.md)
A model for defining when human involvement matters, what should trigger escalation, and who has authority to act.

### [Governance Claim Boundaries](frameworks/governance_claim_boundaries.md)
A framework for preventing organizations from claiming more assurance than their actual governance evidence supports.

## Practical Tools

### [AI Evaluation Rubric](tools/ai_evaluation_rubric.md)
A structured review model for factual support, ambiguity, unsupported inference, bias, consistency, instruction following, human-review need, and downstream risk.

### [Human Review Decision Model](tools/human_review_decision_model.md)
A consequence-based framework for deciding when AI can proceed automatically, when a human should review, and when the system should stop.

### [AI Control & Evidence Register](tools/control_evidence_register.md)
A reusable register connecting AI risks to controls, owners, evidence, testing, thresholds, and exception paths.

## Worked Example

### [Fictional AI System Assessment](examples/fictional_ai_system_assessment.md)
A non-confidential assessment of a fictional AI assistant used in a regulated financial-services workflow, showing purpose boundaries, risks, controls, evidence, human oversight, evaluation, and launch criteria.

## How I Think About Governance

My approach starts with the organization, not just the model.

Technical teams may build and operate an AI system, but the organization still owns the operational consequences of using it. Governance therefore has to connect system behavior to business ownership, control performance, evidence, escalation, customer impact, and executive accountability.

The goal is not to make every AI system risk free. The goal is to make decisions, responsibilities, controls, and evidence clear enough that the organization can govern the system deliberately and respond when reality does not match expectations.

## What This Repository Is

This is a public professional proof-of-work portfolio created by **Ashmini Basant**.

It is intended to show how I translate operational risk, business accountability, AI system behavior, and consumer impact into governance structures that technical and business teams can use together.

This repository contains public frameworks, fictional examples, and reusable templates. Organization-specific assessments, implementation design, control testing, and advisory work are separate from the public material presented here.

## Broader Portfolio

My broader proof-of-work portfolio also includes marketing and consumer trust, regulatory response operations, and regulated growth strategy:

[View the full portfolio](https://github.com/ashminibasant/ashminibasant/tree/main/portfolio)

## Important Note

This material is an operational governance framework and professional portfolio. It is not legal advice, certification, or a representation that using these materials alone creates compliance with any law, regulation, or standard.