# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA/Testing Lead

### Role Summary
The QA/Testing Lead owns the overall test strategy, ensures quality standards are met at every stage of the lifecycle, and acts as the team's quality advocate from planning through release.

### Responsibilities
- Define and maintain the test strategy, test plans, and acceptance criteria standards
- Own end-to-end, integration, and regression test suites
- Review and sign off on Definition of Done criteria with Product Managers and Developers
- Identify, track, and triage defects; coordinate fixes with Developers
- Report quality metrics (pass rates, defect density, coverage) to Project Managers
- Validate release readiness before deployment (see [Release & Deployment Guide](octoacme-release-and-deployment.md))

### Goals
- Prevent defects from reaching production
- Reduce cost of quality by shifting testing left in the lifecycle
- Maintain clear, agreed-upon acceptance criteria for every feature

### Typical Communication / Interaction
- **With Product Managers (PdM):** Refine acceptance criteria during backlog grooming; escalate scope changes that risk test coverage
- **With Project Managers (PM):** Provide weekly quality metrics; flag risks to release readiness in the risk register
- **With Developers:** Pair on testability design; review PRs for test coverage; triage defects together
- **With Stakeholders:** Present quality dashboards in sprint reviews; confirm sign-off on critical workflows
- **With DevOps Engineers:** Integrate automated test suites into CI/CD pipelines; agree on quality gates

---

## UX Designer

### Role Summary
UX Designers advocate for user needs and translate product requirements into intuitive, accessible experiences. They bridge the gap between customer insight and engineering implementation.

### Responsibilities
- Conduct user research and synthesize findings into actionable design insights
- Produce wireframes, prototypes, and design specifications
- Collaborate with Product Managers to refine requirements before development begins
- Run usability testing and feed results back to the backlog
- Maintain a shared design system and component library
- Ensure designs meet accessibility standards

### Goals
- Deliver experiences that are usable, accessible, and aligned with product goals
- Reduce rework by resolving UX ambiguity before engineering begins
- Create a consistent design language across the product

### Typical Communication / Interaction
- **With Product Managers (PdM):** Joint discovery sessions; translate user insights into prioritized requirements
- **With Project Managers (PM):** Surface design dependencies and timelines in project planning
- **With Developers:** Hand off design specs and assets; participate in design review on PRs; answer implementation questions
- **With QA/Testing Lead:** Align on usability acceptance criteria; validate that final builds match approved designs
- **With Stakeholders:** Present prototypes and usability findings; gather feedback before full development

---

## Data Analyst

### Role Summary
Data Analysts monitor product and operational metrics, surface actionable insights, and support data-driven decisions across planning, execution, and retrospective phases.

### Responsibilities
- Define, instrument, and maintain dashboards for key product and delivery metrics
- Analyze usage data, A/B test results, and experiment outcomes
- Provide regular reporting to Product Managers and Project Managers on KPIs and OKRs
- Identify anomalies or trends that signal risks or opportunities
- Support data requirements for new features (tracking plans, schema design)
- Contribute data findings to retrospectives and continuous improvement

### Goals
- Make objective, evidence-based decision-making accessible to the whole team
- Reduce time to insight by maintaining reliable, self-service dashboards
- Ensure instrumentation is in place before features ship

### Typical Communication / Interaction
- **With Product Managers (PdM):** Define success metrics; report on experiment outcomes; inform roadmap prioritization
- **With Project Managers (PM):** Contribute to status reports with data signals; flag metric anomalies that may indicate delivery risk
- **With Developers:** Align on tracking plans and data schema prior to implementation; validate instrumentation in QA
- **With QA/Testing Lead:** Verify that analytics events fire correctly and match the tracking plan
- **With Stakeholders:** Present data-driven insights in monthly stakeholder updates and sprint reviews

---

## DevOps Engineer

### Role Summary
DevOps Engineers design, build, and operate the CI/CD pipelines, infrastructure, and deployment automation that enable reliable, repeatable releases. They ensure the platform supports both velocity and stability.

### Responsibilities
- Design, implement, and maintain CI/CD pipelines and deployment automation
- Manage infrastructure (cloud, containers, configuration management)
- Define and enforce deployment standards, rollback procedures, and runbooks
- Own post-deploy monitoring, alerting, and on-call response for infrastructure issues
- Collaborate on security hardening and compliance automation
- Support developers with environment provisioning and toolchain improvements

### Goals
- Enable fast, safe deployments with minimal manual intervention
- Maintain high availability and observability of all production systems
- Reduce mean time to recovery (MTTR) for incidents

