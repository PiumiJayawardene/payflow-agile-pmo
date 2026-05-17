# Project Charter
## PayFlow Open Banking Payments Feature

| Field | Detail |
|-------|--------|
| Project Title | Open Banking Payments Feature — PayFlow Platform v2.0 |
| Project Sponsor | Maria Santos — CEO, PayFlow Ltd |
| Product Owner | James Okafor — Head of Product |
| Scrum Master / PM | Piumi Jayawardene |
| Engineering Lead | Priya Sharma |
| Date Initiated | January 2025 |
| Target Go-Live | End of Q1 2025 (Week 13) |
| Version | 1.0 — Approved |

---

## 1. Business Case

PayFlow Ltd is a B2B SaaS fintech platform used by 400 SME clients for payment reconciliation. Clients currently fund their PayFlow wallets through manual bank transfers, causing a 2–3 day settlement delay.

Competitors are already offering instant funding through Open Banking. This creates a competitive disadvantage for PayFlow and affects customer satisfaction, enterprise sales, and revenue growth.

**The problem in numbers:**
- 2–3 day funding lag compared with competitor instant funding
- 23% of surveyed clients identify funding speed as their top pain point
- Estimated £180,000 ARR opportunity from a new Pro pricing tier
- 3 enterprise prospects blocked from signing due to funding speed concerns

**The solution:**
Implement UK Open Banking payments using the TrueLayer API, allowing clients to push funds from their bank account to their PayFlow wallet in under 60 seconds directly from the PayFlow dashboard.

---

## 2. Objectives

| # | Objective | Target | Measurement |
|---|-----------|--------|-------------|
| OBJ-01 | Payment initiation time | < 60 seconds | System performance test |
| OBJ-02 | Go-live date | End of Week 13 | Milestone tracker |
| OBJ-03 | FCA PSD2 compliance sign-off | Obtained before go-live | Legal confirmation |
| OBJ-04 | Defect rate at launch | < 2 critical defects | QA sign-off report |
| OBJ-05 | Client activation in first 30 days | 50+ clients using feature | Product analytics |
| OBJ-06 | Sprint velocity | ≥ 35 points average | Jira velocity chart |

---

## 3. Scope

### In Scope

- OAuth 2.0 bank authentication via TrueLayer API
- UK bank account connection for supported banks
- Payment initiation from bank account to PayFlow wallet
- Payment history and transaction view
- Strong Customer Authentication for payments
- Audit logging for all payment events
- Internal admin dashboard for payment monitoring
- Load testing for 5,000 concurrent users

### Out of Scope

- International payments
- Mobile app development
- Crypto or DeFi integrations
- White-label reseller capability
- Full accounting system replacement

---

## 4. Delivery Approach

| Parameter | Detail |
|-----------|--------|
| Methodology | Agile Scrum |
| Sprint length | 2 weeks |
| Sprint count | 3 sprints plus discovery phase |
| Team size | 6 members |
| Ceremonies | Daily standup, sprint planning, sprint review, retrospective |
| Definition of Ready | Story has acceptance criteria, estimate, and confirmed dependencies |
| Definition of Done | Acceptance criteria pass, QA sign-off, code reviewed, PO accepted |

---

## 5. Budget

| Category | Budget | Notes |
|----------|--------|-------|
| Development team | £58,500 | 6-person team over 13 weeks |
| TrueLayer API | £3,900 | Enterprise API plan |
| AWS infrastructure | £1,200 | Additional compute and monitoring |
| Security penetration test | £4,000 | External vendor |
| Contingency | £6,760 | 10% contingency |
| **Total** | **£74,360** | |

---

## 6. Initial RAID Log

### Risks
- TrueLayer API rate limits may affect performance under load
- FCA PSD2 compliance sign-off may delay go-live
- Planned developer leave may reduce Sprint 2 capacity

### Assumptions
- TrueLayer API documentation is accurate and available
- Existing PayFlow authentication can be extended
- Legal requirements will remain stable during the delivery window

### Issues
- No open issues at initiation

### Dependencies
- TrueLayer sandbox credentials required before Sprint 1
- AWS environment setup required before development starts
- FCA PSD2 legal guidance required before payment initiation release

---

## 7. Success Criteria

The project will be considered successful when:

1. Payment initiation completes in under 60 seconds.
2. All Sprint 3 user stories are accepted by the Product Owner.
3. FCA compliance sign-off is received before go-live.
4. Zero P1 or P2 defects remain open at launch.
5. At least 50 clients activate the feature within 30 days.
6. Lessons learned are documented in the final retrospective.

---

## 8. Sign-Off

| Role | Name | Decision | Date |
|------|------|----------|------|
| CEO / Sponsor | Maria Santos | Approved | January 2025 |
| Head of Product | James Okafor | Approved | January 2025 |
| Engineering Lead | Priya Sharma | Committed | January 2025 |
| Scrum Master / PM | Piumi Jayawardene | Committed | January 2025 |