# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly

## Cross-Functional Handoff Checklist
Use this checklist when work moves between roles (e.g., design → development, development → QA, QA → release).

### Design → Development Handoff
- [ ] UX Designer has shared final design specs and annotated assets
- [ ] Interaction patterns and edge cases documented
- [ ] Accessibility requirements clearly noted
- [ ] Developer and UX Designer have walked through the spec together

### Development → QA Handoff
- [ ] Acceptance criteria reviewed and confirmed complete
- [ ] Automated test coverage meets agreed threshold
- [ ] Known limitations or deferred issues documented
- [ ] QA Lead has reviewed test plan and has environment access

### QA → Release Handoff
- [ ] All acceptance criteria validated and signed off by QA Lead
- [ ] Release notes drafted by Technical Writer and reviewed
- [ ] Customer Success / Support Liaison briefed on changes
- [ ] Business Analyst has confirmed solution meets original requirements
- [ ] PM has confirmed all go/no-go criteria are met
