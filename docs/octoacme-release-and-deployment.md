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

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Pre-Release Review Checklist
Use this checklist to confirm all roles have completed their release responsibilities before go-live.

| Role | Responsibility | Status |
|---|---|---|
| QA Lead / Quality Owner | All acceptance criteria validated; test report approved | ☐ |
| UX Designer | Visual and UX acceptance confirmed against design specs | ☐ |
| Technical Writer | Release notes and user-facing docs published or staged | ☐ |
| Business Analyst | Requirements traceability confirmed; no outstanding scope gaps | ☐ |
| Customer Success / Support Liaison | Support team briefed; FAQs and communication plan ready | ☐ |
| Project Manager | Go/no-go decision recorded; risks resolved or accepted | ☐ |
| Product Manager | Feature acceptance sign-off completed | ☐ |

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
