# Sprint Retrospective
## PayFlow Open Banking — Sprint 3

| Field | Detail |
|-------|--------|
| Date | Friday, Week 8 — 4:00 PM |
| Duration | 60 minutes |
| Facilitator | Piumi Jayawardene |
| Format | Start / Stop / Continue + Project-Level Retrospective |
| Attendance | Delivery team only |
| Tool | Retrospective board and action log |

---

## Sprint 3 Summary

Sprint 3 focused on launch readiness, quality assurance, security, compliance, and client pilot preparation. The team completed all committed work and finished the sprint with no open P1 or P2 defects.

The project is now ready to move into UAT pilot, compliance sign-off, go-live authorisation, and hypercare.

---

## Start — For Future Projects

### 1. Start load testing earlier

Load testing should begin in Sprint 2 rather than Sprint 3. This gives the team more time to fix performance issues before go-live.

### 2. Start compliance documentation in parallel with development

Compliance evidence should be prepared continuously during delivery, not only near the end of the project.

### 3. Start pilot client recruitment earlier

Client pilot recruitment should begin during Sprint 2. Coordinating real clients takes time, especially when legal, onboarding, and support communication are involved.

### 4. Start go-live checklist tracking from Sprint 1

Go-live readiness should be treated as a live checklist from the beginning of delivery, not only during the final sprint.

---

## Stop — For Future Projects

### 1. Stop assuming staging matches production

The team learned that staging environments may behave differently from production. Production-like staging must be confirmed early.

### 2. Stop estimating security remediation as zero effort

Penetration test findings need planned capacity. Even medium findings can require urgent development and QA effort.

### 3. Stop leaving performance validation until the final sprint

Performance risks should be validated earlier, especially for payment polling and high-volume transaction features.

### 4. Stop treating pilot onboarding as an admin task only

Pilot onboarding requires product, support, compliance, and communication planning. It should be managed as a formal workstream.

---

## Continue

### 1. Continue QA involvement from refinement

QA involvement from the beginning improved acceptance criteria quality and reduced late testing surprises.

### 2. Continue same-day pull request reviews

Fast code reviews helped the team maintain delivery flow and avoid technical bottlenecks.

### 3. Continue async-first communication

The `#dev-questions` channel reduced unnecessary interruptions and helped the Engineering Lead focus on complex work.

### 4. Continue team health checks

Team health checks gave the Scrum Master useful signals about workload, morale, collaboration, and confidence.

### 5. Continue clear sprint goals

Each sprint had a focused goal, which helped stakeholders understand delivery progress clearly.

---

## Final Team Health Check

Scale: 1 to 5, where 5 = excellent.

| Dimension | Sprint 1 | Sprint 2 | Sprint 3 | Trend |
|-----------|----------|----------|----------|-------|
| Clarity of sprint goal | 4.4 | 4.7 | 4.9 | Improved |
| Team collaboration | 4.6 | 4.8 | 4.9 | Improved |
| Work-life balance | 3.7 | 4.3 | 4.6 | Improved |
| Confidence in delivery | 4.1 | 4.6 | 4.9 | Improved |
| Team morale | 4.0 | 4.5 | 4.8 | Improved |

---

## Project-Level Lessons Learned

### 1. External API dependencies must be confirmed early

Open Banking delivery depends heavily on external vendor credentials, documentation, sandbox availability, and production access.

**Lesson:** Confirm all external dependencies before sprint planning.

### 2. Compliance should be embedded into delivery

FCA PSD2, Strong Customer Authentication, audit logging, and security evidence should be included in sprint work, not handled separately at the end.

**Lesson:** Treat compliance as part of Definition of Done for regulated fintech work.

### 3. Large stories carry hidden risk

The 13-point stories required close tracking. Large stories often hide uncertainty in technical design, testing, and edge cases.

**Lesson:** Split stories where possible before sprint commitment.

### 4. Performance testing needs earlier visibility

Payment polling and payment initiation timing are business-critical. Performance issues discovered late could delay go-live.

**Lesson:** Start performance testing before the final sprint.

### 5. Pilot onboarding is a delivery activity

Pilot preparation includes client selection, onboarding instructions, support process, communication, and feedback tracking.

**Lesson:** Treat pilot onboarding as a managed delivery workstream.

---

## Final Retrospective Action Log

| ID | Action | Owner | Recommended Timing | Status |
|----|--------|-------|--------------------|--------|
| PR-01 | Add load testing checkpoint to Sprint 2 for future projects | Scrum Master | Next project planning | Recommended |
| PR-02 | Create compliance evidence tracker from project kickoff | Scrum Master + Legal | Project initiation | Recommended |
| PR-03 | Add security remediation buffer to final sprint plans | Scrum Master + Engineering Lead | Sprint planning | Recommended |
| PR-04 | Begin pilot client recruitment one sprint earlier | Product Owner | Sprint 2 | Recommended |
| PR-05 | Confirm production-like staging environment before Sprint 2 | Engineering Lead + DevOps | Sprint 2 planning | Recommended |
| PR-06 | Maintain async communication protocol in future agile projects | Scrum Master | Team working agreement | Recommended |

---

## Scrum Master Closing Notes

The PayFlow Open Banking Payments delivery simulation demonstrates strong Agile PMO practice across sprint planning, stakeholder communication, risk management, compliance coordination, and delivery governance.

The team achieved all three sprint goals, maintained stable velocity, improved team health, and reached launch readiness with no open critical defects.

This retrospective closes the sprint delivery phase and supports the transition into UAT pilot, final sign-off, go-live, and hypercare.