### Typical Communication / Interaction
- **With Project Managers (PM):** Coordinate deployment windows, communicate infrastructure risks, and update the risk register
- **With Product Managers (PdM):** Clarify infrastructure constraints that affect feature timelines or release scope
- **With Developers:** Define branching strategy and CI requirements; review infrastructure-as-code changes; unblock environment issues
- **With QA/Testing Lead:** Integrate automated test gates into pipelines; validate staging parity before release
- **With Security Lead:** Implement security controls in pipelines (SAST, DAST, dependency scanning); respond to vulnerability findings

---

## Support / Customer Success

### Role Summary
Support and Customer Success teams act as the voice of the customer. They manage post-release feedback, triage customer-reported issues, and ensure smooth adoption of new features.

### Responsibilities
- Triage, document, and escalate customer-reported bugs and feature requests
- Maintain support documentation, FAQs, and release notes for end users
- Coordinate with Product Managers on common customer pain points and feedback themes
- Communicate upcoming releases and breaking changes to customers and partners
- Track customer satisfaction metrics (CSAT, NPS) and share trends with the team
- Participate in release readiness reviews to ensure support teams are prepared

### Goals
- Minimize customer disruption from releases and incidents
- Close the feedback loop between customers and the product team
- Reduce time-to-resolution for critical customer issues

### Typical Communication / Interaction
- **With Product Managers (PdM):** Provide aggregated feedback and pain point themes; validate that release notes meet customer needs
- **With Project Managers (PM):** Flag high-severity customer issues that may require escalation or schedule adjustments
- **With Developers:** Report reproducible bugs with evidence; validate fixes in staging before release
- **With QA/Testing Lead:** Contribute customer-scenario test cases; confirm fixes resolve reported issues
- **With Stakeholders:** Present customer satisfaction data and adoption metrics in stakeholder updates

---

## Security Lead

### Role Summary
The Security Lead advises on secure development practices, owns the security review process, and coordinates incident response. They ensure security is embedded across the entire project lifecycle rather than treated as a gate at the end.

### Responsibilities
- Define and maintain the security review process and secure development standards
- Conduct threat modeling and security reviews for new features and architecture changes
- Own vulnerability management: triage findings from scans, prioritize remediation, track to closure
- Lead security incident response and post-incident reviews
- Ensure compliance requirements (regulatory, contractual) are reflected in delivery processes
- Train and advise team members on security best practices

### Goals
- Shift security left: identify and resolve risks before code ships to production
- Maintain a clear, current view of the threat landscape and outstanding vulnerabilities
- Ensure fast, effective response when security incidents occur

### Typical Communication / Interaction
- **With Project Managers (PM):** Surface security risks in the risk register; advise on remediation timelines; escalate critical vulnerabilities
- **With Product Managers (PdM):** Review features for privacy and security implications; ensure compliance constraints are reflected in acceptance criteria
- **With Developers:** Provide secure coding guidance; review code for security issues; validate fixes for reported vulnerabilities
- **With DevOps Engineers:** Define security controls in CI/CD (secret scanning, SAST, DAST, container scanning); review infrastructure configurations
- **With QA/Testing Lead:** Integrate security test cases (e.g., penetration testing scenarios) into the test plan
- **With Stakeholders:** Report on security posture, compliance status, and outstanding risks in monthly updates

---

## RACI / Responsibility Matrix

The following matrix summarizes accountability across key project activities. Use this as a quick reference to resolve ownership ambiguity.

**Key:** R = Responsible, A = Accountable, C = Consulted, I = Informed

| Activity | Project Manager | Product Manager | Developers | QA/Testing Lead | UX Designer | Data Analyst | DevOps Engineer | Support/CS | Security Lead |
|---|---|---|---|---|---|---|---|---|---|
| Define project scope and charter | A | C | I | I | I | I | I | I | I |
| Prioritize backlog & roadmap | C | A | C | C | C | C | I | C | C |
| Define acceptance criteria | C | A | C | R | R | C | I | C | C |
| Design & UX specifications | I | C | C | C | A | I | I | I | I |
| Feature implementation | I | I | A | C | C | I | C | I | I |
| Test planning & execution | C | I | C | A | C | I | C | I | C |
| CI/CD & deployment automation | C | I | C | C | I | I | A | I | C |
| Security review & threat model | C | C | C | C | I | I | C | I | A |
| Release readiness sign-off | A | C | C | R | C | I | R | R | R |
| Post-release monitoring | C | I | R | C | I | R | R | C | C |
| Customer feedback & escalation | C | C | C | I | I | C | I | A | I |
| Retrospective facilitation | A | C | C | C | C | C | C | C | C |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- For cross-functional handoff checklists and templates that reference these roles, see [Cross-Functional Handoffs & Checklists](octoacme-cross-functional-handoffs.md).

