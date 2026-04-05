# OctoAcme — Role Interaction Matrix

This matrix summarises the key touchpoints between OctoAcme roles across the project lifecycle.  
Rows represent the **initiating / primary role**; columns represent the **collaborating role**.  
Each cell describes the nature of the interaction. A `—` means no direct regular interaction.

For full role definitions see [OctoAcme Personas](./octoacme-roles-and-personas.md).  
For lifecycle gate ownership see the [Ownership & Handoffs Checklist](./octoacme-ownership-and-handoffs-checklist.md).

---

## Interaction Matrix

|                         | Developers                              | Product Manager                          | Project Manager                          | Release Manager                          | QA Lead                                  | UX Designer                              | DevOps Engineer                          | Stakeholder Group                        |
|-------------------------|-----------------------------------------|------------------------------------------|------------------------------------------|------------------------------------------|------------------------------------------|------------------------------------------|------------------------------------------|------------------------------------------|
| **Developers**          | —                                       | Receive specs & AC; provide estimates    | Report progress; escalate blockers       | Confirm feature readiness; code freeze sign-off | Collaborate on test plans & bug triage   | Implement designs; attend design reviews | Integrate CI/CD; resolve build & env issues | —                                        |
| **Product Manager**     | Provide specs & AC; review demos        | —                                        | Weekly scope/timeline sync               | Approve release scope; supply release notes | Define & review AC; discuss quality trade-offs | Align on UX direction; review research   | Review observability data for decisions  | Gather customer insights; share roadmap  |
| **Project Manager**     | Facilitate ceremonies; remove blockers  | Weekly sync on scope & priorities        | —                                        | Coordinate release schedule & windows    | Track quality gates & test milestones    | Communicate design timeline dependencies | Manage infra dependency & env scheduling | Distribute status updates; escalate risks |
| **Release Manager**     | Verify feature completeness; code freeze | Confirm scope; obtain release notes      | Align deployment windows & milestones    | —                                        | Obtain test sign-off on release candidate | —                                        | Execute pipeline; verify rollback procedures | Announce releases; request UAT          |
| **QA Lead**             | Review AC; assist debug & defect resolution | Clarify AC; provide quality metrics    | Report test milestones & quality risks   | Provide release candidate sign-off       | —                                        | Validate UI against design specs; accessibility | Align on CI test execution & test data  | Facilitate UAT sessions                  |
| **UX Designer**         | Hand off specs; review implemented UI   | Collaborate on user research & UX direction | Flag design dependencies & timeline     | —                                        | Support visual & accessibility test criteria | —                                        | —                                        | Conduct usability studies; gather feedback |
| **DevOps Engineer**     | Support CI/CD; containerisation & env issues | Provide usage & performance data      | Communicate infra dependencies & maintenance windows | Execute deployments; validate rollback   | Configure test environments & data pipelines | —                                        | —                                        | —                                        |
| **Stakeholder Group**   | —                                       | Feed customer insights; receive roadmap updates | Receive status updates; flag operational concerns | Provide UAT feedback; receive release announcements | Participate in UAT; report field issues  | Participate in usability studies         | —                                        | —                                        |

---

## Key Interaction Examples

### Example 1 — Release Readiness
1. **Release Manager** schedules the release window and notifies **Project Manager** and **Product Manager**.
2. **QA Lead** runs final regression suite and provides a pass/fail report to **Release Manager**.
3. **DevOps Engineer** confirms pipeline and rollback procedures are in place.
4. **Release Manager** calls go/no-go with **Product Manager** sign-off.
5. **DevOps Engineer** executes deployment; **Release Manager** announces to **Stakeholder Group**.

### Example 2 — Feature Delivery Cycle
1. **Product Manager** defines acceptance criteria with input from **UX Designer** and **Stakeholder Group**.
2. **Developers** implement the feature and coordinate UI details with **UX Designer**.
3. **QA Lead** validates against acceptance criteria and reports defects to **Developers**.
4. **Project Manager** tracks milestone completion and flags any delays to **Stakeholders**.
5. **Release Manager** gates the feature into the next release after QA sign-off.

### Example 3 — Incident Response
1. **DevOps Engineer** detects a production anomaly via monitoring and triggers the incident channel.
2. **Release Manager** coordinates the response: rollback decision, stakeholder notification.
3. **Developers** diagnose and apply a fix; **QA Lead** verifies the fix in staging.
4. **Project Manager** updates the risk register and schedules a blameless post-mortem.
5. **Product Manager** communicates impact and resolution to **Stakeholder Group**.
