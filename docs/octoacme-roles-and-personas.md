# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

For a quick view of how these roles interact across the project lifecycle, see the [Role Interaction Matrix](./octoacme-roles-and-personas-interaction-matrix.md).  
For ownership and handoff guidance, see the [Ownership & Handoffs Checklist](./octoacme-ownership-and-handoffs-checklist.md).

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

### Interactions with Other Roles
- **Product Managers**: Receive feature specs and acceptance criteria; provide effort estimates and flag technical trade-offs.
- **Project Managers**: Report progress and blockers in standups; escalate risks and dependency issues.
- **QA Lead**: Collaborate on test plans, Definition of Done, and bug triage.
- **UX Designer**: Implement UI/UX designs; participate in design reviews and usability feedback sessions.
- **DevOps Engineer**: Coordinate on CI/CD pipeline requirements, deployment scripts, and infrastructure needs.
- **Release Manager**: Confirm feature readiness and provide sign-off for release candidates.

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

### Interactions with Other Roles
- **Project Managers**: Align on scope, timeline, and resource trade-offs; participate in weekly sync and status reviews.
- **Developers**: Provide specs and acceptance criteria; review demos and validate delivered value.
- **UX Designer**: Collaborate on user research findings and design direction; review and approve UX solutions.
- **QA Lead**: Define acceptance criteria and review test coverage; discuss quality trade-offs during planning.
- **Release Manager**: Provide release content and notes; approve go/no-go decisions for major releases.
- **Stakeholder Group**: Gather feedback and communicate roadmap priorities; relay customer insights into backlog decisions.

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

### Interactions with Other Roles
- **Product Managers**: Weekly sync on scope and priorities; escalate timeline or resource conflicts.
- **Developers**: Facilitate sprint ceremonies; remove blockers and track delivery progress.
- **Release Manager**: Coordinate release schedule and deployment windows; update stakeholders on release readiness.
- **QA Lead**: Track quality metrics and test completion gates as part of milestone reviews.
- **DevOps Engineer**: Manage dependencies around infrastructure, environment readiness, and deployment scheduling.
- **Stakeholder Group**: Distribute status updates and escalate issues that affect delivery commitments.

---

## Release Manager

### Role Summary
Release Managers own release planning, scheduling, and cross-functional coordination to ensure successful, low-risk deployments. They act as the central point of contact between engineering, QA, DevOps, and stakeholders during release cycles.

### Responsibilities
- Maintain and communicate the release calendar and deployment windows
- Coordinate go/no-go decisions with all contributing teams
- Verify that pre-release criteria (acceptance tests, security scans, release notes) are met
- Manage rollback plans and ensure they are tested and documented
- Announce releases to stakeholders and support teams
- Track post-release metrics and trigger incident response if needed

### Goals
- Reduce release risk through clear processes and readiness criteria
- Maintain a predictable and transparent release cadence
- Ensure teams are prepared for both planned releases and emergency rollbacks

### Typical Communication
- Release readiness meetings prior to each deployment
- Go/no-go decision emails or Slack messages shared across teams
- Post-release announcements and status summaries

### Interactions with Other Roles
- **Project Managers**: Align on deployment window scheduling and milestone commitments.
- **Product Managers**: Confirm release scope and obtain content for release notes.
- **Developers**: Verify feature completeness and obtain sign-off on code freeze.
- **QA Lead**: Confirm test coverage and receive sign-off on release candidates.
- **DevOps Engineer**: Coordinate pipeline execution, environment readiness, and rollback procedures.
- **Stakeholder Group**: Communicate release timelines, impact, and post-launch status.

---

## QA Lead

### Role Summary
QA Leads own the quality strategy, test planning, and validation of acceptance criteria throughout the project lifecycle. They champion quality gates that protect the team from shipping defects.

### Responsibilities
- Define and maintain the overall test strategy and quality standards
- Create and review test plans, test cases, and acceptance criteria
- Coordinate manual and automated test activities across the team
- Report on test coverage, defect trends, and quality metrics
- Participate in release go/no-go decisions
- Drive improvements in testing tooling, automation, and coverage

### Goals
- Prevent defects from reaching production
- Improve automated test coverage to reduce manual effort over time
- Ensure acceptance criteria are testable and consistently verified

### Typical Communication
- Sprint planning sessions to review and refine acceptance criteria
- Bug triage meetings with Developers and Product Managers
- Quality status updates in weekly delivery syncs

