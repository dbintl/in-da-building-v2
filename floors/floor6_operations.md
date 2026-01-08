# Floor 6 — Operations & Execution

Purpose
-------
Enable teams and individual founders to translate plans into reliable, repeatable operations by applying systems thinking, defining workflows, and establishing execution discipline. This floor focuses on operational hygiene: process mapping, role clarity, documentation standards, monitoring of key workflows, and continuous improvement practices that reduce friction and scale reliably. It is about readiness to operate, not implementation of specific infrastructure.

Inputs
------
- Organizational context: team size, roles, operating rhythm (e.g., sprint cadence, on-call), and primary operational goals (uptime, delivery cadence, customer response time).
- Core workflows and processes: descriptions of critical processes (e.g., customer onboarding, product delivery, incident response, billing), existing SOPs, and known pain points.
- Artifacts: current documentation, runbooks, templates, and any performance indicators or historical metrics (optional, user-controlled).
- Constraints and priorities: compliance needs, regulatory windows, staffing limits, and acceptable failure modes.

Outputs
-------
- Process maps and clear workflow definitions for critical paths (owner, inputs, outputs, SLAs).
- Starter runbooks and SOPs for high-priority operations (incident response, release checklist, customer onboarding).
- Documentation standards and a lightweight taxonomy (naming, versioning, access controls) to keep operational artifacts discoverable and actionable.
- Execution playbooks: recommended meeting rhythms, escalation paths, handoffs, and role RACI matrices.
- Measurement plan: suggested KPIs, monitoring signals, and cadence for operational reviews and retrospectives.
- Continuous improvement plan: templates for post-mortems, improvement backlogs, and experiment cycles.
- Metadata and provenance for generated artifacts (assumptions, version, "requires human verification" flag for high-impact SOPs).

How AI assists
--------------
1. Process elicitation: guide structured interviews to capture undocumented workflows and surface edge cases or handoff gaps.
2. Process mapping & visualization seeds: generate clear, human-readable process maps and stepwise checklists that teams can refine into formal diagrams.
3. Runbook & SOP drafts: produce practical, task-oriented runbooks and release/incident checklists tailored to the user’s constraints and risk tolerances, with explicit owner and escalation fields.
4. Role & RACI scaffolding: suggest role responsibilities and RACI matrices to reduce ambiguity in handoffs and decision rights.
5. Measurement and monitoring suggestions: recommend focused KPIs and alert thresholds based on described workflows and risk profiles; produce a simple monitoring playbook (what to monitor, who responds, when to escalate).
6. Documentation hygiene coaching: provide templates and editorial guidance (naming, versioning, changelogs) and audit prompts to prevent drift between runbooks and reality.
7. Continuous improvement facilitation: generate post-mortem templates, blameless-retro prompts, and prioritized improvement backlogs derived from incident narratives or performance gaps.

Validation & safeguards
-----------------------
- Human verification required: all operational checklists that affect customer-facing availability or compliance must be reviewed and approved by designated humans before being operationalized.
- Non-prescriptive guidance: avoid recommending specific tooling or vendor lock-in; provide neutral patterns and criteria for tool selection instead.
- Deterministic, auditable steps: ensure runbooks use deterministic language (who does what, when, and how) and clearly surface assumptions and prerequisites.
- Safety for critical systems: flag any recommendations that could materially alter production behavior (automated rollbacks, mass-notifications) and require staged roll-out and human approvals.
- Data minimization & privacy: do not request sensitive credentials or secrets when eliciting processes; recommend secure secrets and access management practices.
- Change control & versioning: recommend change control gates for high-impact runbook edits (peer review, staging validation, and deployment windows) and keep a versioned audit trail.
- Simulation & testing: encourage tabletop exercises and automated tests where applicable; validate runbooks against scenario matrices (failures, partial outages, recovery).
- Bias & completeness checks: prompt teams to consider diversity of failure modes (both technical and human) and to include runbook steps for common edge cases.

Success metrics
---------------
- Process coverage: percentage of high-priority workflows with owned, versioned runbooks and SOPs.
- Mean time to resolution (MTTR): reduction in median MTTR for incidents covered by floor-generated runbooks.
- Execution reliability: reduction in repeated operational failures for documented processes (recurrence rate).
- Documentation hygiene: proportion of artifacts that meet documentation quality standards (naming, versioning, owner, test status).
- Operational cadence adherence: proportion of teams following recommended meeting rhythms and operational review cadences.
- Improvement velocity: number of closed improvement backlog items per quarter resulting from post-mortems and retrospectives.
- Human review rate for high-impact changes: percentage of high-risk runbook changes that underwent required human sign-off (target: 100%).
