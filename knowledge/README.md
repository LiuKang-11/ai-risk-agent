# Wafer Agent Knowledge Sources

This folder contains four knowledge-source packages for a wafer-defect multi-agent system in watsonx Orchestrate.

Packages:
- `wafer_monitoring_policy`: attach to the Wafer Monitor Agent
- `wafer_defect_diagnosis_kb`: attach to the Wafer Diagnosis Agent
- `wafer_compliance_policy`: attach to the Wafer Compliance Agent
- `wafer_response_playbook`: attach to the Wafer Response Planner

Design rules:
- Keep one package attached per agent.
- Reuse the same package across agents only when intentionally sharing policy.
- Keep monitoring, diagnosis, compliance, and response guidance separate so each agent stays within role.
