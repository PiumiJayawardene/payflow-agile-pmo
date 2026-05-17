# Sprint Review
## PayFlow Open Banking — Sprint 1

| Field | Detail |
|-------|--------|
| Date | Friday, Week 4 — 3:00 PM |
| Duration | 60 minutes |
| Attendees | Maria Santos, James Okafor, Priya Sharma, Sam Clarke, Development Team |
| Facilitator | Piumi Jayawardene |

---

## Sprint Goal Assessment

**Sprint Goal:**  
A PayFlow client can authenticate with their UK bank through OAuth 2.0 and establish a verified bank connection securely in under 90 seconds.

**Goal Achieved:** Yes

The demo showed the end-to-end OAuth flow using a sandbox bank account. The client selected a bank, completed authentication, returned to PayFlow, and saw the account marked as connected.

---

## Live Demo Summary

| # | Demo Item | Outcome | Product Owner Response |
|---|-----------|---------|------------------------|
| 1 | OAuth 2.0 redirect from PayFlow to bank login | Successful | Accepted |
| 2 | Secure redirect back to PayFlow after authentication | Successful | Accepted |
| 3 | Connected bank account display | Successful | Accepted |
| 4 | 2FA challenge before payment action | Successful | Accepted |
| 5 | Bank connection error handling | Successful | Accepted |
| 6 | Mobile responsiveness for bank connection screen | Partial | Improvement required |

---

## Story Completion

| Story | Points | Status | Notes |
|-------|--------|--------|-------|
| POB-01 OAuth Bank Authentication | 8 | Done | Accepted by Product Owner |
| POB-02 Two-Factor Authentication on Payments | 5 | Done | Accepted by Product Owner |
| POB-03 Connect Bank Account | 13 | Partial | Desktop completed; mobile responsive improvement carried forward |
| POB-TECH-01 TrueLayer API sandbox setup | 8 | Done | Sandbox integration completed |
| POB-TECH-02 Database schema for bank connections | 3 | Done | Schema created and tested |
| POB-TECH-03 Error handling framework | 5 | Done | API timeout and error states handled |
| **Committed** | **42 pts** | | |
| **Completed** | **39 pts** | | |

---

## Sprint Metrics

| Metric | Value |
|--------|-------|
| Stories committed | 6 |
| Stories fully completed | 5 |
| Stories partially completed | 1 |
| Points committed | 42 |
| Points completed | 39 |
| Velocity | 39 pts |
| P1 defects | 0 |
| P2 defects | 0 |
| P3 defects | 1 |
| Defects open at sprint end | 0 |

---

## Stakeholder Feedback

| Stakeholder | Feedback | Action |
|-------------|----------|--------|
| Maria Santos | OAuth flow looks professional and close to client-ready | Continue with payment initiation in Sprint 2 |
| James Okafor | Mobile view must be improved before pilot testing | Add mobile responsive improvement to Sprint 2 |
| Priya Sharma | API integration is stable in sandbox | Prepare production credential checklist |
| Sam Clarke | QA needs earlier access to mobile acceptance criteria | Add device scope to future UI stories |

---

## Backlog Changes After Review

| Item | Change |
|------|--------|
| POB-03b | Added mobile responsive improvement for bank connection screen |
| POB-10 | Added optional Disconnect Bank Account feature |
| Acceptance Criteria | Device scope to be added for remaining UI stories |

---

## Sprint Review Conclusion

Sprint 1 successfully delivered the core authentication and bank connection foundation for the PayFlow Open Banking payments feature. The sprint goal was achieved, with a minor carry-forward item related to mobile responsiveness.

The team is ready to proceed to Sprint 2, focusing on payment initiation, Strong Customer Authentication, audit logging, and bank connection status visibility.