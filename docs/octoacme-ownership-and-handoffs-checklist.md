# OctoAcme — Ownership & Handoffs Checklist

This checklist maps ownership and key handoff points for each stage of the OctoAcme project lifecycle.  
Use it during planning and release readiness reviews to confirm that each gate has a clear owner and that inputs/outputs are agreed.

For full role definitions see [OctoAcme Personas](./octoacme-roles-and-personas.md).  
For cross-role interaction detail see the [Role Interaction Matrix](./octoacme-roles-and-personas-interaction-matrix.md).

---

## 1. Project Initiation
*Reference: [Project Initiation Guide](./octoacme-project-initiation.md)*

| Gate / Deliverable                        | Owner               | Key Inputs From                         | Handoff To              |
|-------------------------------------------|---------------------|-----------------------------------------|-------------------------|
| Problem statement & business case         | Product Manager     | Stakeholder Group, Project Manager      | Project Manager         |
| Project One-pager completed               | Project Manager     | Product Manager                         | Sponsor / Stakeholder Group |
| Stakeholder list & communication plan     | Project Manager     | Product Manager, Stakeholder Group      | All roles               |
| Initial risk list                         | Project Manager     | Developers, DevOps Engineer             | Project Manager (risk register) |
| Resource needs (team roles, estimates)    | Project Manager     | Developers, QA Lead, DevOps Engineer    | Product Manager         |
| Go / No-go decision for planning          | Product Manager + Project Manager | Sponsor, Stakeholder Group | Planning phase |

### Initiation Ownership Checklist
- [ ] Product Manager has drafted and reviewed the Project One-pager
- [ ] Stakeholder Group has been identified and communication preferences documented
- [ ] UX Designer engaged if the initiative includes user-facing changes
- [ ] QA Lead briefed on scope for early test planning input
- [ ] DevOps Engineer notified if new infrastructure or environments are required

---

## 2. Project Planning
*Reference: [Project Planning](./octoacme-project-planning.md)*

| Gate / Deliverable                        | Owner               | Key Inputs From                         | Handoff To              |
|-------------------------------------------|---------------------|-----------------------------------------|-------------------------|
| Prioritised backlog with AC               | Product Manager     | Developers, QA Lead, UX Designer        | Developers, QA Lead     |
| Definition of Done (DoD)                  | QA Lead + Developers | Product Manager                        | Whole team              |
| Release plan & milestone map              | Release Manager     | Project Manager, Product Manager        | Developers, DevOps Engineer |
| Test plan / QA strategy                   | QA Lead             | Developers, Product Manager             | Release Manager         |
| UX design assets (wireframes/prototypes)  | UX Designer         | Product Manager, Stakeholder Group      | Developers, QA Lead     |
| CI/CD pipeline & environment plan         | DevOps Engineer     | Developers, QA Lead, Release Manager    | Developers, Release Manager |
| Risk register (initial)                   | Project Manager     | Developers, DevOps Engineer, QA Lead    | Whole team              |

### Planning Ownership Checklist
- [ ] Product Manager has prioritised and estimated the backlog before sprint planning
- [ ] QA Lead has reviewed and confirmed all acceptance criteria are testable
- [ ] UX Designer has completed and handed off design assets for planned sprint stories
- [ ] Release Manager has confirmed the release calendar and deployment window
- [ ] DevOps Engineer has confirmed environment availability and pipeline readiness
- [ ] Project Manager has documented dependencies and escalation paths

---

## 3. Execution & Tracking
*Reference: [Execution & Tracking](./octoacme-execution-and-tracking.md)*

| Gate / Deliverable                        | Owner               | Key Inputs From                         | Handoff To              |
|-------------------------------------------|---------------------|-----------------------------------------|-------------------------|
| Feature implementation (per story)        | Developers          | Product Manager (AC), UX Designer (specs) | QA Lead (for testing) |
| Code review & PR approval                 | Developers (peer)   | Developers                              | QA Lead, DevOps Engineer |
| QA test execution & sign-off (per story)  | QA Lead             | Developers                              | Product Manager (demo)  |
| UI review against design specs            | UX Designer         | Developers                              | QA Lead, Product Manager |
| CI pipeline health                        | DevOps Engineer     | Developers                              | Developers, QA Lead     |
| Weekly status update                      | Project Manager     | All roles                               | Stakeholder Group       |
| Risk register update                      | Project Manager     | All roles                               | Product Manager, Stakeholders |

