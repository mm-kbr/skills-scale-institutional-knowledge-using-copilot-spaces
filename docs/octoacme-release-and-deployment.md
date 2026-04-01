# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared
- QA Lead sign-off obtained (see [Release Readiness Checklist](octoacme-checklists-and-templates.md#3-release-readiness-checklist))

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support (Release Manager & Customer Support Liaison)

> The **Release Manager** owns this checklist. For a comprehensive pre-release gate review, use the [Release Readiness Checklist](octoacme-checklists-and-templates.md#3-release-readiness-checklist).
> See [`docs/octoacme-roles-and-personas.md`](octoacme-roles-and-personas.md) for Release Manager and QA Lead responsibilities.

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
