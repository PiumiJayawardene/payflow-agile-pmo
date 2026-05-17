# Sprint 3 Plan
## PayFlow Open Banking — Sprint 3 of 3

| Field | Detail |
|-------|--------|
| Sprint Goal | All payment features are complete, performance-tested, FCA-compliant, and ready for client pilot launch |
| Sprint Number | 3 |
| Start Date | Monday, Week 7 |
| End Date | Friday, Week 8 |
| Sprint Length | 2 weeks |
| Sprint Focus | Launch preparation, quality assurance, security, UAT readiness, and final feature completion |
| Sprint Planning | Monday Week 7 — 10:00 AM to 12:00 PM |
| Sprint Review | Friday Week 8 — 3:00 PM to 4:00 PM |
| Retrospective | Friday Week 8 — 4:00 PM to 5:00 PM |
| Daily Standup | 09:15 AM every day, 15-minute timebox |

---

## Sprint Theme

Sprint 3 is the final delivery sprint. The focus is not only on adding the remaining features, but also on proving that the solution is secure, scalable, compliant, and ready for a controlled client pilot.

The sprint follows a **quality over quantity** approach. New feature work is limited so that the team has enough time for load testing, penetration testing, production smoke testing, UAT preparation, and compliance evidence.

---

## Team Capacity

| Team Member | Role | Days Available | Story Points Capacity |
|-------------|------|----------------|----------------------|
| Priya Sharma | Engineering Lead / Backend | 10 | 12 |
| Backend Developer | Backend Developer | 10 | 10 |
| Frontend Developer | Frontend Developer | 10 | 8 |
| Sam Clarke | QA Engineer | 9 | 7 |
| Piumi Jayawardene | Scrum Master / PM | 10 | N/A |
| James Okafor | Product Owner | 4 | N/A |
| **Team Total** | | | **37 pts** |

---

## Sprint 3 Committed Backlog

| Story ID | Title | Points | Owner | Status |
|----------|-------|--------|-------|--------|
| POB-06 | View Payment History | 5 | Frontend Developer | To Do |
| POB-07 | Scheduled Recurring Payments | 8 | Backend Developer | To Do |
| POB-TECH-05 | Load testing for 5,000 concurrent users | 8 | Priya | To Do |
| POB-TECH-06 | Penetration test coordination and remediation | 5 | Scrum Master + IT | To Do |
| POB-TECH-07 | Production smoke test execution | 3 | Sam Clarke | To Do |
| POB-TECH-08 | UAT client pilot onboarding for 10 pilot clients | 5 | Scrum Master + Product Owner | To Do |
| **Total Committed** | | **34 pts** | | |

**Sprint Capacity:** 37 pts  
**Committed:** 34 pts  
**Buffer:** 3 pts  

A 3-point buffer is included because this sprint contains external testing, UAT coordination, security review, and go-live readiness activities.

---

## Sprint 3 Priorities

### 1. Complete remaining client-facing features

Payment history and scheduled payments complete the main client experience for Open Banking wallet funding.

### 2. Prove performance under load

The system must support 5,000 concurrent users and still complete payment initiation within the agreed performance target.

### 3. Validate security

Penetration testing must confirm that no critical vulnerabilities exist before go-live.

### 4. Prepare pilot clients

The team will onboard 10 pilot clients for UAT before full launch.

### 5. Finalise compliance readiness

Audit logs, SCA controls, and evidence packs must be ready for final Legal / Compliance sign-off.

---

## Dependencies and Pre-Sprint Checklist

| Dependency | Owner | Status | Required By |
|------------|-------|--------|-------------|
| Production-like staging environment | DevOps | In progress | Sprint Day 3 |
| Load testing plan | Priya | Drafted | Sprint Day 2 |
| Penetration test vendor booking | Scrum Master | Confirmed | Sprint Day 5 |
| Pilot client shortlist | Product Owner | Drafted | Sprint Day 4 |
| Go-live readiness checklist | Scrum Master | In progress | Sprint Day 2 |
| Compliance evidence requirements | Legal / Compliance | Confirmed | Sprint Day 5 |

---

## Definition of Ready

A Sprint 3 item is ready when:

- Acceptance criteria are approved by the Product Owner
- Testing approach is clear
- Compliance or security impact is understood
- Required environments are available
- External vendor or client dependency is confirmed
- Owner and expected output are agreed

---

## Definition of Done

A Sprint 3 item is done when:

- Acceptance criteria pass
- QA signs off the feature or test activity
- Product Owner accepts the feature or deliverable
- No P1 or P2 defects are open
- Security findings are resolved or formally accepted
- Compliance evidence is documented
- UAT pilot materials are ready
- Go-live readiness checklist is updated

---

## Sprint 3 Daily Standup Log — Sample

### Day 1 — Monday Week 7

**Priya:** Preparing load test scripts and reviewing payment polling performance.  
**Backend Developer:** Starting scheduled recurring payments backend logic.  
**Frontend Developer:** Starting payment history UI and date range filter.  
**Sam:** Drafting production smoke test checklist.  
**Piumi:** Confirming penetration test schedule and pilot client onboarding plan.  
**Blockers:** Production-like staging environment still in progress.

---

### Day 5 — Friday Week 7

**Priya:** Load test scripts ready. Initial test shows payment completion under 60 seconds at moderate load.  
**Backend Developer:** Scheduled payments creation flow complete. Pause and resume logic in progress.  
**Frontend Developer:** Payment history table complete. Export button under testing.  
**Sam:** Smoke test checklist completed. Edge-case testing started.  
**Piumi:** Pen test confirmed for Week 8. Pilot client communication drafted.  
**Blockers:** None.

---

### Day 9 — Thursday Week 8

**Priya:** Load test completed for 5,000 concurrent users. Results are within target.  
**Backend Developer:** Scheduled payments complete and ready for PO review.  
**Frontend Developer:** Payment history completed and accepted by QA.  
**Sam:** Production smoke test passed with 100% checklist completion.  
**Piumi:** Pilot onboarding pack ready. Pen test completed with no critical findings.  
**Blockers:** None.