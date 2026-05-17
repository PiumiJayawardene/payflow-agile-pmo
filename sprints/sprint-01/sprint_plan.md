# Sprint 1 Plan
## PayFlow Open Banking — Sprint 1 of 3

| Field | Detail |
|-------|--------|
| Sprint Goal | A PayFlow client can authenticate with their UK bank via OAuth 2.0 and establish a verified connection securely in under 90 seconds |
| Sprint Number | 1 |
| Start Date | Monday, Week 3 |
| End Date | Friday, Week 4 |
| Sprint Length | 2 weeks |
| Sprint Planning | Monday Week 3 — 10:00 AM to 12:00 PM |
| Sprint Review | Friday Week 4 — 3:00 PM to 4:00 PM |
| Retrospective | Friday Week 4 — 4:00 PM to 5:00 PM |
| Daily Standup | 09:15 AM every day, 15-minute timebox |

---

## Team Capacity

| Team Member | Role | Days Available | Story Points Capacity |
|-------------|------|----------------|----------------------|
| Priya Sharma | Engineering Lead / Backend | 10 | 13 |
| Backend Developer | Backend Developer | 10 | 13 |
| Frontend Developer | Frontend Developer | 10 | 10 |
| Sam Clarke | QA Engineer | 8 | 8 |
| Piumi Jayawardene | Scrum Master / PM | 10 | N/A |
| James Okafor | Product Owner | 3 | N/A |
| **Team Total** | | | **44 pts** |

---

## Sprint 1 Committed Backlog

| Story ID | Title | Points | Owner | Status |
|----------|-------|--------|-------|--------|
| POB-01 | OAuth Bank Authentication | 8 | Priya + Backend Developer | To Do |
| POB-02 | Two-Factor Authentication on Payments | 5 | Backend Developer | To Do |
| POB-03 | Connect Bank Account | 13 | Frontend Developer + Priya | To Do |
| POB-TECH-01 | TrueLayer API integration sandbox setup | 8 | Priya | To Do |
| POB-TECH-02 | Database schema for bank connections | 3 | Backend Developer | To Do |
| POB-TECH-03 | Error handling framework for API failures | 5 | Frontend Developer | To Do |
| **Total Committed** | | **42 pts** | | |

**Sprint Capacity:** 44 pts  
**Committed:** 42 pts  
**Buffer:** 2 pts  

The buffer is intentional because Sprint 1 includes external API uncertainty and initial technical setup.

---

## Dependencies and Pre-Sprint Checklist

| Dependency | Owner | Status | Required By |
|------------|-------|--------|-------------|
| TrueLayer sandbox API credentials | Priya | Received | Sprint Day 1 |
| AWS environment for OAuth callbacks | DevOps | Configured | Sprint Day 1 |
| FCA PSD2 legal guidance | Legal / Compliance | In progress | Sprint Day 5 |
| UI design mockups for bank connection flow | Product Owner | Approved | Sprint Day 1 |

---

## Definition of Ready

A story is ready for sprint when:

- Acceptance criteria are written and agreed by the Product Owner
- Story is estimated by the delivery team
- Dependencies are identified and unblocked
- Design mockup exists for UI stories
- Technical approach has been discussed in refinement

---

## Definition of Done

A story is done when:

- All acceptance criteria pass in staging
- Code is reviewed by at least one other developer
- Unit test coverage is at least 80% for new code
- QA has tested and signed off the story
- No open P1 or P2 defects are linked to the story
- Feature flag is configured where needed
- Product Owner accepts the story in Sprint Review

---

## Sprint 1 Daily Standup Log — Sample

### Day 1 — Monday Week 3

**Priya:** TrueLayer credentials received. Starting OAuth flow design. No blockers.  
**Backend Developer:** Database schema started. Reviewing TrueLayer token structure. No blockers.  
**Frontend Developer:** UI mockups reviewed with Product Owner. Starting OAuth redirect screens. No blockers.  
**Sam:** Reviewing acceptance criteria for POB-01 and POB-02. Writing test cases.  
**Blockers:** None. FCA legal guidance still outstanding and being monitored.

---

### Day 3 — Wednesday Week 3

**Priya:** OAuth redirect flow 70% complete. Pair programming with backend developer on token encryption.  
**Backend Developer:** Token encryption implemented. Schema migrations running in development environment.  
**Frontend Developer:** OAuth UI complete. Working on bank list selection screen.  
**Sam:** Test cases written for POB-01. Starting POB-02 test cases.  
**Blockers:** None.

---

### Day 7 — Wednesday Week 4

**Priya:** OAuth flow complete. Pull request raised and under review. TrueLayer sandbox tested with Lloyds and Barclays.  
**Backend Developer:** Pull request review completed. Schema complete. Starting error handling work.  
**Frontend Developer:** Bank connection UI 90% complete. Loading and error states remaining.  
**Sam:** POB-01 testing started in staging. One minor mobile display defect logged.  
**Blockers:** None.