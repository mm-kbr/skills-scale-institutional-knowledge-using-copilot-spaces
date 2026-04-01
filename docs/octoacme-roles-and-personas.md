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

---

## QA Lead

### Role Summary
The QA Lead owns the quality strategy for a project, ensuring that features are thoroughly tested and meet acceptance criteria before release.

### Responsibilities
- Define and maintain the test plan, test cases, and quality gates
- Coordinate test coverage across unit, integration, and end-to-end layers
- Manage defect triage and escalate critical issues
- Verify release readiness and contribute to the go/no-go decision
- Maintain and improve QA processes and tooling

### Goals
- Prevent regressions and surface defects early in the cycle
- Ensure acceptance criteria are objectively verifiable
- Build confidence in every release through consistent test coverage

### Typical Communication
- Sprint planning and backlog grooming (acceptance criteria review)
- Daily standups to surface blocking defects
- Pre-release sign-off reports and QA summaries

### Interactions / Handoffs
- **Developers**: Collaborates to define acceptance criteria, reviews PR test coverage, and validates fixes before closing defects.
- **Product Managers**: Confirms that acceptance criteria are complete and testable; escalates critical quality risks.
- **Project Managers**: Reports defect status and testing progress; flags release-blocking issues for schedule impact assessment.
- **Release Manager**: Provides formal QA sign-off as a prerequisite for the go/no-go decision; participates in smoke test execution after deployment.

---

## Release Manager

### Role Summary
The Release Manager owns the end-to-end release pipeline, deployment process, and rollback strategy to ensure safe, predictable production releases.

### Responsibilities
- Maintain the release calendar and coordinate deployment windows
- Own the Release Readiness Checklist and drive the go/no-go decision
- Coordinate with teams to ensure all pre-release criteria are met
- Communicate release status and post-release outcomes to stakeholders
- Document and iterate on the rollback / incident playbook

### Goals
- Deliver releases on schedule with minimal production incidents
- Maintain a clear audit trail for every deployment
- Continuously improve deployment speed and reliability

### Typical Communication
- Release planning sessions with PM and engineering leads
- Pre-release readiness reviews with QA Lead and Developers
- Post-release announcements to stakeholders and support

### Interactions / Handoffs
- **Developers**: Aligns on code freeze dates, merge windows, and hotfix criteria.
- **QA Lead**: Receives formal QA sign-off before approving a release; coordinates smoke test execution.
- **Product Managers**: Confirms scope and release notes content; agrees on go/no-go criteria.
- **Project Managers**: Provides release timeline inputs; escalates deployment blockers for stakeholder communication.

---

## UX Designer

### Role Summary
The UX Designer creates user flows, wireframes, and interface prototypes that align product goals with user needs, and ensures design intent is realized through delivery.

### Responsibilities
- Conduct user research and usability testing to inform design decisions
- Produce wireframes, prototypes, and design specifications
- Collaborate on acceptance criteria to include UX quality standards
- Review implemented features for design fidelity before release
- Maintain a shared design system or style guide

### Goals
- Deliver intuitive, accessible user experiences
- Reduce rework by resolving design ambiguity before development begins
- Advocate for the user throughout the project lifecycle

### Typical Communication
- Design reviews and prototype walkthroughs with Product Manager, Project Manager, and Developers
- Usability test readouts for stakeholders
- Inline design annotations and Figma/design-tool comments during development

### Interactions / Handoffs
- **Developers**: Provides specifications and annotated designs; reviews implemented UI for fidelity and accessibility compliance.
- **Product Managers**: Aligns on user personas, journeys, and feature acceptance criteria that include UX quality gates.
- **Project Managers**: Flags design-scope changes and timeline impacts; ensures design tasks are reflected in the project plan.
- **QA Lead**: Defines UX-specific acceptance criteria (e.g., accessibility, responsive layout) to be included in the test plan.

---

## Business Analyst

### Role Summary
The Business Analyst bridges business stakeholders and the delivery team by capturing requirements, translating them into actionable work items, and validating that delivered features solve the intended problem.

### Responsibilities
- Elicit and document business requirements from stakeholders
- Translate requirements into user stories with clear acceptance criteria
- Support backlog grooming and prioritization sessions
- Validate delivered features against original requirements and success metrics
- Identify process improvement opportunities through data analysis

### Goals
- Ensure delivered features address genuine business needs
- Reduce ambiguity and rework caused by unclear requirements
- Maintain a traceable link between business goals and delivery outcomes

### Typical Communication
- Requirements workshops and discovery sessions with stakeholders
- Backlog grooming and sprint planning with Product Manager / Project Manager and Developers
- Post-delivery validation reports and sign-off documentation

### Interactions / Handoffs
- **Developers**: Provides detailed acceptance criteria; answers requirement questions during implementation to avoid blockers.
- **Product Managers**: Collaborates on backlog prioritization and success metric definition; validates stories before sprint commitment.
- **Project Managers**: Surfaces scope change requests and their impact on schedule; helps maintain the project one-pager accuracy.
- **QA Lead**: Reviews acceptance criteria together to ensure all are testable; participates in UAT planning.

---

## Customer Support Liaison

### Role Summary
The Customer Support Liaison brings frontline user perspectives into the product lifecycle, ensuring that support insights inform planning and that product changes are communicated clearly to support teams.

### Responsibilities
- Surface recurring support issues and user pain points to the product team
- Communicate upcoming product changes and releases to the support organization
- Participate in sprint reviews to flag usability or support-complexity concerns
- Collaborate on release notes and user-facing change documentation
- Escalate urgent customer-reported issues to Product Manager and Project Manager for prioritization

### Goals
- Close the feedback loop between users and the delivery team
- Reduce support ticket volume through proactive communication and documentation
- Ensure support teams are prepared for every release

### Typical Communication
- Regular syncs with Product Manager / Project Manager to share support trends and escalations
- Sprint review attendance and feedback sessions
- Release readiness briefings for the support organization

### Interactions / Handoffs
- **Product Managers**: Shares aggregated user feedback and support escalations to influence roadmap prioritization.
- **Project Managers**: Flags customer-impacting issues that may require schedule changes or hotfixes.
- **Release Manager**: Reviews release notes and support documentation before deployment; confirms support team readiness.
- **Developers**: Provides context on customer-reported bugs; validates fixes from a user-experience perspective.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [`docs/octoacme-checklists-and-templates.md`](octoacme-checklists-and-templates.md) for RACI-lite, Definition of Ready/Done, Release Readiness, and Stakeholder Update templates that reference these roles.

