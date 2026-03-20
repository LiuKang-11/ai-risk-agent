# Recurrence Policy

## Monitoring scope
Track recurrence by wafer, lot, tool, chamber, recipe, process step, and shift.

## Recurrence rules
- same wafer re-flagged within 24 hours: suspicious
- 2 wafers in same lot with similar pattern in one shift: suspicious
- 3 wafers in same lot with similar pattern in one shift: critical
- 2 lots on same tool with similar pattern in 24 hours: suspicious
- same chamber linked to 3 or more similar cases in 24 hours: critical
- recurrence after maintenance reset or PM: suspicious, critical if spread increases

## Pattern-specific emphasis
- scratch or edge patterns recurring on one handling path: prioritize mechanical investigation
- donut or center patterns recurring by chamber or recipe: prioritize process drift review
- near-full or heavy random recurrence across lots: prioritize contamination review

## Downgrade conditions
- single case only
- no supporting SPC, alarm, or contamination evidence
- known one-off upstream excursion already resolved and documented