### Interactions with Other Roles
- **Developers**: Collaborate on test plans, review acceptance criteria, assist with debugging and defect resolution.
- **Product Managers**: Clarify acceptance criteria; provide quality metrics to inform prioritization decisions.
- **Project Managers**: Report on quality gate status and testing milestones; flag risks to release timelines.
- **Release Manager**: Provide sign-off on release candidates; communicate remaining open defects and their severity.
- **DevOps Engineer**: Align on CI pipeline test execution, environment configuration, and test data management.
- **UX Designer**: Validate usability and accessibility aspects of delivered features against design specifications.

---

## UX Designer

### Role Summary
UX Designers guide the user experience strategy, interaction design, and visual standards for OctoAcme products. They ensure that features are usable, accessible, and aligned with user needs.

### Responsibilities
- Conduct user research, define personas, and map user journeys
- Create wireframes, prototypes, and high-fidelity design assets
- Maintain design system components and UI standards
- Facilitate usability testing and incorporate feedback
- Review implemented features against design specifications
- Advocate for accessibility and inclusive design practices

### Goals
- Reduce friction and improve end-user satisfaction
- Ensure design consistency across the product
- Deliver clear, tested design assets that reduce rework for Developers

### Typical Communication
- Design review sessions with Product Managers and Developers
- Usability test reports shared with the broader team
- Annotated design files and component library updates

### Interactions with Other Roles
- **Product Managers**: Collaborate on defining user needs, validating research findings, and aligning on UX direction.
- **Developers**: Hand off design specifications, answer implementation questions, and review completed UI work.
- **QA Lead**: Support accessibility and visual regression testing; review design acceptance criteria.
- **Project Managers**: Communicate design timelines and flag dependencies that affect the delivery schedule.
- **Stakeholder Group**: Gather customer feedback to inform design decisions and validate usability improvements.

---

## DevOps Engineer

### Role Summary
DevOps Engineers manage the CI/CD pipelines, infrastructure provisioning, release automation, monitoring, and incident preparedness for OctoAcme. They bridge the gap between development and operations to enable fast, reliable delivery.

### Responsibilities
- Design, build, and maintain CI/CD pipelines and deployment automation
- Provision and manage infrastructure (cloud, containers, networking)
- Set up observability tooling: logging, metrics, alerting, dashboards
- Conduct and document rollback drills and incident response procedures
- Enforce security and compliance controls in deployment pipelines
- Optimize build times and deployment reliability

### Goals
- Enable teams to ship frequently with confidence
- Minimize deployment failures and mean time to recovery (MTTR)
- Maintain secure, auditable, and reproducible infrastructure

### Typical Communication
- Infrastructure change announcements in relevant team channels
- Incident postmortems and runbook updates
- Pipeline status updates during release windows

### Interactions with Other Roles
- **Developers**: Support CI/CD integration, provide feedback on build health, and assist with containerization and environment issues.
- **Release Manager**: Coordinate deployment scheduling, execute releases via automation, and validate rollback procedures.
- **QA Lead**: Configure test environments and maintain test data pipelines; support test automation in CI.
- **Project Managers**: Communicate infrastructure dependencies, scheduled maintenance windows, and environment availability.
- **Product Managers**: Provide observability data (usage metrics, performance) to support product decisions.

---

## Stakeholder Group (Customer Success / Operations)

### Role Summary
Stakeholder Groups represent the business and customer-facing teams (e.g., Customer Success, Operations, Sales, Support) that consume and are affected by delivered features. They provide real-world feedback and help ensure rollouts meet end-user and operational needs.

### Responsibilities
- Communicate customer pain points, feature requests, and rollout concerns
- Review and validate product changes from an operational and customer support perspective
- Participate in UAT (User Acceptance Testing) for high-impact releases
- Advise on change management and communication to end users
- Provide post-launch feedback on adoption and issues

### Typical Communication
- Monthly stakeholder update meetings with Project and Product Managers
- Ad-hoc feedback via designated channels or issue trackers
- UAT sign-off emails or approvals for major releases

### Interactions with Other Roles
- **Product Managers**: Feed customer insights into roadmap planning; receive roadmap updates and priority rationale.
- **Project Managers**: Receive status updates and escalation paths; flag operational concerns that affect delivery scope.
- **Release Manager**: Receive release announcements and advance notice of changes; provide UAT feedback.
- **UX Designer**: Participate in usability studies and provide real-user feedback on designs.
- **QA Lead**: Participate in UAT sessions; report field issues discovered post-launch.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See the [Role Interaction Matrix](./octoacme-roles-and-personas-interaction-matrix.md) for a structured view of cross-role interactions.
- See the [Ownership & Handoffs Checklist](./octoacme-ownership-and-handoffs-checklist.md) for lifecycle gate ownership across roles.

