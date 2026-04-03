# OctoAcme Project Management Docs

> **About this space:** This GitHub Copilot Space serves as the single source of truth for OctoAcme's project management knowledge. All process guides are versioned here so that the whole team — and Copilot — can reference, discuss, and evolve them together.

## Overview

OctoAcme's project management process follows a lightweight, end-to-end lifecycle that emphasizes iterative delivery, clear ownership, and measurable outcomes. Work moves through five phases: **Initiation** (validate the problem, identify stakeholders, define success metrics, and decide go/no-go), **Planning** (break scope into shippable increments, define acceptance criteria and Definition of Done, estimate, and map milestones), **Execution** (deliver in small increments while tracking progress and risks), **Release** (deploy with pre-/post-checks, rollback planning, and release notes), and **Close & Retrospective** (capture learnings and convert them into action items). Consistent artifacts — a project one-pager/charter, a prioritized backlog, a risk register, and retrospective action items — keep work visible and auditable across all phases.

Roles and responsibilities are explicitly defined to reduce ambiguity and improve accountability. A **Project Manager (PM)** coordinates delivery (plans, cadence, risk/dependency management, and stakeholder communications), while a **Product Manager (PdM)** defines outcomes, prioritizes the backlog, and measures success. **Developers** design and implement features, write tests and documentation, and collaborate on estimates and technical risk mitigation. **QA/Testing** validates quality and acceptance criteria. Stakeholders contribute inputs and approvals, with clear escalation paths when delivery is blocked or business impact is at risk.

Communication is structured around a steady team rhythm and predictable reporting. OctoAcme typically runs **daily standups** focused on progress, blockers, and dependencies; a **weekly delivery sync** to review progress and flag risks; and **demos/reviews** at the end of each sprint or milestone. Stakeholder alignment is maintained through regular updates using a "single source of truth" status document and a standard weekly status format (progress, next steps, risks/blockers, asks/decisions). Risks are managed via a risk register and escalated through a defined path (team triage → PM → Product Lead → Sponsor).

Quality assurance is embedded throughout delivery, with expectations that work is testable, reviewable, and releasable in small increments. Execution practices include a project board workflow (Backlog → Ready → In Progress → In Review → QA → Done) and a PR discipline favoring smaller PRs, clear acceptance criteria, CI-based checks (tests, linting, security scanning), and at least one approval before merge. Release management adds additional safeguards — ensuring acceptance criteria are met, CI is green, release notes and rollback plans are prepared, and smoke tests are run in staging and after production deployment — followed by a blameless retrospective if something goes wrong.

## Process Docs

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | High-level overview of OctoAcme's end-to-end project management lifecycle |
| [Project Initiation](octoacme-project-initiation.md) | Stakeholder alignment, problem validation, and go/no-go decision process |
| [Project Planning](octoacme-project-planning.md) | Scope breakdown, backlog creation, estimation, and milestone mapping |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Sprint/iteration execution, board workflow, and progress tracking |
| [Risks & Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, and stakeholder communication cadence |
| [Release & Deployment](octoacme-release-and-deployment.md) | Pre/post-release checklists, rollback planning, and release notes |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Blameless retrospectives, action items, and process improvement cycles |
| [Roles & Personas](octoacme-roles-and-personas.md) | Definitions and responsibilities for each role on an OctoAcme project |

---

*Expand or revise this README as new processes and documents are added.*
