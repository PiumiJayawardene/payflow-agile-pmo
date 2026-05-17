# Sprint Retrospective
## PayFlow Open Banking — Sprint 2

| Field | Detail |
|-------|--------|
| Date | Friday, Week 6 — 4:00 PM |
| Duration | 60 minutes |
| Facilitator | Piumi Jayawardene |
| Format | 4Ls — Liked, Learned, Lacked, Longed For |
| Attendance | Delivery team only |
| Tool | Team retrospective board |

---

## Liked

### 1. Full payment demo worked successfully

The team successfully demonstrated the core payment journey from connected bank account to PayFlow wallet. This gave stakeholders strong confidence in the project.

### 2. Planned developer leave was handled well

Sprint 2 capacity was reduced in advance, so the planned annual leave did not create delivery disruption.

### 3. Async communication improved focus

The `#dev-questions` channel reduced direct interruptions to the Engineering Lead. Technical questions were grouped and answered more efficiently.

### 4. Compliance involvement was stronger

Legal / Compliance input was included earlier for audit log fields and SCA expectations. This reduced the risk of late rework.

---

## Learned

### 1. Payment polling adds technical complexity

Polling every 5 seconds is useful for client visibility, but it may increase server load under high user volume.

**Learning:** Load testing must be included before go-live.

### 2. SCA needs more test coverage

Strong Customer Authentication is business-critical and regulatory-critical. Testing should include happy path, failed challenge, bypass attempt, expiry, and retry flows.

**Learning:** Security and compliance stories need extra QA time.

### 3. Sandbox behaviour may differ from production

The TrueLayer sandbox is useful for testing, but some production behaviours may differ.

**Learning:** A production-like staging environment and smoke test are needed before launch.

---

## Lacked

### 1. More QA time for SCA

SCA implementation was technically complex, and QA had limited time near the end of the sprint.

**Improvement:** Security-heavy stories should be split or tested earlier.

### 2. Better production-like staging setup

The staging environment did not fully mirror production configuration.

**Improvement:** DevOps should configure production-like staging before Sprint 3 testing.

### 3. More performance visibility

The team did not yet have enough evidence that payment polling would scale.

**Improvement:** Add load testing for 5,000 concurrent users in Sprint 3.

---

## Longed For

### 1. Earlier load testing

The team wanted performance testing to begin earlier, especially for payment polling and payment confirmation timing.

### 2. Clearer go-live readiness checklist

The team wanted one shared checklist covering QA, compliance, UAT, security, performance, and stakeholder sign-off.

### 3. More time for edge-case testing

The team wanted additional testing for failed payment states, expired bank tokens, retry logic, and API timeout scenarios.

---

## Retrospective Action Log

| ID | Action | Owner | Due | Status |
|----|--------|-------|-----|--------|
| R2-01 | Create production smoke test plan for go-live | Sam Clarke | Week 7 Day 1 | Open |
| R2-02 | Prepare load test plan for 5,000 concurrent users | Priya Sharma | Sprint 3 planning | Open |
| R2-03 | Configure production-like staging environment | DevOps | Week 7 Day 3 | Open |
| R2-04 | Create go-live readiness checklist | Scrum Master | Week 7 Day 2 | Open |
| R2-05 | Add edge-case test scenarios for failed payments and expired tokens | QA Engineer | Week 7 Day 4 | Open |

---

## Team Health Check

Scale: 1 to 5, where 5 = excellent.

| Dimension | Sprint 1 | Sprint 2 | Trend |
|-----------|----------|----------|-------|
| Clarity of sprint goal | 4.4 | 4.7 | Improved |
| Team collaboration | 4.6 | 4.8 | Improved |
| Work-life balance | 3.7 | 4.3 | Improved |
| Confidence in delivery | 4.1 | 4.6 | Improved |
| Team morale | 4.0 | 4.5 | Improved |

---

## Scrum Master Notes

Sprint 2 was a strong delivery sprint. The team completed all committed work despite reduced capacity from planned developer leave.

The main focus for Sprint 3 should be quality, launch readiness, performance testing, security testing, UAT pilot preparation, and compliance sign-off. The project remains on track for the Week 13 go-live target.