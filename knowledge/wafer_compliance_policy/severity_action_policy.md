# Severity to Action Policy

## Normal
- allowed: monitor, log, and optionally request more evidence
- restricted: no containment action
- blocked: no hold-related request without new evidence

## Suspicious
- allowed: create case log, notify responsible teams, request metrology review, request engineering attention
- restricted: hold request requires approval path
- blocked: autonomous production interruption

## Critical
- allowed: immediate case log, high-priority notification, expedited review, hold request submission through workflow
- restricted: tool interruption and lot containment must follow approval workflow
- blocked: direct autonomous hold, release, recipe modification, or tool disablement

## Confidence modifier
- low confidence lowers action aggressiveness
- high confidence with corroborating evidence can justify stronger escalation inside policy limits
