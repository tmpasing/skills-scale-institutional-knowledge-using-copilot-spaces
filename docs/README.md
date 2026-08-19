# OctoAcme Project Management Documentation

## Overview
OctoAcme follows a structured, iterative approach to project management that emphasizes customer value, clear ownership, data-informed decision making, and psychological safety. This documentation collection provides guidance and templates for everyone involved in delivering projects — from initial idea validation through planning, execution, release, and continuous improvement.

## Core Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: every project names a Project Manager and Product Lead.
- Data-informed: measure results and iterate based on evidence.
- Psychological safety: encourage feedback, learning, and blameless improvement.

## Project lifecycle at a glance
1. Initiation → Validate business need and align stakeholders
2. Planning → Break work into shippable increments
3. Execution → Build, test, review, and iterate
4. Release → Deploy and verify
5. Retrospective → Capture learnings and improve

## Brief summary of OctoAcme project management processes
OctoAcme’s project management approach is structured around lightweight, repeatable artifacts and an iterative lifecycle: Initiation, Planning, Execution, Release, and Close. Work begins with a Project One-pager to capture the problem, goals, success metrics, stakeholders, and a high‑level timeline. Planning turns that into a prioritized backlog (using a Backlog Item template), estimates, a Definition of Done, and a release plan. Day‑to‑day work is tracked on a project board with clear columns (Backlog, Ready, In Progress, In Review, QA, Done) and supported by checklists and templates (risk register, release notes, and deployment/rollback checklists) to keep releases low‑risk and well documented.

Roles and responsibilities are explicit: Product Managers define outcomes, prioritize the backlog, and measure success; Project Managers coordinate schedules, risks, and cross‑team communication; Developers implement features, produce tests and documentation; and QA validates acceptance. Clear ownership is emphasized for each project and artifact—PM and Product Lead are named owners—so decisions, estimates, and mitigations have accountable parties. Persona definitions are also used to frame exercises and role‑based guidance in the team’s learning materials.

Communication follows a predictable cadence to maintain alignment and surface risks early: short daily standups (focused on progress and blockers), weekly delivery syncs for progress and risk discussion, and regular demos/reviews at the end of sprints or milestones. Stakeholders get periodic updates (weekly or monthly as appropriate), and there are documented escalation paths (team → PM → Product Lead → Sponsor) plus an incident/triage workflow for production or security issues. The risk register and weekly PM syncs are the primary mechanisms for monitoring and updating risk status and cross‑team dependencies.

Quality assurance and release controls are built into the workflow. PR guidance encourages small, focused changes (target ≤ 400 lines), with PR descriptions including issue links and acceptance criteria; CI must run tests and lint before review, and at least one approval is required before merging. Testing is multi‑layered—unit tests for logic, integration tests where relevant, and end‑to‑end smoke tests for critical flows—combined with security scanning in CI and manual QA as needed. Releases follow type‑specific checklists (patch, minor, major) with pre‑release verification, smoke tests in staging, an automated deployment pipeline where possible, and documented rollback/incident playbooks to minimize production risk.

## Documentation index

### Getting Started
- docs/octoacme-project-management-overview.md — Introduction to roles, artifacts, and cadence

### By Phase
- docs/octoacme-project-initiation.md — How to validate ideas and align stakeholders
- docs/octoacme-project-planning.md — Backlog creation, estimation, and release planning
- docs/octoacme-execution-and-tracking.md — Team rhythm, PR workflow, and progress tracking
- docs/octoacme-release-and-deployment.md — Pre‑release checks, deployment, and rollback playbook
- docs/octoacme-retrospective-and-continuous-improvement.md — Retrospectives and action tracking

### Cross‑Cutting
- docs/octoacme-risks-and-communication.md — Risk register, escalation, and stakeholder comms
- docs/octoacme-roles-and-personas.md — Role summaries and responsibilities

## Quick reference by role
- Developers: Start with docs/octoacme-project-management-overview.md and docs/octoacme-execution-and-tracking.md. Key touchpoints: daily standups, sprint planning, PR workflow.
- Product Managers: Start with docs/octoacme-project-initiation.md and docs/octoacme-project-planning.md. Key touchpoints: stakeholder alignment, backlog prioritization, success metrics.
- Project Managers: Start with docs/octoacme-project-management-overview.md, docs/octoacme-risks-and-communication.md, and docs/octoacme-release-and-deployment.md. Key touchpoints: risk tracking, status reporting, cross‑team coordination.

## When to use each document
- Initiation: Use the Project Initiation Guide when validating an idea and preparing a one‑pager.
- Planning: Use Project Planning to build a backlog, estimates, and release plan.
- Execution: Use Execution & Tracking for day‑to‑day work management and PR practices.
- Release: Use Release & Deployment for pre‑release checks and deployment steps.
- Retrospective: Use Retrospective & Continuous Improvement after releases or sprints to capture improvements.

## Contributing
To suggest changes, create an issue using the Process Doc Update template at .github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml and reference the document path you want to update.
