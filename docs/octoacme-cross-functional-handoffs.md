# OctoAcme — Cross-Functional Handoffs & Checklists

## Purpose
Provide actionable checklists for the key handoff points in the OctoAcme project lifecycle. Each checklist clarifies which roles own each step, reducing ambiguity and preventing work from falling through the cracks.

For a full description of each role, see [Roles & Personas](octoacme-roles-and-personas.md).
For lifecycle context, see the relevant phase documents: [Project Initiation](octoacme-project-initiation.md), [Project Planning](octoacme-project-planning.md), [Execution & Tracking](octoacme-execution-and-tracking.md), [Risks & Communication](octoacme-risks-and-communication.md), [Release & Deployment](octoacme-release-and-deployment.md), and [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md).

---

## 1. Requirements → Design Handoff

**Trigger:** Product Manager has defined and prioritized a feature; UX design work is about to begin.
**Owner:** Product Manager hands off to UX Designer.

- [ ] Problem statement and success metrics documented (Product Manager)
- [ ] User stories and acceptance criteria drafted in the backlog (Product Manager)
- [ ] Relevant user research or feedback surfaced to UX Designer (Product Manager + Support/CS)
- [ ] Technical constraints and feasibility notes shared with UX Designer (Developers)
- [ ] Security and privacy requirements noted for the feature (Security Lead)
- [ ] Data tracking requirements (events, metrics) identified (Data Analyst)
- [ ] UX Designer confirms scope understanding and raises open questions (UX Designer)
- [ ] Design timeline added to project plan (Project Manager + UX Designer)

---

## 2. Design → Development Handoff

**Trigger:** UX design is approved and development is ready to begin.
**Owner:** UX Designer hands off to Developers.

- [ ] Final design specs, wireframes, and assets published in shared design tool (UX Designer)
- [ ] Accessibility requirements documented in acceptance criteria (UX Designer)
- [ ] Open design questions resolved with Product Manager (UX Designer + Product Manager)
- [ ] Developers have reviewed specs and raised questions before work starts (Developers)
- [ ] Analytics tracking plan reviewed and agreed upon (Data Analyst + Developers)
- [ ] Security review completed or scheduled for the feature (Security Lead)
- [ ] Feature branch strategy and PR conventions confirmed (DevOps Engineer + Developers)
- [ ] Definition of Done agreed upon for the feature (Product Manager + QA/Testing Lead + Developers)

---

## 3. Definition of Done (DoD) Checklist

Use this checklist before marking any feature or story as "Done" on the project board.

**Owner:** QA/Testing Lead confirms; Developers self-certify.

- [ ] All acceptance criteria met and verified
- [ ] Unit and integration tests written and passing in CI
- [ ] No known critical or high-severity defects outstanding
- [ ] Code reviewed and approved per team policy
- [ ] Security scan passing (no new high/critical findings unresolved)
- [ ] Design reviewed against approved UX specs (UX Designer sign-off)
- [ ] Analytics instrumentation in place and verified (Data Analyst)
- [ ] Documentation updated (README, API docs, release notes draft)
- [ ] Feature flagged or deployment-ready per DevOps standards (DevOps Engineer)
- [ ] Product Manager has accepted the feature

---

## 4. Release Readiness Checklist

**Trigger:** Sprint or milestone is complete; team is preparing to ship to production.
**Owner:** Project Manager drives; all roles contribute.

See also: [Release & Deployment Guide](octoacme-release-and-deployment.md).

- [ ] All in-scope features meet Definition of Done (QA/Testing Lead)
- [ ] Release notes drafted and reviewed for accuracy (Product Manager + Support/CS)
- [ ] Support team briefed on new features, known issues, and workarounds (Support/CS)
- [ ] Rollback plan documented and reviewed (DevOps Engineer + Project Manager)
- [ ] Deployment window communicated to all stakeholders (Project Manager)
- [ ] Staging environment verified with smoke tests (QA/Testing Lead + DevOps Engineer)
- [ ] Security scans and compliance checks completed (Security Lead + DevOps Engineer)
- [ ] Feature flags and configuration changes reviewed (DevOps Engineer)
- [ ] Monitoring and alerting confirmed for new features (DevOps Engineer + Data Analyst)
- [ ] Product Manager has given final release sign-off
- [ ] Project Manager has given coordination sign-off

---

## 5. Incident / Security Escalation Checklist

**Trigger:** A production incident or security vulnerability is identified.
**Owner:** Security Lead (security incidents) or DevOps Engineer (infrastructure/availability incidents); Project Manager coordinates communication.

### Immediate Response (0-1 hour)
- [ ] Incident acknowledged and on-call engineer paged (DevOps Engineer)
- [ ] Severity level assigned (P1–P4) and incident channel/ticket created (Project Manager + Security Lead)
- [ ] Affected scope identified (services, data, customers) (DevOps Engineer + Security Lead)
- [ ] Immediate mitigation or rollback initiated if applicable (DevOps Engineer)
- [ ] Stakeholders and Support/CS notified of impact (Project Manager)

### Investigation & Containment
- [ ] Root cause investigation begun; findings documented (DevOps Engineer + Developers + Security Lead)
- [ ] Additional engineers or SMEs engaged if needed (Project Manager)
- [ ] Customer communications drafted (Support/CS + Product Manager)
- [ ] Temporary workarounds communicated internally and externally (Support/CS)

### Resolution & Follow-up
- [ ] Fix implemented, tested, and deployed (Developers + QA/Testing Lead + DevOps Engineer)
- [ ] Incident resolved and stakeholders notified (Project Manager)
- [ ] Post-incident review (PIR) scheduled within 5 business days (Project Manager)
- [ ] PIR completed; root cause, timeline, and action items documented (all relevant roles)
- [ ] Action items added to backlog with owners and target dates (Project Manager + Product Manager)
- [ ] Risk register updated to reflect new controls (Project Manager + Security Lead)

---

## 6. Retrospective Input Checklist

**Trigger:** End of sprint, milestone, or project phase.
**Owner:** Project Manager facilitates; all roles contribute.

See also: [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md).

- [ ] Each role prepares "What went well / What could improve / Actions" (All roles)
- [ ] QA/Testing Lead shares quality metrics for the period (QA/Testing Lead)
- [ ] Data Analyst shares relevant product and delivery metrics (Data Analyst)
- [ ] DevOps Engineer reports on deployment frequency and incident counts (DevOps Engineer)
- [ ] Support/CS shares top customer pain points from the period (Support/CS)
- [ ] Security Lead reports on vulnerability status and security actions (Security Lead)
- [ ] Action items from last retrospective reviewed for completion (Project Manager)
- [ ] New action items documented with owners and due dates (Project Manager)
- [ ] Retrospective notes shared with the broader team (Project Manager)
