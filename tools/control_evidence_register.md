# AI Control & Evidence Register

A reusable register for connecting AI risks to controls, owners, evidence, testing, and escalation.

## Why This Matters

A control is not useful merely because it exists on paper. A governable AI process should be able to show what the control is, who owns it, when it operates, what evidence proves it operated, and what happens when it fails.

## Register Template

| Field | Description |
|---|---|
| Use Case ID | Unique AI use-case identifier |
| Risk | Failure or harm the control is intended to reduce |
| Control Objective | What must be true after the control operates |
| Control Activity | Specific preventive, detective, or corrective action |
| Control Type | Preventive / Detective / Corrective |
| Frequency | Real time / Per transaction / Daily / Weekly / Release-based / Periodic |
| Owner | Person or function accountable for operation |
| Reviewer | Independent or secondary reviewer if applicable |
| Evidence | Record showing the control operated |
| Evidence Location | Where the record is retained |
| Test Method | How operating effectiveness is checked |
| Threshold | Pass/fail or escalation criteria |
| Exception Path | What happens when the control fails |
| Last Tested | Most recent validation date |
| Status | Effective / Needs Improvement / Failed / Not Tested |

## Example Controls

### Unsupported Inference

**Risk:** Model infers customer facts that were not provided.  
**Control Objective:** Material outputs must be supported by known inputs or explicitly identified as uncertain.  
**Control Activity:** Evaluation checks for unsupported inference; high-consequence cases require human review.  
**Evidence:** Evaluation result, reviewer disposition, exception log.  
**Threshold:** No unsupported inference in approved high-consequence outputs.

### Hallucinated Evidence

**Risk:** Model invents facts, citations, policy language, or sources.  
**Control Objective:** Material factual claims must be traceable to approved evidence.  
**Control Activity:** Source validation before final use.  
**Evidence:** Source links, validation result, retained final output.  
**Threshold:** Zero fabricated sources in final approved outputs.

### Unauthorized Autonomous Action

**Risk:** Agent takes action outside approved authority.  
**Control Objective:** System actions remain within defined permission boundaries.  
**Control Activity:** Role-based permissions, transaction limits, approval gates, and exception alerts.  
**Evidence:** Permission configuration, action logs, approval records, exception alerts.  
**Threshold:** No successful action outside approved scope.

## Testing Questions

When testing a control, ask:

1. Did the control actually operate when required?
2. Is there evidence beyond someone's recollection that it happened?
3. Did the control prevent, detect, or contain the intended failure?
4. Were exceptions identified and escalated?
5. Could the organization reproduce this evidence later?
6. Does the control still match how the system is actually used?

## Design Principle

The best control register is not the longest one. It is the one where every material control can be tied to a real owner, a real operating event, and evidence that survives scrutiny.