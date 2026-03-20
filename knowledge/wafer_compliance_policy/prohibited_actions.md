# Prohibited Autonomous Actions

## Blocked actions
- directly place a production lot on hold in MES
- directly release a held lot
- disable or reconfigure a production tool
- modify recipes, limits, or control parameters
- close compliance cases without human review
- send external customer-facing communications

## Human-review triggers
- critical severity
- low-confidence case with high operational impact
- cross-lot or cross-tool containment recommendation
- policy exception or conflicting evidence

## Default rule
If an action could interrupt production, alter manufacturing state, or create a release decision, require human approval.
