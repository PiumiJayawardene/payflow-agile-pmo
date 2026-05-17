# Sprint 2 Plan
## PayFlow Open Banking — Sprint 2 of 3

| Field | Detail |
|-------|--------|
| Sprint Goal | A PayFlow client can connect their bank, initiate their first payment into their PayFlow wallet, and complete the journey with SCA compliance and audit logging |
| Sprint Number | 2 |
| Start Date | Monday, Week 5 |
| End Date | Friday, Week 6 |
| Sprint Length | 2 weeks |
| Capacity Note | Backend Developer has planned annual leave for 3 days, reducing team capacity |
| Sprint Planning | Monday Week 5 — 10:00 AM to 12:00 PM |
| Sprint Review | Friday Week 6 — 3:00 PM to 4:00 PM |
| Retrospective | Friday Week 6 — 4:00 PM to 5:00 PM |
| Daily Standup | 09:15 AM every day, 15-minute timebox |

---

## Team Capacity

| Team Member | Role | Days Available | Story Points Capacity |
|-------------|------|----------------|----------------------|
| Priya Sharma | Engineering Lead / Backend | 10 | 13 |
| Backend Developer | Backend Developer | 7 | 9 |
| Frontend Developer | Frontend Developer | 10 | 10 |
| Sam Clarke | QA Engineer | 8 | 6 |
| Piumi Jayawardene | Scrum Master / PM | 10 | N/A |
| James Okafor | Product Owner | 3 | N/A |
| **Team Total** | | | **38 pts** |

---

## Sprint 2 Committed Backlog

| Story ID | Title | Points | Owner | Status |
|----------|-------|--------|-------|--------|
| POB-03b | Bank connection mobile responsive improvement | 2 | Frontend Developer | To Do |
| POB-04 | View Bank Connection Status | 3 | Frontend Developer | To Do |
| POB-05 | Initiate a Payment | 13 | Priya + Backend Developer | To Do |
| POB-08 | FCA Audit Log | 8 | Backend Developer | To Do |
| POB-09 | SCA Compliance | 8 | Priya | To Do |
| POB-TECH-04 | Payment status polling | 3 | Backend Developer | To Do |
| **Total Committed** | | **37 pts** | | |

**Sprint Capacity:** 38 pts  
**Committed:** 37 pts  
**Buffer:** 1 pt  

The sprint commitment is slightly below capacity because of planned developer leave and the technical complexity of payment initiation and compliance work.

---

## Dependencies and Pre-Sprint Checklist

| Dependency | Owner | Status | Required By |
|------------|-------|--------|-------------|
| TrueLayer production credential checklist | Priya | Confirmed | Sprint Day 1 |
| Updated mobile acceptance criteria | Product Owner | Completed | Sprint Day 1 |
| FCA PSD2 guidance | Legal / Compliance | Received | Sprint Day 1 |
| Audit log data fields agreed | Legal + Product Owner | Confirmed | Sprint Day 2 |
| SCA test scenarios | QA Engineer | In progress | Sprint Day 3 |

---

## Sprint 2 Focus Areas

### 1. Payment Initiation

The main business value of Sprint 2 is enabling clients to initiate a payment from a connected bank account into their PayFlow wallet.

### 2. Strong Customer Authentication

All payment initiation attempts must require Strong Customer Authentication before the payment is processed.

### 3. FCA Audit Logging

Every payment event must be logged with sufficient detail to support regulatory audit requirements.

### 4. Bank Connection Status

Clients must be able to view whether their bank connection is active, expired, or in error.

---

## Sprint 1 Retrospective Actions Carried into Sprint 2

| Action ID | Action | Status |
|----------|--------|--------|
| R1-01 | Confirm all Sprint 2 dependencies before planning | Done |
| R1-02 | Create `#dev-questions` Slack channel | Done |
| R1-03 | Add device scope to remaining UI stories | Done |
| R1-04 | Review 13-point stories for splitting | Done |
| R1-05 | Hold workload check-ins with delivery team | Done |

---

## Definition of Ready

A story is ready for Sprint 2 when:

- Acceptance criteria are reviewed and approved by the Product Owner
- Compliance-related requirements are confirmed with Legal where needed
- Story points are agreed by the delivery team
- Dependencies are identified and unblocked
- QA has enough detail to prepare test cases
- UI stories include device scope

---

## Definition of Done

A story is done when:

- All acceptance criteria pass in staging
- Code is reviewed and approved
- Unit tests are completed for new logic
- QA signs off the story
- No P1 or P2 defects remain open
- Payment events are logged where relevant
- Product Owner accepts the story in Sprint Review
- Compliance-related stories have Legal input where required

---

## Sprint 2 Daily Standup Log — Sample

### Day 1 — Monday Week 5

**Priya:** Starting payment initiation architecture and SCA flow design. No blockers.  
**Backend Developer:** Reviewing audit log schema and payment status polling requirements. Planned leave starts next week.  
**Frontend Developer:** Starting mobile responsive improvement for bank connection screen.  
**Sam:** Preparing test cases for payment initiation and SCA.  
**Blockers:** None.

---

### Day 4 — Thursday Week 5

**Priya:** Payment initiation API integration is 60% complete. SCA token validation design agreed.  
**Backend Developer:** Audit log schema completed. Started payment status polling implementation.  
**Frontend Developer:** Mobile responsive improvement completed. Starting connection status UI.  
**Sam:** SCA test cases drafted. Audit log test data requirements shared.  
**Blockers:** None.

---

### Day 8 — Wednesday Week 6

**Priya:** Payment initiation working in staging. SCA challenge triggered successfully.  
**Backend Developer:** Returned from leave. Payment polling implementation under final testing.  
**Frontend Developer:** Connection status UI completed and ready for QA.  
**Sam:** Testing payment initiation and audit log export. One minor defect logged for status refresh delay.  
**Blockers:** None.