### Execution Ownership Checklist
- [ ] Developers self-assign and link stories to PRs before starting work
- [ ] QA Lead moves completed stories to QA column only after all AC are met and tests pass
- [ ] UX Designer completes UI review before story is marked Done
- [ ] DevOps Engineer monitors CI and notifies team of pipeline failures promptly
- [ ] Project Manager updates risk register at each weekly sync
- [ ] Project Manager sends weekly status update to Stakeholder Group

---

## 4. Risk Management & Communication
*Reference: [Risk Management & Communication](./octoacme-risks-and-communication.md)*

| Gate / Deliverable                        | Owner               | Key Inputs From                         | Handoff To              |
|-------------------------------------------|---------------------|-----------------------------------------|-------------------------|
| Risk identification & assessment          | Project Manager     | All roles                               | Product Manager, Sponsor |
| Mitigation plans                          | Role owning the risk | Project Manager                        | Project Manager (register) |
| Stakeholder communication plan            | Project Manager     | Product Manager, Release Manager        | Stakeholder Group       |
| Incident triage & communication           | Release Manager     | DevOps Engineer, Developers             | Project Manager, Stakeholders |
| Post-incident blameless retrospective     | Project Manager     | DevOps Engineer, Developers, QA Lead    | Whole team              |

### Risk & Communication Ownership Checklist
- [ ] Each risk in the register has a named owner and mitigation plan
- [ ] Release Manager is listed in the escalation path for production incidents
- [ ] Stakeholder Group receives advance notice of any high-impact risks or changes
- [ ] DevOps Engineer has an up-to-date incident runbook
- [ ] Post-incident retrospective is scheduled within 5 business days of resolution

---

## 5. Release & Deployment
*Reference: [Release & Deployment Guide](./octoacme-release-and-deployment.md)*

| Gate / Deliverable                        | Owner               | Key Inputs From                         | Handoff To              |
|-------------------------------------------|---------------------|-----------------------------------------|-------------------------|
| Release candidate sign-off                | QA Lead             | Developers                              | Release Manager         |
| Release notes                             | Product Manager     | Developers, Release Manager             | Stakeholder Group, Support |
| Rollback / mitigation plan                | DevOps Engineer     | Release Manager, Developers             | Release Manager         |
| Deployment execution                      | DevOps Engineer     | Release Manager                         | Release Manager (post-deploy verification) |
| Post-deploy verification                  | QA Lead + DevOps Engineer | Release Manager                  | Release Manager         |
| Release announcement                      | Release Manager     | Product Manager                         | Stakeholder Group, Support |

### Release Ownership Checklist
- [ ] QA Lead has provided written sign-off on the release candidate
- [ ] Release notes reviewed and approved by Product Manager
- [ ] Rollback procedure documented and tested by DevOps Engineer
- [ ] Deployment window confirmed with Project Manager and Stakeholder Group
- [ ] Post-deploy smoke tests completed and results logged by QA Lead / DevOps Engineer
- [ ] Release Manager has sent post-release announcement to Stakeholder Group

---

## 6. Retrospective & Continuous Improvement
*Reference: [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)*

| Gate / Deliverable                        | Owner               | Key Inputs From                         | Handoff To              |
|-------------------------------------------|---------------------|-----------------------------------------|-------------------------|
| Retrospective facilitation                | Project Manager     | All roles                               | All roles               |
| Action items (2–3 top items)              | Project Manager     | All roles                               | Assigned owner per item |
| Metrics review (velocity, quality, MTTR)  | Project Manager + QA Lead + DevOps Engineer | All roles | Product Manager, Stakeholders |
| Process improvement backlog update        | Project Manager     | All roles                               | Product Manager         |
| Follow-up on previous action items        | Project Manager     | Action item owners                      | All roles               |

### Retrospective Ownership Checklist
- [ ] All roles have been invited and attend the retrospective
- [ ] QA Lead presents quality trends (defect rates, coverage changes)
- [ ] DevOps Engineer presents pipeline and deployment health metrics
- [ ] Each action item has a named owner and a due date
- [ ] Action items are added to the backlog or issue tracker within 24 hours of the retro
- [ ] Previous action items reviewed for completion before closing them
