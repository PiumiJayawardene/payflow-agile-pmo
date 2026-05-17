# Weekly Status Report — Week 4 of 13
## PayFlow Open Banking Payments Feature

**Reporting Period:** Week 4  
**Prepared By:** Piumi Jayawardene, Scrum Master / PM  
**Distribution:** Maria Santos, James Okafor, Priya Sharma, Aisha Patel  
**Date:** Friday, Week 4  

---

## 1. Overall RAG Status

| Area | Status | Notes |
|------|--------|-------|
| Overall Project | Green | Sprint 1 completed successfully and project remains on track |
| Scope | Green | Core Sprint 1 scope delivered with one minor mobile improvement carried forward |
| Timeline | Green | Sprint 1 completed on schedule |
| Budget | Green | Spend remains within approved plan |
| Team / Resource | Amber | Work-life balance score requires monitoring |
| Technical Risk | Amber | External API dependency risk reduced but still monitored |
| FCA Compliance | Amber | Initial legal guidance is in progress and needed before later payment release stages |

---

## 2. Executive Summary

Sprint 1 was completed successfully, delivering the core authentication and bank connection foundation for the PayFlow Open Banking Payments feature. The team completed 39 out of 42 committed story points, achieving a strong first sprint velocity. OAuth authentication, two-factor authentication, TrueLayer sandbox setup, database schema, and error handling were completed. One mobile responsiveness improvement was carried forward into Sprint 2, but the project remains on track for the Week 13 go-live target.

---

## 3. Progress This Week

### Completed

- Completed OAuth bank authentication flow
- Completed two-factor authentication for payment actions
- Completed TrueLayer sandbox integration setup
- Completed database schema for bank connections
- Completed API error handling framework
- Completed Sprint 1 review
- Completed Sprint 1 retrospective

### In Progress

- Mobile responsive improvement for bank connection screen
- FCA PSD2 compliance clarification
- Sprint 2 planning preparation
- Payment initiation technical design
- Audit log field confirmation

### Planned Next Week

- Begin Sprint 2
- Complete bank connection mobile responsive improvement
- Build bank connection status dashboard
- Build payment initiation flow
- Implement Strong Customer Authentication controls
- Implement FCA audit logging
- Continue legal and compliance coordination

---

## 4. Key Metrics

| Metric | Target | Actual | Status |
|--------|--------|--------|--------|
| Sprint 1 velocity | ≥ 35 pts | 39 pts | Green |
| Points committed | 42 pts | 42 pts | Green |
| Points completed | 35+ pts | 39 pts | Green |
| Stories fully completed | 5 | 5 | Green |
| Stories partially completed | 1 | 1 | Amber |
| Open P1 defects | 0 | 0 | Green |
| Open P2 defects | 0 | 0 | Green |
| Open P3 defects | 0 | 0 | Green |
| Budget status | Within plan | Within plan | Green |

---

## 5. Risks and Issues

| ID | Risk / Issue | Impact | Action | Owner | Due Date | Status |
|----|--------------|--------|--------|-------|----------|--------|
| R01 | TrueLayer API rate limits may affect future payment performance | Could impact Sprint 2 and Sprint 3 performance validation | Monitor API usage and plan load testing | Priya Sharma | Sprint 3 | Open |
| R02 | FCA PSD2 legal guidance still needs confirmation | Could delay compliance-related acceptance | Continue Legal review and confirm requirements before Sprint 2 completion | Aisha Patel | Week 5 | Open |
| R03 | Backend developer leave planned for Sprint 2 | May reduce Sprint 2 capacity | Reduce Sprint 2 commitment and front-load critical backend work | Piumi Jayawardene | Sprint 2 Planning | Mitigated |
| R04 | Mobile responsiveness was not fully defined in Sprint 1 acceptance criteria | Could affect client usability | Add device scope to remaining UI stories | James Okafor | Week 5 Refinement | Open |

---

## 6. Decisions Made

| ID | Decision | Outcome | Owner |
|----|----------|---------|-------|
| D01 | Carry forward mobile responsive improvement | Added to Sprint 2 as POB-03b | James Okafor |
| D02 | Keep Sprint 2 focused on payment initiation and compliance | Sprint 2 goal confirmed | Piumi Jayawardene + James Okafor |
| D03 | Add device scope to UI acceptance criteria | Required for remaining UI stories | James Okafor |
| D04 | Use async communication channel for technical questions | `#dev-questions` to be created for Sprint 2 | Piumi Jayawardene |

---

## 7. Upcoming Milestones

| Milestone | Target Date | Status | Notes |
|-----------|-------------|--------|-------|
| Sprint 2 Planning | Week 5 | On Track | Sprint goal focused on payment initiation and compliance |
| Payment Initiation Demo | Week 6 | On Track | Expected by Sprint 2 review |
| FCA Audit Log Completion | Week 6 | On Track | Legal input required |
| Sprint 2 Review | Week 6 | On Track | Full payment journey expected |
| Sprint 3 Planning | Week 7 | On Track | Focus will shift to launch readiness |
| Go-live | Week 13 | On Track | No change to target date |

---

## 8. Escalations

| Escalation | Level | Escalated To | Required Action | Status |
|------------|-------|--------------|-----------------|--------|
| FCA PSD2 requirement clarification | Level 2 | Aisha Patel | Confirm compliance expectations before payment initiation release | Open |
| Sprint 2 capacity adjustment | Level 1 | Piumi Jayawardene | Adjust sprint commitment due to planned developer leave | Closed |
| Mobile responsive carry-forward | Level 1 | James Okafor | Prioritise in Sprint 2 backlog | Open |

---

## 9. Confidence Statement

**Confidence in Week 13 Go-Live:** High  

Sprint 1 achieved its main objective and delivered the technical foundation required for Open Banking payments. Velocity is above target, no critical defects remain open, and the only carry-forward item is a manageable mobile improvement. The main risks for the next phase relate to compliance clarification, payment initiation complexity, and Sprint 2 capacity, all of which are being actively managed.