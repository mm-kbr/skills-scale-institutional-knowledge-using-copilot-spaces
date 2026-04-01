# OctoAcme — Checklists & Templates

Practical checklists and templates to reduce ambiguity and improve consistency across the OctoAcme project lifecycle.

See [`docs/octoacme-roles-and-personas.md`](octoacme-roles-and-personas.md) for full descriptions of all roles referenced below.

---

## 1. Role Assignment / RACI-Lite Template

Use at project initiation to clarify who is **Responsible**, **Accountable**, **Consulted**, and **Informed** for key activities.

| Activity | Developer | Product Manager | Project Manager | QA Lead | Release Manager | UX Designer | Business Analyst | Customer Support Liaison |
|---|---|---|---|---|---|---|---|---|
| Define problem statement & success metrics | C | A/R | C | I | I | C | R | C |
| Backlog creation & prioritization | C | A/R | C | C | I | C | R | C |
| Design & prototyping | C | C | I | C | I | A/R | C | I |
| Feature implementation | A/R | C | I | C | I | C | I | I |
| Test plan & execution | C | I | I | A/R | C | I | C | I |
| Release readiness / go-no-go | C | C | C | R | A/R | I | I | C |
| Stakeholder communication | I | C | A/R | I | C | I | C | C |
| Post-release support handoff | I | C | I | C | R | I | I | A/R |

**Legend:** R = Responsible, A = Accountable, C = Consulted, I = Informed

> Copy and adjust this table for each project, adding or removing rows to match actual activities.

---

## 2. Definition of Ready / Definition of Done

### Definition of Ready (before a story enters a sprint)
- [ ] User story has a clear title and description
- [ ] Acceptance criteria are written, specific, and testable (reviewed by QA Lead and Business Analyst)
- [ ] UX designs or wireframes are attached or linked (if UI changes are involved)
- [ ] Dependencies on other stories or teams are identified and resolved or tracked
- [ ] Story is estimated (T-shirt size or story points)
- [ ] Story is prioritized in the backlog by the Product Manager

### Definition of Done (before a story is marked complete)
- [ ] All acceptance criteria are met and verified
- [ ] Unit and integration tests written and passing in CI
- [ ] QA Lead has reviewed and approved the implementation
- [ ] UX Designer has confirmed design fidelity (if UI changes are involved)
- [ ] PR reviewed and merged to the target branch
- [ ] No new high-severity defects introduced
- [ ] Documentation updated (if behavior or API changes)
- [ ] Feature flag or rollout configuration set (if applicable)

---

## 3. Release Readiness Checklist

Use before every release in conjunction with [`docs/octoacme-release-and-deployment.md`](octoacme-release-and-deployment.md).

### Code & Quality Gates
- [ ] All stories in scope meet the Definition of Done
- [ ] QA Lead has provided formal sign-off (no open release-blocking defects)
- [ ] CI pipeline is green (tests, lint, security scans)
- [ ] Performance benchmarks reviewed (no regressions)

### Release Artifacts
- [ ] Release notes drafted and reviewed by Product Manager
- [ ] Release Manager has confirmed deployment window and notified stakeholders
- [ ] Customer Support Liaison has briefed the support team on changes

### Deployment Readiness
- [ ] Staging deployment successful; smoke tests passed
- [ ] Rollback plan documented and reviewed by Release Manager
- [ ] Feature flags / configuration changes prepared
- [ ] Database migration scripts tested (if applicable)

### Go / No-Go Decision
- [ ] Release Manager confirms all gates above are met
- [ ] Product Manager approves scope
- [ ] QA Lead confirms quality sign-off
- [ ] Project Manager confirms stakeholder awareness

> If any gate is not met, the Release Manager logs the exception and determines whether to proceed, defer, or escalate.

---

## 4. Stakeholder Update Template

Use for regular status communications as described in [`docs/octoacme-risks-and-communication.md`](octoacme-risks-and-communication.md).

```
Subject: [Project Name] — Status Update YYYY-MM-DD

## Summary
One or two sentences on overall project health (Green / Amber / Red).

## Progress This Period
- [Milestone or feature]: [status / % complete]
- [Milestone or feature]: [status / % complete]

## Next Steps
- [Action item] — Owner: [Role/Name] — Due: [Date]
- [Action item] — Owner: [Role/Name] — Due: [Date]

## Risks & Blockers
| Risk / Blocker | Impact | Owner | Mitigation |
|---|---|---|---|
| [Description] | High/Med/Low | [Role] | [Action] |

## Decisions Needed
- [Decision]: [Context and options] — Needed from: [Stakeholder] — By: [Date]

## Upcoming Milestones
| Milestone | Target Date | Status |
|---|---|---|
| [Name] | [Date] | On track / At risk / Delayed |
```

> Authored by the Project Manager; reviewed with Product Manager before distribution.
> Customer Support Liaison should be included in the distribution list for releases affecting end users.
