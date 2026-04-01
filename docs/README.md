# OctoAcme Project Management Docs

Welcome to the OctoAcme Project Management documentation space. Here you'll find the processes, standards, and tools used to deliver, track, and improve OctoAcme projects.

## Overview

OctoAcme runs projects with a lightweight, repeatable lifecycle that emphasizes iterative delivery, clear ownership, and measurable outcomes. Work begins in **Initiation**, where the team validates the business need and defines success criteria before investing in detailed planning — producing a Project One-pager, stakeholder list, communication plan, high-level timeline, and initial risk list. A decision gate (approve / don't approve) confirms priority and alignment before moving forward. Once approved, **Planning** turns the initiative into an actionable backlog: the team holds a kickoff, breaks work into shippable increments, defines acceptance criteria and a Definition of Done, captures estimates, and agrees on a milestone/release plan.

During **Execution & Tracking**, OctoAcme uses a project board (Backlog → Ready → In Progress → In Review → QA → Done) with a consistent team rhythm: daily standups, a weekly delivery sync, and demos at sprint or milestone boundaries. The **Project Manager (PM)** coordinates delivery, schedules, risks, and communications; the **Product Manager (PdM)** defines outcomes and prioritizes the backlog; **Developers** implement and review; **QA/Testing** validates acceptance criteria; and **Stakeholders** provide input and approvals. Communication follows a structured cadence — weekly PM+PdM alignment, twice-weekly team standups, and monthly stakeholder updates — with escalation paths and templates for status and incident communications.

Quality assurance is built into both delivery and release practices. On the engineering side, OctoAcme expects small PRs linked to issues and acceptance criteria, CI running tests and linting before review, and at least one approval before merge. Testing covers unit, integration, and end-to-end smoke tests for critical flows, with security scanning in CI. For **Release**, a deployment checklist covers staging validation, production deploy, post-deploy verification, and stakeholder announcement — backed by an incident/rollback playbook. After each release, **Retrospectives** convert learnings into tracked improvement actions, closing the loop on the delivery lifecycle.

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](./octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and lifecycle summary |
| [Project Initiation Guide](./octoacme-project-initiation.md) | Initiation checklist, one-pager template, and decision gate |
| [Project Planning](./octoacme-project-planning.md) | Scope, milestones, backlog setup, and Definition of Done |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Project board, team rhythm, and tracking practices |
| [Risk Management & Communication](./octoacme-risks-and-communication.md) | Risk register, escalation paths, and communication templates |
| [Release & Deployment Guide](./octoacme-release-and-deployment.md) | Pre-release checklist, deployment steps, and rollback playbook |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Retrospective format and improvement action tracking |
| [Roles & Personas Reference](./octoacme-roles-and-personas.md) | Responsibilities, goals, and communication patterns for each role |
