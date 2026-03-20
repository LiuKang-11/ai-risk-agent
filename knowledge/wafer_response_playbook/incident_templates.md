# Incident Templates

## Case log template
- title: wafer defect incident for `wafer_id` or `lot_id`
- fields: severity, suspected defect, confidence, affected scope, evidence summary, requested next steps

## Engineering ticket template
- title: suspected `{defect_class}` issue on tool `{tool_id}` at `{process_step}`
- include: recurrence summary, alarms, lot impact, recommended inspection focus

## Notification template
- severity: `{severity}`
- summary: suspected `{defect_class}` on `{tool_id}` affecting `{scope}`
- action needed: `{requested_action}`
- case reference: `{case_id}`

## Lot-hold request template
- lot: `{lot_id}`
- reason: `{containment_reason}`
- supporting evidence: `{evidence_summary}`
- requested approver: `{approval_role}`
