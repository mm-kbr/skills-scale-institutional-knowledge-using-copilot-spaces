# OctoAcme Project Management Docs

Welcome to the OctoAcme project management documentation hub. This README serves as the central entry point for understanding how OctoAcme teams plan, execute, and deliver work. Whether you are a new contributor getting oriented or a returning team member looking for a specific reference, start here.

## Overview

OctoAcme's project management approach follows a lightweight, consistent lifecycle that helps teams deliver iteratively while keeping ownership and outcomes clear. Work moves through five phases: **Initiation** (confirm the problem, stakeholders, and measurable success criteria), **Planning** (translate the approved initiative into milestones and a prioritized backlog), **Execution** (build, test, and review in small increments), **Release** (deploy with verification and rollback readiness), and **Close & Retrospective** (capture learnings and feed improvements back into the backlog and process). Core artifacts—such as a project charter/one-pager, roadmap and release plan, acceptance criteria with a Definition of Done, a risk register, and retrospective action items—serve as the shared source of truth throughout delivery.

Roles are explicitly defined to reduce ambiguity and improve coordination. A named **Project Manager (PM)** coordinates delivery mechanics including the plan, schedule, risks, and communications, while the **Product Manager (PdM)** owns outcomes such as problem framing, prioritization, and measuring success. **Developers** implement and test features, collaborate on design and estimates, and maintain code quality; **QA/Testing** validates quality and acceptance criteria; and **Stakeholders** provide input, alignment, and approvals at key milestones. This clear division of responsibilities supports predictable execution and makes it easier to onboard new team members into how decisions are made and work is tracked.

Day-to-day execution is organized around a steady team rhythm and visible workflow tracking. Teams use a project board (such as GitHub Projects) with states including **Backlog, Ready, In Progress, In Review, QA, and Done**, supported by daily standups for surfacing blockers and dependencies and a weekly delivery sync for progress reviews, demos, and risk flags. Communication is structured to maintain transparency: PM and PdM align weekly, delivery teams hold standups as agreed, and stakeholders receive regular updates—monthly by default with ad-hoc escalation when needed. Risks and dependencies are actively managed via a risk register and a defined escalation path that starts with team triage and can progress to Product Lead and sponsor-level escalation when business impact requires it.

Quality and release practices emphasize small, verifiable increments and operational safety. Pull requests are kept small when possible, include issue links and acceptance criteria, and require CI checks (tests, lint, and security scanning) to pass before review, with at least one approval required before merge. Testing expectations scale with impact: unit tests for new logic, integration tests where applicable, and end-to-end smoke tests for critical flows before release, plus manual QA when needed for feature acceptance. Releases follow a standardized checklist—ensure acceptance criteria are met, draft release notes, prepare rollback and mitigation plans, deploy to staging with smoke tests, deploy to production via automation where possible, verify post-deploy health, and communicate outcomes to stakeholders and support teams.

---

## Docs Index

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | High-level overview of the OctoAcme project management methodology, principles, and lifecycle |
| [Project Initiation](octoacme-project-initiation.md) | How to kick off a new initiative: problem framing, success criteria, stakeholder alignment |
| [Project Planning](octoacme-project-planning.md) | Translating an approved initiative into milestones, backlog, and a delivery plan |
| [Execution and Tracking](octoacme-execution-and-tracking.md) | Running sprints/iterations, tracking progress, managing blockers, and workflow states |
| [Risks and Communication](octoacme-risks-and-communication.md) | Managing the risk register, communication cadences, and escalation paths |
| [Release and Deployment](octoacme-release-and-deployment.md) | Release checklists, deployment practices, rollback plans, and post-deploy verification |
| [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Running retrospectives, capturing action items, and feeding improvements back into the process |
| [Roles and Personas](octoacme-roles-and-personas.md) | Detailed descriptions of each role: PM, PdM, Developers, QA/Testing, and Stakeholders |

---

> **Maintainer note:** Please keep this index up to date as new documents are added to the `docs/` folder. Each new file should be listed in the table above with a short description so that the index remains a reliable entry point for the team.
