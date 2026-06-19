# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas (proposed additions)

To reduce ambiguity for cross-cutting responsibilities and operational tasks, add the following personas. Each entry includes a brief summary, responsibilities, and how the persona typically interacts with existing roles (PM, PdM, Developers, QA).

### Delivery Lead (cross-functional)
- Role summary: Drives sprint-level execution across multiple teams and ensures commitments and dependencies are managed.
- Responsibilities:
  - Coordinates sprint planning across teams and maintains sprint commitments.
  - Tracks cross-team dependencies and ownerings.
  - Facilitates removal of blockers and escalates when necessary.
  - Maintains sprint-level status and progress artifacts.
- Interactions:
  - Works closely with Project Manager for scheduling and status reporting.
  - Aligns with Product Manager on scope clarifications.
  - Coordinates with Tech Lead/Developers on capacity and impediments.
  - Partners with QA Lead on release readiness.

### Technical Lead / Architect
- Role summary: Owns technical direction for a project area and ensures design decisions meet scalability and maintainability goals.
- Responsibilities:
  - Provide technical guidance and architecture reviews.
  - Make technical tradeoff decisions and document rationale (technical debt vs delivery).
  - Ensure code quality standards and review designs.
  - Identify cross-cutting technical risks and mitigation strategies.
- Interactions:
  - Collaborates with Developers on design and code reviews.
  - Works with PM/PdM on feasibility and estimates.
  - Coordinates with Security Liaison and QA on testability and compliance.

### Release Coordinator / Release Engineer
- Role summary: Manages release pipelines, rollout plans, and rollback/runbooks to ensure smooth deployments.
- Responsibilities:
  - Own release pipelines and staging/prod deployment coordination.
  - Draft and maintain rollback/runbook artifacts and deployment checklists.
  - Coordinate pre-release verifications and post-release monitoring.
  - Liaise with on-call and support teams during releases.
- Interactions:
  - Works with Developers for CI/PR readiness.
  - Coordinates timing and communications with PM.
  - Engages Support/Operations for incident handoffs.
  - Works with Security and Platform teams for approvals.

### QA Lead / Test Architect
- Role summary: Defines the test strategy and ensures adequate automation and manual coverage for acceptance gating.
- Responsibilities:
  - Create test strategies for features and ensure automation coverage targets.
  - Coordinate manual QA efforts and exploratory testing.
  - Maintain acceptance gating criteria and test environments.
- Interactions:
  - Partners with Developers on testability and automation.
  - Aligns with PM/PdM on acceptance criteria.
  - Works with Release Coordinator on pre-release checks.

### UX Researcher / Designer
- Role summary: Owns user research and design decisions that shape acceptance criteria and usability outcomes.
- Responsibilities:
  - Run user research and usability tests; synthesize findings.
  - Produce prototypes and design specs for implementation.
  - Provide design reviews and accessibility considerations.
- Interactions:
  - Works with PdM to translate research into product requirements.
  - Collaborates with Developers on implementation details.
  - Partners with QA on usability testing.

### Security Liaison / Compliance Representative
- Role summary: Ensures designs and releases meet security and compliance requirements and coordinates mitigations.
- Responsibilities:
  - Review designs for security risks and compliance gaps.
  - Coordinate security scans, threat modeling, and remediation.
  - Document residual risk and acceptance criteria.
- Interactions:
  - Collaborates with Tech Lead and Developers for secure implementation.
  - Works with Release Coordinator and PM for schedule impacts.
  - Engages centralized security teams when needed.

### Data Analyst / Measurement Lead
- Role summary: Owns instrumentation, metrics, and validation of success criteria for releases and experiments.
- Responsibilities:
  - Define success metrics and instrumentation needs.
  - Implement and validate telemetry and dashboards.
  - Analyze experiment/feature signals and report results.
- Interactions:
  - Works with PdM to define measurable outcomes.
  - Partners with Developers for instrumentation work.
  - Shares dashboards and reports with PM and stakeholders.

### Support / Operations Liaison
- Role summary: Represents support and operations perspectives to ensure operational readiness and customer supportability.
- Responsibilities:
  - Capture runbook and operational requirements.
  - Coordinate incident readiness and post-release support items.
  - Provide feedback on common support issues and required observability.
- Interactions:
  - Works with Release Coordinator on on-call readiness.
  - Engages Developers and PM for customer-impacting issues.
  - Helps create runbooks and post-incident action items.

### How adding these personas improves outcomes
- Clarifies ownership for cross-cutting concerns (releases, security, measurement, operations).
- Reduces handoff friction by naming owners for common operational tasks.
- Improves onboarding and ramp by providing concrete expectations and examples of responsibilities.
- Speeds decision-making where specialist knowledge is required (security, architecture, release operations).

Suggested next steps (for inclusion in PR or issue comment):
1. Add a new "Additional Personas" section in docs/octoacme-roles-and-personas.md (this section).
2. Add role-to-owner mapping templates and checklists (see companion file below).
3. Circulate the draft to PMs, PdMs, Tech Leads, Security, and Release Engineers for feedback.
4. Iterate and merge the doc update via the project issue/template workflow.
