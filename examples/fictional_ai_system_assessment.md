# Fictional AI System Assessment

This example shows how I would assess a fictional AI-enabled business process from an operational governance and product-risk perspective.

The system described below is entirely fictional and is not based on a real employer, client, or product.

## Scenario

A financial-services platform wants to deploy an AI assistant that reviews customer-submitted information, summarizes missing documentation, suggests next steps to service representatives, and drafts customer-facing explanations.

The AI does **not** make final eligibility or credit decisions.

## Intended Purpose

* reduce manual review time
* make missing-document requests more consistent
* help service representatives understand case status
* draft clearer customer communications

## Primary Governance Questions

### 1. What decisions can the system influence?

Even if the model does not make a formal eligibility decision, its summary may influence what the representative notices, what documentation is requested, and what explanation the customer receives.

That means the use case still has meaningful downstream decision risk.

### 2. What should the model never do?

The system should not:

* invent missing facts
* infer protected or sensitive characteristics
* state that a customer is approved or denied
* provide legal conclusions
* override documented eligibility rules
* hide uncertainty when information is incomplete
* take irreversible account action

### 3. What evidence is required?

For material outputs, retain:

* source inputs used by the assistant
* generated summary or draft
* model/version identifier
* reviewer disposition
* edits or overrides when material
* final customer communication
* escalation record when applicable

## Key Risks and Controls

| Risk | Control | Evidence |
|---|---|---|
| Unsupported inference | Prompt/instruction boundary + evaluation testing + human review for exceptions | Evaluation results, override records |
| Hallucinated facts | Source-grounding requirement and factual validation | Source links, reviewer confirmation |
| Unequal treatment | Scenario testing across comparable cases and monitoring for systematic variance | Test set results, monitoring reports |
| Over-reliance by staff | Clear UI labeling and required confirmation before material action | UI design record, confirmation logs |
| Incorrect customer communication | Human approval for material customer-facing output | Approval record, final message |
| Scope creep | Approved-use-case inventory and change review | Use-case record, change approvals |

## Human Oversight Model

### Low Consequence

Routine formatting or summarization with clear source support may proceed with monitoring and sampling.

### Medium Consequence

Requests for additional documentation should require the representative to confirm that the request matches policy and the customer record.

### High Consequence

Any output touching denial, adverse treatment, pricing, legal rights, fraud conclusions, or other material decisions should require human decision-making and approved business rules outside the model.

## Evaluation Plan

Test scenarios should include:

* complete and incomplete files
* contradictory customer information
* ambiguous documentation
* edge cases outside normal policy
* prompts that invite unsupported inference
* attempts to get the model to make a prohibited decision
* cases with similar facts but different irrelevant demographic details
* source documents containing misleading or distracting text

## Metrics

I would monitor:

* factual-support error rate
* unsupported-inference rate
* human override rate
* percentage of escalated cases
* material customer-communication correction rate
* variance across comparable cases
* repeat failure categories
* time saved without increased error rate

## Launch Decision

I would not approve broad deployment based only on average model accuracy.

Launch readiness would depend on whether critical failure modes are controlled, whether high-consequence decisions remain outside unauthorized model authority, whether review evidence is retained, and whether the organization can detect when real-world use begins to differ from the approved design.

## Design Principle

The important governance question is not simply whether the model performs well. It is whether the surrounding system gives the organization enough control, evidence, and accountability to use that performance responsibly.