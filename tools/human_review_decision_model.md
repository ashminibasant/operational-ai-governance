# Human Review Decision Model

A practical framework for deciding when AI output can proceed automatically, when a human should review it, and when the system should stop.

## Core Principle

Human review should be driven by consequence, ambiguity, and accountability — not added everywhere by default and not removed simply because automation is technically possible.

## Decision Factors

Assess each use case across five questions:

1. **Consequence:** What happens if the system is wrong?
2. **Reversibility:** Can the outcome be easily corrected?
3. **Ambiguity:** How much judgment or missing context is involved?
4. **Evidence:** Can the organization reconstruct what happened and why?
5. **Authority:** Is the system allowed to make or influence this decision?

## Decision Matrix

| Consequence | Ambiguity | Reversibility | Recommended Handling |
|---|---|---|---|
| Low | Low | High | Automated processing may be appropriate with monitoring |
| Low | High | High | Human review for uncertain cases |
| Medium | Low | Medium/High | Automation with controls, sampling, and escalation |
| Medium | High | Any | Human review before final action |
| High | Low | Low | Human approval required |
| High | High | Any | Human decision required; AI may assist only |
| Critical | Any | Any | AI should not make the final decision without explicit approved authority and controls |

## Escalation Triggers

Escalate when:

* confidence is below defined threshold
* evidence is missing or contradictory
* output contains unsupported inference
* the request falls outside the approved use case
* customer impact is material
* a policy or legal boundary is unclear
* the system recommends an action it is not authorized to take
* repeated exceptions suggest the operating model is failing

## Example

**Use case:** AI drafts a response to a routine customer inquiry.

If the issue is low consequence, factually supported, and easily reversible, the response may be suitable for automated handling with monitoring.

If the inquiry concerns account eligibility, denial, pricing, health, legal rights, or another material consequence, the same model output should be treated differently. AI may prepare information, but a human should review or make the final decision.

## Evidence to Retain

For governed human review, capture:

* what triggered review
* what the AI recommended
* what evidence was available
* who reviewed it
* what decision the reviewer made
* whether the reviewer overrode the AI
* why the override occurred when material
* what follow-up or escalation was required

## Design Principle

“Human in the loop” is not a control unless the human has enough information, time, authority, and responsibility to change the outcome.