# OctoAcme Project Management Docs

OctoAcme follows an iterative, customer-first delivery approach with clear ownership (PM + PdM), a lightweight initiation and planning stage, timeboxed execution with CI-backed quality gates, and regular retrospectives to drive continuous improvement. The docs in this folder provide the project lifecycle, workflows, roles, and templates used to run OctoAcme projects.

## Process Documents

- [octoacme-project-management-overview.md](octoacme-project-management-overview.md) — High-level introduction to OctoAcme's project management approach, core roles, and communication cadence.
- [octoacme-project-initiation.md](octoacme-project-initiation.md) — Steps to validate and authorize new work, align stakeholders, and create the Project One-pager.
- [octoacme-project-planning.md](octoacme-project-planning.md) — How to break an approved initiative into an actionable backlog, define dependencies, and create a release plan.
- [octoacme-execution-and-tracking.md](octoacme-execution-and-tracking.md) — Day-to-day execution workflows, PR practices, testing strategy, and team rhythm (standups, syncs, demos).
- [octoacme-risks-and-communication.md](octoacme-risks-and-communication.md) — Risk identification, the Risk Register, stakeholder communication templates, and escalation paths.
- [octoacme-release-and-deployment.md](octoacme-release-and-deployment.md) — Release types, pre-release requirements, deployment checklists, and rollback playbooks.
- [octoacme-retrospective-and-continuous-improvement.md](octoacme-retrospective-and-continuous-improvement.md) — How to run retrospectives, capture learnings, and convert them into actionable improvements.
- [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) — Definitions of core roles (Developers, Product Managers, Project Managers) and their responsibilities.

## OctoAcme Project Management Overview

OctoAcme operates on five core principles: **customer-first delivery**, **iterative value**, **clear ownership**, **data-informed decisions**, and **psychological safety**. Every project follows a consistent lifecycle:

**Initiation & Planning:** New initiatives begin with a lightweight Project One-pager that captures the problem statement, success metrics, stakeholders, and timeline. Work is approved to move to planning only when success metrics are clear, stakeholders align on priority, and team availability is confirmed.

**Execution & Delivery:** Teams run timeboxed iterations using a project board (Backlog → Ready → In Progress → In Review → QA → Done). Pull requests are kept small (target ≤400 lines), include issue links and acceptance criteria, and are backed by automated CI (tests, linting, security scans). At least one approval is required before merging. Daily standups surface blockers and progress; weekly delivery syncs review status and risks; regular demos at sprint or milestone end keep stakeholders informed.

**Quality & Communication:** Quality assurance includes unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows before release, and security scanning in CI. Manual QA validates feature acceptance when needed. Risks are tracked in a simple register reviewed weekly, with a clear escalation path (team → PM → Product Lead → Sponsor). Communication templates ensure consistent status updates and incident response.

**Release & Continuous Improvement:** Deployments are standardized with pre-release checks, smoke tests, deployment checklists, and a rollback/incident playbook. After each sprint, release, or milestone, teams run retrospectives to capture learnings and convert them into actionable improvements—measured and tracked for impact.

**Roles & Responsibilities:** Product Managers define outcomes and prioritize the backlog; Project Managers coordinate schedules, risks, and communications; Developers implement features, tests, and reviews; QA/Testing validates acceptance criteria and runs integration and smoke tests; stakeholders provide input and approvals. Clear ownership and psychological safety enable the team to move fast and learn continuously.
