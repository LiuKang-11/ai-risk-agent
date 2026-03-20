# Escalation Criteria

## Escalate to Wafer Diagnosis Agent when
- monitoring severity is suspicious or critical
- model confidence is moderate or high and supported by context
- recurrence exists by lot, tool, chamber, or process step
- SPC alert and alarm history align with a process or equipment issue
- contamination or mechanical damage is plausible

## Keep in monitor-only mode when
- evidence is weak and isolated
- classifier confidence is low with no supporting signals
- recent history suggests a resolved one-off excursion

## Required summary for escalation
- suspected severity
- supporting evidence
- recurrence scope
- relevant SPC findings
- relevant alarm or lot-history findings
- why diagnosis is needed now
