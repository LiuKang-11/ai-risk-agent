# Monitoring Thresholds

## Decision intent
Use these thresholds to decide whether the case should remain in monitoring, be marked suspicious, or be escalated as critical.

## Severity bands
### Normal
- isolated signal with no confirmed tool, lot, or chamber recurrence
- SPC within control limits and no meaningful drift
- classifier confidence below escalation threshold and no supporting evidence
- no contamination indicators or abnormal alarm history

### Suspicious
- one threshold breach with weak or mixed supporting evidence
- 2 or more similar cases on the same tool within 24 hours
- 2 or more similar cases in the same lot within 12 hours
- SPC warning rule triggered without a hard out-of-control event
- abnormal tool alarms or chamber state changes near event time

### Critical
- contamination trigger condition met
- 3 or more similar cases on the same tool or chamber within 12 hours
- lot-level spread across multiple wafers
- SPC out-of-control event with matching defect recurrence
- edge, scratch, near-full, or mixed severe pattern paired with tool alarms
- any case that suggests broad yield loss, safety risk, or cross-lot propagation

## Confidence thresholds
- low confidence: below 0.60, do not escalate on model output alone
- moderate confidence: 0.60 to 0.84, require at least one corroborating signal
- high confidence: 0.85 and above, may escalate when paired with recurrence, SPC, or alarm evidence

## Immediate escalation conditions
- potential contamination affecting multiple wafers, lots, or chambers
- suspected mechanical damage trend on the same tool path
- repeated chamber anomalies after recent maintenance or reset
- severe metrology deviation paired with defect recurrence
