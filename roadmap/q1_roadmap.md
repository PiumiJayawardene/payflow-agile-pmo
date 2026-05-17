# Q1 2025 Delivery Roadmap
## PayFlow Open Banking Payments Feature

This roadmap shows the 13-week Agile delivery timeline for the PayFlow Open Banking Payments feature, from project initiation through sprint delivery, UAT, go-live, and hypercare.

---

## Roadmap Overview

| Phase | Timeline | Key Outcome |
|-------|----------|-------------|
| Discovery & Initiation | Weeks 1–2 | Project setup, stakeholder alignment, backlog readiness |
| Sprint 1 | Weeks 3–4 | OAuth authentication and bank connection foundation |
| Sprint 2 | Weeks 5–6 | Payment initiation, SCA, and audit logging |
| Sprint 3 | Weeks 7–8 | Payment history, scheduled payments, performance, security, and UAT readiness |
| UAT & Go-Live | Weeks 9–13 | Compliance sign-off, pilot testing, controlled go-live, and hypercare |

---

## Mermaid Gantt Chart

```mermaid
gantt
  title PayFlow Open Banking — Q1 2025 Delivery Roadmap
  dateFormat  YYYY-MM-DD
  axisFormat  %b %d

  section Discovery & Initiation
    Project kickoff & team onboarding     :done,    d1, 2025-01-06, 3d
    TrueLayer API assessment              :done,    d2, 2025-01-06, 5d
    Architecture design & review          :done,    d3, 2025-01-08, 5d
    FCA PSD2 legal kickoff                :done,    d4, 2025-01-09, 3d
    Backlog refinement & estimation       :done,    d5, 2025-01-13, 3d

  section Sprint 1 — Auth & Bank Connection
    Sprint 1 planning                     :done,    s1p, 2025-01-20, 1d
    OAuth 2.0 bank authentication         :done,    s1a, 2025-01-20, 10d
    Two-factor authentication             :done,    s1b, 2025-01-20, 8d
    Bank account connection               :done,    s1c, 2025-01-22, 10d
    TrueLayer sandbox integration         :done,    s1d, 2025-01-20, 10d
    Sprint 1 review & retrospective       :done,    s1r, 2025-01-31, 1d

  section Sprint 2 — Payments & Compliance
    Sprint 2 planning                     :done,    s2p, 2025-02-03, 1d
    Bank connection status dashboard      :done,    s2a, 2025-02-03, 5d
    Payment initiation feature            :done,    s2b, 2025-02-03, 10d
    FCA audit logging                     :done,    s2c, 2025-02-05, 8d
    SCA compliance controls               :done,    s2d, 2025-02-05, 8d
    Sprint 2 review & retrospective       :done,    s2r, 2025-02-14, 1d

  section Sprint 3 — Launch Readiness
    Sprint 3 planning                     :done,    s3p, 2025-02-17, 1d
    Payment history view                  :done,    s3a, 2025-02-17, 7d
    Scheduled recurring payments          :done,    s3b, 2025-02-18, 8d
    Load testing                          :done,    s3c, 2025-02-19, 7d
    Penetration test coordination         :done,    s3d, 2025-02-21, 5d
    Production smoke testing              :done,    s3e, 2025-02-26, 2d
    Sprint 3 review & retrospective       :done,    s3r, 2025-02-28, 1d

  section UAT & Go-Live
    Compliance evidence pack submission   :active,  u1, 2025-03-03, 5d
    UAT pilot — 10 SME clients            :         u2, 2025-03-10, 10d
    Final FCA compliance sign-off         :         u3, 2025-03-17, 5d
    Go / No-Go meeting                    :milestone, u4, 2025-03-24, 1d
    Controlled go-live                    :milestone, gl, 2025-03-28, 1d
    Hypercare support                     :         hc, 2025-03-28, 14d
```

---

## Key Delivery Milestones

| Milestone | Target Date | Status | Notes |
|-----------|-------------|--------|-------|
| Project kickoff completed | 2025-01-08 | Done | Team onboarded and project initiated |
| Backlog refined and estimated | 2025-01-15 | Done | Initial backlog prepared for sprint planning |
| Sprint 1 completed | 2025-01-31 | Done | OAuth and bank connection foundation delivered |
| Sprint 2 completed | 2025-02-14 | Done | Payment initiation, SCA, and audit logging delivered |
| Sprint 3 completed | 2025-02-28 | Done | Launch-readiness work completed |
| Compliance evidence pack submitted | 2025-03-03 | In Progress | Final evidence prepared for Legal review |
| UAT pilot started | 2025-03-10 | Planned | 10 SME clients selected for pilot |
| Final compliance sign-off | 2025-03-21 | Planned | Required before payment feature launch |
| Go / No-Go meeting | 2025-03-24 | Planned | Sponsor decision before release |
| Controlled go-live | 2025-03-28 | Planned | Controlled release followed by hypercare |
| Hypercare completed | 2025-04-11 | Planned | Two-week post-launch support period |

---

## Roadmap Notes

- The delivery timeline is structured around three Agile sprints following a discovery and initiation phase.
- Sprint 1 focuses on authentication and secure bank connection.
- Sprint 2 delivers the core payment initiation journey with compliance controls.
- Sprint 3 focuses on launch readiness, including performance testing, security testing, UAT preparation, and final feature completion.
- The final phase includes compliance review, pilot testing, go-live approval, controlled release, and hypercare support.