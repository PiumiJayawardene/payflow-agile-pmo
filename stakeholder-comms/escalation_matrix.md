# Escalation Matrix
## PayFlow Open Banking Payments Feature

---

## Purpose

This escalation matrix defines how delivery, scope, technical, compliance, security, and go-live risks should be escalated during the PayFlow Open Banking Payments project.

The goal is to ensure that issues are raised to the correct decision-maker quickly, with clear ownership, response times, and communication channels.

---

## Escalation Levels

| Level | Escalation Type | Trigger | Escalate To | Response Time | Channel |
|-------|-----------------|---------|-------------|---------------|---------|
| Level 1 | Scrum Master Resolution | Minor delivery issue, process issue, team coordination issue, low-impact blocker | Piumi Jayawardene — Scrum Master / PM | Same business day | Slack / Jira comment / 1:1 |
| Level 2 | Product or Technical Decision | Scope conflict, backlog priority issue, acceptance criteria dispute, technical dependency, sprint commitment risk | James Okafor — Product Owner or Priya Sharma — Engineering Lead | Within 4 hours | Slack followed by meeting if needed |
| Level 3 | Sponsor Escalation | Budget impact, go-live date at risk, major resource issue, regulatory delay, unresolved Level 2 issue | Maria Santos — CEO / Sponsor | Within 2 hours | Phone call followed by email summary |
| Level 4 | Emergency Escalation | Critical security vulnerability, data breach, FCA regulatory action, production payment failure | Maria Santos + Aisha Patel + Priya Sharma | Within 30 minutes | Phone call / emergency meeting |

---

## Specific Escalation Triggers

| Situation | Level | Escalation Owner | Required Action |
|-----------|-------|------------------|-----------------|
| Sprint velocity drops below 25 points | Level 2 | Scrum Master | Review sprint scope with Product Owner and agree recovery plan |
| Sprint goal is at risk | Level 2 | Scrum Master | Escalate to Product Owner and Engineering Lead |
| Go-live date may slip by more than 1 week | Level 3 | Scrum Master | Prepare options paper for CEO / Sponsor |
| Budget overrun forecast exceeds 15% | Level 3 | Scrum Master | Escalate to CEO with budget impact and options |
| FCA PSD2 sign-off delayed by more than 2 weeks | Level 3 | Scrum Master + Legal | Escalate to CEO and agree launch options |
| Critical penetration test finding | Level 4 | Scrum Master + Engineering Lead | Pause go-live readiness and start emergency remediation |
| Production payment failure | Level 4 | Engineering Lead | Start incident response and notify CEO immediately |
| TrueLayer API outage exceeds 4 hours | Level 2 | Engineering Lead | Contact vendor support and prepare client communication |
| Team member unavailable for more than 3 working days | Level 2 | Scrum Master | Assess capacity impact and re-plan sprint if needed |
| Product Owner unavailable for sprint review/sign-off | Level 2 | Scrum Master | Escalate decision delay and agree substitute reviewer |
| UAT pilot feedback identifies major usability issue | Level 2 | Product Owner | Prioritise fix or agree launch workaround |
| Open P1 or P2 defect before go-live | Level 3 | QA Engineer + Scrum Master | Escalate to sponsor and block go-live until resolved |

---

## Escalation Contact List

| Name | Role | Escalation Responsibility | Primary Channel | Availability |
|------|------|---------------------------|-----------------|--------------|
| Piumi Jayawardene | Scrum Master / PM | Delivery coordination, risk tracking, reporting, first-level escalation | Slack + Email | Mon–Fri, 08:00–18:00 |
| James Okafor | Product Owner | Product scope, backlog priority, acceptance decisions | Slack + Jira | Mon–Fri, 09:00–17:30 |
| Priya Sharma | Engineering Lead | Technical decisions, architecture, production readiness, technical risks | Slack + Jira | Mon–Fri, 09:00–18:00 |
| Maria Santos | CEO / Sponsor | Budget, go-live, business risk, major escalations | Email + Phone | Business hours, urgent issues anytime |
| Aisha Patel | Legal / Compliance Lead | FCA PSD2, SCA, compliance sign-off, regulatory risk | Email + Review meeting | Mon–Fri, 09:00–17:00 |
| Sam Clarke | QA Engineer | QA sign-off, defect risk, smoke testing, UAT readiness | Jira + Slack | Mon–Fri, 09:00–17:30 |
| TrueLayer Support | API Vendor | API support, sandbox issues, production API incidents | Support portal + Email | As per vendor SLA |
| IT / DevOps | Infrastructure Support | AWS, staging, production environment, deployment support | Jira + Slack | Mon–Fri, on-call during go-live |

---

## Escalation Workflow

1. Issue is identified by delivery team, QA, Product Owner, Legal, or stakeholder.
2. Scrum Master logs or updates the issue in Jira or the risk register.
3. Scrum Master assesses urgency, impact, and escalation level.
4. Issue is escalated to the correct owner based on the matrix above.
5. Decision, action, and owner are documented.
6. Follow-up is tracked in Jira, weekly status report, or risk register.
7. Escalation is closed only after the issue is resolved or formally accepted.

---

## Escalation Communication Format

When escalating, the Scrum Master should include:

- Issue summary
- Business or delivery impact
- Urgency level
- Options available
- Recommended action
- Decision owner
- Deadline for decision
- Current status

---

## Example Escalation

**Issue:** FCA PSD2 compliance sign-off may be delayed beyond Week 12.  
**Level:** Level 3 — Sponsor Escalation  
**Escalated To:** Maria Santos, CEO / Sponsor  
**Impact:** Payment initiation cannot go live without compliance approval.  
**Recommendation:** Continue UAT pilot, but block full payment feature go-live until Legal confirms approval.  
**Decision Needed By:** Week 12 Go / No-Go meeting.  

---

## Governance Notes

- Level 1 issues should be resolved by the Scrum Master without unnecessary stakeholder noise.
- Level 2 issues require Product Owner or Engineering Lead decision-making.
- Level 3 issues must be visible in the weekly status report.
- Level 4 issues require immediate emergency response and formal incident documentation.
- Any unresolved escalation must be reviewed in the next weekly status report.