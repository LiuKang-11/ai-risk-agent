# SPC Alert Rules

## Rule usage
The Monitor Agent should use SPC outcomes as escalation evidence, not as a substitute for diagnosis.

## Alert classes
- advisory: trend drift, slow mean shift, or warning limit breach
- alert: repeated warning breaches, zone-rule violations, or sustained drift
- critical: out-of-control point, repeated control limit violations, or fast excursion tied to defect recurrence

## Recommended SPC triggers
- one point beyond control limit: escalate to suspicious, critical if recurrence exists
- 2 of 3 consecutive points beyond warning limit on same side: suspicious
- 4 of 5 consecutive points beyond 1 sigma on same side: suspicious
- 8 consecutive points on one side of centerline: suspicious
- monotonic trend over 6 or more points: advisory or suspicious based on magnitude
- step change after maintenance, recipe change, or chamber clean: suspicious

## Escalation guidance
- SPC signal only: keep at advisory unless case recurrence exists
- SPC plus tool alarms: raise by one level
- SPC plus lot spread across multiple wafers: raise to critical
- SPC plus contamination indicators: raise to critical immediately
