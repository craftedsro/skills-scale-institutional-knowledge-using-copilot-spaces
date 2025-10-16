# Risk Management Template

## Purpose
This template helps teams systematically identify, assess, track, and mitigate project risks throughout the project lifecycle.

## When to Use
- During project initiation to capture initial risks
- During planning to identify detailed risks and dependencies
- Weekly during execution to review and update risk status
- Before major milestones or releases

## Risk Register

| Risk ID | Risk Description | Category | Impact | Likelihood | Risk Score | Owner | Mitigation Plan | Status | Last Updated |
|---------|-----------------|----------|--------|------------|------------|-------|-----------------|--------|--------------|
| R-001 | [Description] | [Category] | [H/M/L] | [H/M/L] | [Score] | [Name] | [Plan] | [Status] | [Date] |

### Risk Scoring Guide

**Impact Levels:**
- **High (3):** Project failure, major scope/timeline change, or significant customer impact
- **Medium (2):** Moderate delays, scope adjustments, or workarounds needed
- **Low (1):** Minor delays, easily mitigated, minimal impact

**Likelihood Levels:**
- **High (3):** Very likely to occur (>60% probability)
- **Medium (2):** Possible to occur (30-60% probability)
- **Low (1):** Unlikely to occur (<30% probability)

**Risk Score = Impact × Likelihood**
- 9 (Critical): Immediate action required
- 6 (High): Active mitigation needed
- 3-4 (Medium): Monitor and plan mitigation
- 1-2 (Low): Track and review

### Risk Categories

**Technical Risks:**
- Technology limitations or uncertainties
- Technical debt or legacy system constraints
- Integration challenges
- Performance or scalability concerns

**Resource Risks:**
- Team availability or capacity constraints
- Key person dependencies
- Skill gaps or training needs
- Budget limitations

**External Dependencies:**
- Third-party services or APIs
- Cross-team dependencies
- Vendor or partner delays
- Regulatory or compliance requirements

**Scope/Requirements Risks:**
- Unclear or changing requirements
- Stakeholder alignment issues
- Feature complexity underestimated
- Scope creep

**Timeline Risks:**
- Aggressive deadlines
- Holiday or PTO impacts
- Concurrent projects competing for resources
- Estimation uncertainty

## Risk Assessment Workflow

### 1. Identify Risks
**Techniques:**
- Brainstorm with team during kickoff and planning
- Review similar past projects for lessons learned
- Analyze dependencies and integration points
- Consider "what could go wrong?" scenarios
- Review technical architecture and design decisions

**Questions to Ask:**
- What could cause this project to fail?
- What unknowns exist that could impact delivery?
- What external factors are outside our control?
- Where do we lack experience or expertise?
- What assumptions are we making?

### 2. Assess and Score
For each identified risk:
- Describe the risk clearly and specifically
- Assign impact level (consider worst-case scenario)
- Estimate likelihood based on available information
- Calculate risk score
- Categorize the risk

### 3. Plan Mitigation
For each risk, define:

**Mitigation Strategy Types:**
- **Avoid:** Change plans to eliminate the risk
- **Reduce:** Take actions to lower impact or likelihood
- **Transfer:** Assign to another party (vendor, partner)
- **Accept:** Acknowledge and monitor, have contingency plan

**Mitigation Plan Template:**
```
Risk: [Brief description]

Mitigation Actions:
1. [Specific action to reduce likelihood or impact]
2. [Another action]

Contingency Plan (if risk occurs):
1. [What we'll do if the risk materializes]
2. [Backup approach]

Success Criteria:
- [How we'll know mitigation is working]

Timeline: [When actions will be completed]
```

### 4. Monitor and Update
**Weekly Risk Review (5-10 minutes):**
- Review all active risks (score ≥ 3)
- Update status and notes
- Re-assess impact and likelihood if situation changed
- Mark resolved risks as closed
- Identify new risks

**Monthly Deep Dive (30 minutes):**
- Review all risks including low-priority
- Validate mitigation strategies are working
- Update contingency plans
- Share risk trends with stakeholders

## Risk Response Status

