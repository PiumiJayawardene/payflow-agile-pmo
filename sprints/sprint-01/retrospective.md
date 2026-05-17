# Sprint Retrospective
## PayFlow Open Banking — Sprint 1

| Field | Detail |
|-------|--------|
| Date | Friday, Week 4 — 4:00 PM |
| Duration | 60 minutes |
| Facilitator | Piumi Jayawardene |
| Format | Start / Stop / Continue |
| Attendance | Delivery team only |
| Tool | Anonymous sticky notes grouped by Scrum Master |

---

## What Went Well — Continue

### 1. TrueLayer API setup was completed quickly

Once the sandbox credentials were available, the engineering team completed the initial API setup faster than expected.

**Continue:** Confirming external API access before sprint execution.

### 2. Daily standups stayed focused

The team consistently kept daily standups within the 15-minute timebox. Detailed technical discussions were moved to follow-up conversations.

**Continue:** Use parking-lot discussions for topics that do not need the full team.

### 3. Pull request reviews were completed quickly

No story was blocked for long periods waiting for code review. The engineering team maintained good collaboration.

**Continue:** Same-day pull request review target.

### 4. QA was involved from the beginning

QA reviewed acceptance criteria early and started preparing test cases before development was complete. This helped identify the mobile display issue before release.

**Continue:** Include QA in backlog refinement and sprint planning.

---

## What Did Not Go Well — Stop

### 1. Some development started before external dependencies were fully confirmed

The team started preparing integration work before all TrueLayer details were fully available.

**Stop:** Starting dependency-heavy work before access, credentials, and documentation are confirmed.

### 2. Engineering Lead received too many direct messages

The Engineering Lead experienced unnecessary interruptions through ad-hoc Slack messages.

**Stop:** Sending non-urgent direct messages for questions that can be handled asynchronously.

### 3. Mobile scope was not clearly defined

The bank connection story included UI work, but mobile responsiveness was not explicitly stated in the acceptance criteria.

**Stop:** Accepting UI stories into a sprint without clear device coverage.

---

## Improvements — Start

### 1. Confirm external dependencies before sprint planning

All external credentials, API access, vendor documentation, and environment details should be confirmed at least 3 days before sprint planning.

**Owner:** Scrum Master  
**Target:** Before Sprint 2 planning

### 2. Create an async communication channel

Create a shared `#dev-questions` channel for non-urgent technical questions. Direct messages should be used only for blockers or urgent issues.

**Owner:** Scrum Master  
**Target:** Sprint 2 Day 1

### 3. Add device scope to UI acceptance criteria

Every UI story should clearly state whether it applies to desktop, tablet, mobile, or all supported devices.

**Owner:** Product Owner + Scrum Master  
**Target:** Sprint 2 backlog refinement

### 4. Split large stories earlier

Stories estimated at 13 points or higher should be reviewed carefully and split where possible.

**Owner:** Product Owner + Delivery Team  
**Target:** Sprint 2 refinement

---

## Retrospective Action Log

| ID | Action | Owner | Due | Status |
|----|--------|-------|-----|--------|
| R1-01 | Confirm all Sprint 2 dependencies before planning | Scrum Master | Before Sprint 2 planning | Open |
| R1-02 | Create `#dev-questions` Slack channel | Scrum Master | Sprint 2 Day 1 | Open |
| R1-03 | Add device scope to remaining UI stories | Product Owner | Week 5 refinement | Open |
| R1-04 | Review 13-point stories for splitting | Product Owner + Team | Week 5 refinement | Open |
| R1-05 | Hold workload check-ins with delivery team | Scrum Master | Week 5 | Open |

---

## Team Health Check

Scale: 1 to 5, where 5 = excellent.

| Dimension | Score | Trend |
|-----------|-------|-------|
| Clarity of sprint goal | 4.4 | Baseline |
| Team collaboration | 4.6 | Baseline |
| Work-life balance | 3.7 | Monitor |
| Confidence in delivery | 4.1 | Baseline |
| Team morale | 4.0 | Baseline |

---

## Scrum Master Notes

The team delivered strong Sprint 1 outcomes and achieved the core sprint goal. The main improvement areas are dependency readiness, clearer UI acceptance criteria, and reducing interruptions for senior technical roles.

The work-life balance score should be monitored in Sprint 2. The Scrum Master will hold short individual check-ins with team members during Week 5.