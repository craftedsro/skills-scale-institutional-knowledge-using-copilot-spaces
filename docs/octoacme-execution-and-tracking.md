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
See detailed escalation process in [Risk Management & Communication](octoacme-risks-and-communication.md#escalation-paths).

**Quick Reference:**
- **Level 1 (0-24h):** Team-level triage in daily standup
- **Level 2 (24-48h):** PM escalates to Product Lead and dependent teams
- **Level 3 (48h+):** Sponsor-level escalation for business-impacting issues

**When to Escalate Immediately:**
- Security vulnerabilities or data breaches
- Production outages affecting customers
- Team member unavailability impacting critical path

## Handoff Procedures

### Within-Team Handoffs
When work moves between team members (e.g., dev → QA, or developer on vacation):
- Update work item status in project board
- Add handoff comment with context: what's done, what's pending, blockers
- @ mention the person taking over
- For longer absences, schedule 15-min handoff sync

### Cross-Team Handoffs
When work depends on another team:
- Document the handoff in project tracker with link to dependent team's ticket
- Share relevant context docs (design, acceptance criteria)
- Identify single point of contact on each team
- Establish expected timeline and follow-up cadence
- Add to dependency tracking in Risk Register

### Project Handoff (PM/Lead Change)
When project ownership transfers:
- Use [Project Handoff Communication Template](octoacme-risks-and-communication.md#project-handoff-communication-template)
- Schedule handoff meeting (60 min minimum)
- Provide access to all project resources
- Shadow period of 1-2 weeks recommended
- Update project documentation with new owner

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Handoff procedures communicated to team
- [ ] Project board columns and workflow agreed upon
