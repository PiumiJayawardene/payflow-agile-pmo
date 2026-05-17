# Risk Register
## PayFlow Open Banking Payments Feature

**Scoring method:** Likelihood × Impact  
**Scale:** 1 = Low, 5 = High  

| Score | Rating |
|-------|--------|
| 15–25 | Red / High |
| 8–14 | Amber / Medium |
| 1–7 | Green / Low |

---

## Risk Register

| ID | Risk Description | Category | Likelihood | Impact | Score | Rating | Owner | Mitigation | Contingency | Status |
|----|------------------|----------|------------|--------|-------|--------|-------|------------|-------------|--------|
| R01 | TrueLayer API rate limits may throttle payment processing under production load | Technical | 3 | 4 | 12 | Amber | Priya Sharma | Request enterprise rate limit tier and complete load testing before go-live | Temporarily queue payment requests and notify clients of processing delay | Mitigated |
| R02 | FCA PSD2 compliance sign-off may be delayed and block go-live | Regulatory | 2 | 5 | 10 | Amber | Scrum Master + Legal | Engage Legal early and prepare compliance evidence pack during Sprint 2 | Launch bank connection only and delay payment initiation until sign-off | Resolved |
| R03 | Planned backend developer leave in Sprint 2 may reduce delivery capacity | Resource | 5 | 2 | 10 | Amber | Scrum Master | Reduce Sprint 2 capacity and front-load critical backend work | Defer scheduled payments to Phase 2 if velocity drops | Resolved |
| R04 | OAuth token expiry may cause payment failures for returning clients | Technical | 3 | 4 | 12 | Amber | Backend Developer | Build token refresh and reconnection flow into bank connection journey | Prompt user to reconnect and preserve payment history | Resolved |
| R05 | Scheduled payments feature may be underestimated and overflow Sprint 3 | Scope | 3 | 3 | 9 | Amber | Product Owner + Scrum Master | Classify as medium priority and treat as deferrable if launch readiness is at risk | Move scheduled payments to Phase 2 without blocking launch | Not Triggered |
| R06 | Penetration test may identify a critical vulnerability close to go-live | Security | 2 | 5 | 10 | Amber | Scrum Master + IT | Schedule penetration test before final sign-off and keep remediation buffer | Delay go-live and run emergency fix sprint | Resolved |
| R07 | Client pilot group may be too small to provide reliable feedback | Product | 2 | 3 | 6 | Green | Product Owner | Recruit 10 pilot clients across different SME segments | Extend pilot to 20 clients and delay go-live by one week if needed | Resolved |

---

## Risk Heat Map

| Impact / Likelihood | 1 Rare | 2 Unlikely | 3 Possible | 4 Likely | 5 Almost Certain |
|---------------------|--------|------------|------------|----------|------------------|
| 5 Critical | | R02, R06 | | | |
| 4 Major | | | R01, R04 | | |
| 3 Moderate | | R07 | R05 | | |
| 2 Minor | | | | | R03 |
| 1 Negligible | | | | | |

---

## Risk Summary

| Rating | Count | Risk IDs |
|--------|-------|----------|
| Red / High | 0 | None |
| Amber / Medium | 6 | R01, R02, R03, R04, R05, R06 |
| Green / Low | 1 | R07 |

---

## Top Risks Requiring Management Attention

### R01 — TrueLayer API rate limits

This is a technical delivery risk because Open Banking payments depend on API availability and performance. The mitigation is to confirm enterprise rate limits, monitor API performance, and complete load testing before launch.

### R02 — FCA PSD2 compliance sign-off delay

This is a regulatory risk because payment initiation cannot go live without compliance confidence. The mitigation is early Legal involvement and preparing evidence during delivery rather than waiting until the end.

### R06 — Critical penetration test finding

This is a security risk because a critical vulnerability could block go-live. The mitigation is to schedule the penetration test early enough to allow remediation time.

---

## Risk Governance

- Risks are reviewed weekly during the Friday status update.
- Any risk with a score of 15 or above must be escalated to the CEO / Sponsor.
- Any regulatory or security risk must be reviewed with Legal / Compliance.
- Any delivery risk affecting sprint commitment must be discussed with the Product Owner.
- Risk status must be updated after each sprint review.

---

## Risk Review Notes

### Sprint 1

Main risks were external API access, unclear mobile scope, and dependency readiness. No red risks were identified.

### Sprint 2

Compliance and SCA risks were actively managed. Backend developer leave was handled through reduced sprint capacity.

### Sprint 3

Security, performance, and UAT risks were addressed through penetration testing, load testing, smoke testing, and pilot onboarding.

---

## Final Risk Position

At the end of Sprint 3, all major risks were either resolved, mitigated, or not triggered. No red risks remained open before the UAT pilot stage.