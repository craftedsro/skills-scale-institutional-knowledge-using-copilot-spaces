# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

For a comprehensive guide on risk management, including detailed scoring, categories, and best practices, see the [Risk Management Template](templates/risk-management-template.md).

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

**Quick Risk Assessment:**
- **Impact:** High (project failure/major delays) | Medium (moderate delays) | Low (minor impact)
- **Likelihood:** High (>60%) | Medium (30-60%) | Low (<30%)
- **Risk Score:** Impact × Likelihood (9=Critical, 6=High, 3-4=Medium, 1-2=Low)

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates

### Weekly Status Update Template
```
**Project:** [Project Name]
**Week of:** [Date]
**Status:** 🟢 On Track | 🟡 At Risk | 🔴 Blocked

**Progress This Week:**
- [Completed item 1]
- [Completed item 2]

**Next Steps:**
- [Planned item 1]
- [Planned item 2]

**Risks & Blockers:**
- [Risk/Blocker 1 - Status and mitigation]
- [Risk/Blocker 2 - Status and mitigation]

**Asks / Decisions Needed:**
- [Decision 1 - Who needs to decide by when]
- [Ask 1 - What help is needed]

**Metrics:**
- [Key metric 1: current value]
- [Key metric 2: current value]
```

### Milestone Update Template
```
**Milestone:** [Name]
**Target Date:** [Date]
**Current Status:** [On Track / At Risk / Delayed]

**Completed:**
- [Achievement 1]
- [Achievement 2]

**In Progress:**
- [Work item 1 - % complete]
- [Work item 2 - % complete]

**Blockers:**
- [Blocker - Impact and resolution plan]

**Next Milestone:** [Name and date]
```

### Incident Communication Template
```
**Incident Status:** [Investigating / Identified / Monitoring / Resolved]
**Severity:** [Critical / High / Medium / Low]
**Started:** [Date/Time]

**Summary:**
[Brief description of the issue and impact]

**Current Actions:**
- [Action being taken 1]
- [Action being taken 2]

**Expected Timeline:**
- [Milestone 1]: [Time]
- [Resolution]: [Time]

**Workaround:** [If available]

**Next Update:** [When stakeholders can expect the next update]

**Follow-up:**
- Post-incident review scheduled for [Date/Time]
```

### Project Handoff Communication Template
```
**Project:** [Name]
**From:** [Current owner]
**To:** [New owner]
**Handoff Date:** [Date]

**Project Status:**
- Current phase: [Phase]
- Health: [Status]

**Key Context:**
- [Important decision 1 and rationale]
- [Important decision 2 and rationale]

**Active Workstreams:**
- [Workstream 1 - Status and next steps]
- [Workstream 2 - Status and next steps]

**Open Risks/Issues:**
- [Risk 1 - Mitigation plan]

**Key Contacts:**
- Product Lead: [Name]
- Tech Lead: [Name]
- Stakeholders: [Names]

**Essential Documents:**
- Project Charter: [Link]
- Project Board: [Link]
- Risk Register: [Link]

**Transition Plan:**
- [Handoff meeting scheduled: Date/Time]
- [Shadow period: Duration]
```

## Escalation Paths

### Standard Escalation Process

**Level 1: Team-Level (0-24 hours)**
- Blockers discussed in daily standup
- Team attempts to resolve internally
- PM informed of blocker status
- *When to escalate:* Issue persists beyond 1 business day OR impacts sprint commitment

**Level 2: PM/Product Lead (24-48 hours)**
- PM escalates to Product Lead and dependent teams
- Cross-functional coordination initiated
- Alternative solutions explored
- Stakeholders notified of potential impact
- *When to escalate:* Issue persists beyond 2 business days OR impacts project timeline/scope

**Level 3: Sponsor/Executive (48+ hours)**
- Business-impacting issues requiring executive decision
- Resource constraints or priority conflicts
- Significant timeline or scope changes needed
- *When to escalate:* Issue threatens project success OR requires budget/resource approval

### Specialized Escalation

**Security Incidents**
- Follow security incident runbook immediately
- Notify Security on-call (no delay)
- Escalate to security@octoacme and CISO within 1 hour
- Document in security incident tracker

**Production Outages**
- Trigger incident response immediately
- Notify on-call engineer and PM
- Follow incident management playbook
- Update status page within 15 minutes

### Escalation Best Practices
- Provide context: what's blocked, impact, what's been tried
- Suggest options when escalating (not just problems)
- Document escalation in project tracker
- Follow up after resolution to prevent recurrence