| Status | Description | Action Required |
|--------|-------------|-----------------|
| Open | Risk identified, needs mitigation plan | Assign owner, create mitigation plan |
| Mitigating | Active work to reduce risk | Continue mitigation activities, monitor progress |
| Monitoring | Mitigation in place, watching for changes | Regular review, update if situation changes |
| Occurred | Risk materialized, executing contingency | Follow contingency plan, escalate if needed |
| Closed | Risk no longer applicable or fully mitigated | Document lessons learned, archive |

## Example Risk Entry

```
Risk ID: R-003
Risk Description: Integration with third-party payment API may have rate limits that impact our checkout flow during peak traffic
Category: External Dependencies
Impact: High (3) - Could cause failed checkouts and revenue loss
Likelihood: Medium (2) - Vendor documentation unclear on limits
Risk Score: 6 (High priority)
Owner: Tech Lead Sarah Johnson

Mitigation Plan:
1. Contact vendor to clarify rate limits (By: Week 1)
2. Implement request queuing and retry logic (By: Week 2)
3. Add monitoring alerts for API rate limit warnings (By: Week 2)
4. Load test integration with expected peak volume (By: Week 3)

Contingency Plan:
- If rate limits hit during launch: Enable graceful degradation to save orders for async processing
- If limits too restrictive: Escalate to vendor for enterprise tier upgrade

Status: Mitigating
Last Updated: 2024-10-15
Notes: Vendor responded, limits are 1000 req/min. Our peak is estimated at 500 req/min, so adding 2x buffer. Implementation in progress.
```

## Risk Communication

### When to Communicate Risks

**To Project Team:**
- All identified risks during planning
- Weekly status updates on high-priority risks
- Immediately when new critical risk identified

**To Stakeholders:**
- High and critical risks (score ≥ 6) in weekly status updates
- Risk trend summary in monthly reports
- Immediately when risk occurs or escalation needed

**To Leadership:**
- Critical risks threatening project success
- Risks requiring budget or resource decisions
- When escalation path reaches executive level

### Risk Communication Template

```
**Risk Alert**

Risk: [Brief description]
Impact if occurs: [Concrete impact on timeline, scope, or business]
Current likelihood: [With supporting evidence]
Mitigation in progress: [What's being done]
Decision needed: [What stakeholder needs to decide/approve]
Timeline: [When decision or action needed by]
```

## Risk Register Maintenance

**PM Responsibilities:**
- Maintain risk register as single source of truth
- Facilitate weekly risk reviews with team
- Escalate high-priority risks to stakeholders
- Update status and notes after each review
- Archive closed risks with lessons learned

**Team Member Responsibilities:**
- Proactively flag new risks as identified
- Own assigned risks and drive mitigation
- Provide status updates on owned risks
- Suggest contingency approaches

## Integration with Other Processes

**During Planning:**
- Review risk register when estimating work
- Factor mitigation tasks into sprint planning
- Identify risks from dependencies and unknowns

**During Execution:**
- Check risk register before starting high-risk work
- Update status as mitigation progresses
- Execute contingencies when risks occur

**During Retrospectives:**
- Review which risks occurred and why
- Evaluate effectiveness of mitigations
- Capture lessons learned for future projects

## Tips for Effective Risk Management

✅ **Do:**
- Be specific and concrete in risk descriptions
- Focus on actionable mitigation plans
- Review risks regularly as a team activity
- Celebrate when risks are successfully mitigated
- Learn from risks that occur

❌ **Don't:**
- Use vague language like "things might go wrong"
- Create risks for issues that are already problems (those are blockers)
- Let the risk register become stale or outdated
- Punish people for raising risks
- Wait until risks occur to have contingency plans

## Related Resources

- [Risk Management & Communication](../octoacme-risks-and-communication.md) - Overall risk and communication practices
- [Project Planning](../octoacme-project-planning.md) - Where initial risks are identified
- [Execution & Tracking](../octoacme-execution-and-tracking.md) - Day-to-day risk monitoring

---

*This template supports the OctoAcme project management framework and aligns with our principle of data-informed decisions.*
