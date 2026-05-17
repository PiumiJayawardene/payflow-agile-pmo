# Sprint Review
## PayFlow Open Banking — Sprint 2

| Field | Detail |
|-------|--------|
| Date | Friday, Week 6 — 3:00 PM |
| Duration | 60 minutes |
| Attendees | Maria Santos, James Okafor, Priya Sharma, Sam Clarke, Development Team |
| Facilitator | Piumi Jayawardene |

---

## Sprint Goal Assessment

**Sprint Goal:**  
A PayFlow client can connect their bank, initiate their first payment into their PayFlow wallet, and complete the journey with SCA compliance and audit logging.

**Goal Achieved:** Yes

The team demonstrated a full payment journey from connected bank account to PayFlow wallet, including payment amount entry, confirmation, Strong Customer Authentication, payment submission, payment status update, and audit logging.

---

## Live Demo Summary

| # | Demo Item | Outcome | Product Owner Response |
|---|-----------|---------|------------------------|
| 1 | Mobile responsive bank connection screen | Successful | Accepted |
| 2 | Bank connection status dashboard | Successful | Accepted |
| 3 | Payment initiation from connected bank account | Successful | Accepted |
| 4 | SCA challenge before payment processing | Successful | Accepted |
| 5 | Payment status polling | Successful | Accepted |
| 6 | FCA audit log entry creation | Successful | Accepted |
| 7 | Audit log export sample | Successful | Accepted |

---

## Story Completion

| Story | Points | Status | Notes |
|-------|--------|--------|-------|
| POB-03b Bank connection mobile responsive improvement | 2 | Done | Sprint 1 carry-forward resolved |
| POB-04 View Bank Connection Status | 3 | Done | Accepted by Product Owner |
| POB-05 Initiate a Payment | 13 | Done | Payment completed in staging |
| POB-08 FCA Audit Log | 8 | Done | Audit fields reviewed with Legal |
| POB-09 SCA Compliance | 8 | Done | SCA challenge working before payment |
| POB-TECH-04 Payment status polling | 3 | Done | Polling configured at 5-second interval |
| **Committed** | **37 pts** | | |
| **Completed** | **37 pts** | | |

---

## Sprint Metrics

| Metric | Value |
|--------|-------|
| Stories committed | 6 |
| Stories completed | 6 |
| Points committed | 37 |
| Points completed | 37 |
| Velocity | 37 pts |
| Sprint 1 velocity | 39 pts |
| Running average velocity | 38 pts |
| P1 defects | 0 |
| P2 defects | 0 |
| P3 defects | 1 |
| Defects open at sprint end | 0 |

---

## Key Demo Outcomes

### Payment initiation

A test client initiated a £500 payment from a Lloyds sandbox bank account to the PayFlow wallet. The payment status updated successfully in staging.

### Strong Customer Authentication

The payment could not be submitted until the SCA challenge was completed. This confirmed the core security requirement for payment processing.

### Audit logging

The audit log captured payment event type, timestamp, user ID, IP address, payment amount, bank used, and outcome.

### Bank connection status

The client dashboard showed Active, Expired, and Error states clearly, with reconnect and retry actions available where appropriate.

---

## Stakeholder Feedback

| Stakeholder | Feedback | Action |
|-------------|----------|--------|
| Maria Santos | The payment flow is strong enough to show to enterprise prospects | Product Owner to schedule controlled client preview |
| James Okafor | Payment history should be prioritised in Sprint 3 | Keep POB-06 as Sprint 3 priority |
| Priya Sharma | Payment polling may create server load under high usage | Add load testing focus in Sprint 3 |
| Sam Clarke | SCA testing needs production-like staging before go-live | Add production smoke test to Sprint 3 |
| Legal / Compliance | Audit log fields meet initial compliance expectations | Prepare final compliance pack before sign-off |

---

## Backlog Changes After Review

| Item | Change |
|------|--------|
| POB-TECH-05 | Added load testing for 5,000 concurrent users |
| POB-TECH-07 | Added production smoke test execution |
| POB-06 | Confirmed as high priority for Sprint 3 |
| Compliance pack | Added as go-live readiness activity |

---

## Sprint Review Conclusion

Sprint 2 successfully delivered the core business value of the PayFlow Open Banking project: clients can initiate payments from a connected bank account with Strong Customer Authentication and audit logging.

The project remains on track for Sprint 3, which will focus on payment history, scheduled payments, load testing, penetration testing, UAT pilot onboarding, and go-live readiness.