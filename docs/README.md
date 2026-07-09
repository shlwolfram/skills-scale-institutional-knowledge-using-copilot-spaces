# OctoAcme Project Management Documentation

## Welcome

This documentation defines how OctoAcme runs projects. Whether you're a Developer, Product Manager, or Project Manager, these guides will help you understand our processes, roles, and key artifacts.

## Core Principles

- **Customer-first**: prioritize customer value and usability
- **Iterative delivery**: deliver small, testable increments
- **Clear ownership**: each project has a named PM and Product Lead
- **Data-informed decisions**: measure impact and iterate based on evidence
- **Psychological safety**: encourage feedback and learning

## OctoAcme Project Management Overview

OctoAcme follows a structured, lifecycle-based approach to project management that emphasizes customer value, iterative delivery, and clear ownership. The methodology spans five core phases: **Initiation**, **Planning**, **Execution**, **Release**, and **Close & Retrospective**. Each phase is guided by a Project One-pager that captures the business problem, success metrics, stakeholders, and initial timeline. The organization prioritizes early alignment through a decision gate at the end of initiation, ensuring that stakeholder consensus and team availability are confirmed before moving into detailed planning. This lightweight but deliberate approach reduces rework and sets projects up for success from the start.

At the organizational level, OctoAcme defines clear roles and responsibilities to avoid ambiguity. **Project Managers (PMs)** coordinate delivery, manage schedules, and handle risk and stakeholder communication. **Product Managers (PdMs)** define what should be built, own success metrics, and prioritize the backlog. **Developers** implement features, write tests, and help identify technical risks, while **QA/Testing** validates quality and acceptance criteria. This separation of concerns enables teams to move faster while maintaining accountability. Weekly syncs between PM and PdM, twice-weekly standups, and monthly stakeholder updates create a predictable communication rhythm that keeps everyone aligned without creating unnecessary overhead.

Execution is managed through an iterative, pull-based backlog system supported by GitHub Projects. Work is broken into small, shippable increments with clear acceptance criteria and a Definition of Done. Pull requests are kept to 400 lines or fewer when possible, with automated testing and linting required before review and at least one approval before merge. Daily standups focus on progress, blockers, and dependencies, while a weekly delivery sync surfaces risks and flagged issues. Quality is assured through unit tests, integration tests, end-to-end smoke tests, security scanning in CI, and manual QA when needed. This multi-layered approach to testing and review minimizes defects and ensures that code entering production meets high standards.

Finally, OctoAcme embeds continuous improvement into its culture through structured retrospectives after each sprint, release, or milestone, and a formal risk management and communication process. The organization maintains a Risk Register tracking impact, likelihood, mitigation, and owner for each identified risk, reviewed weekly during syncs. Pre-release requirements include passing CI and security scans, drafted release notes, and a documented rollback plan. If issues arise, the team follows an incident playbook to triage, rollback, and capture learnings. By institutionalizing these practices—from risk escalation paths (Team → PM → Product Lead → Sponsor) to post-incident retrospectives—OctoAcme reduces single-person dependency, accelerates onboarding, and ensures that lessons learned feed back into the living documentation stored in `docs/` and `.copilot/`.

## Project Lifecycle Overview

OctoAcme projects follow a structured lifecycle:

1. **Initiation** - validate business need, identify stakeholders, confirm go/no-go decision
2. **Planning** - scope work, estimate, create prioritized backlog, define Definition of Done
3. **Execution** - build, test, review, iterate; manage daily standups and risk tracking
4. **Release** - deploy to production, run smoke tests, verify, communicate with stakeholders
5. **Close & Retrospective** - capture learnings and drive continuous improvements

## Documentation Map

| Document | Purpose | Best For |
|----------|---------|----------|
| [Project Management Overview](./octoacme-project-management-overview.md) | High-level introduction to OctoAcme's approach, roles, and principles | Everyone (start here!) |
| [Project Initiation Guide](./octoacme-project-initiation.md) | Validate business need, align stakeholders, authorize work | Product Managers, Project Managers |
| [Project Planning](./octoacme-project-planning.md) | Turn initiatives into actionable plans, define backlog, manage dependencies | Project Managers, Developers |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Day-to-day execution, progress tracking, quality standards, blocker escalation | Developers, Project Managers |
| [Risk Management & Communication](./octoacme-risks-and-communication.md) | Identify and manage risks, communicate status, escalation paths | Project Managers, Product Managers |
| [Release & Deployment Guide](./octoacme-release-and-deployment.md) | Standardize releases, pre-release requirements, rollback procedures | Developers, Product Managers |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Capture learnings, drive improvements, track action items | Everyone (after milestones) |
| [Roles & Personas](./octoacme-roles-and-personas.md) | Define typical roles, responsibilities, and communication patterns | Everyone (reference guide) |

## Quick Start by Role

**New to OctoAcme?** Start with the [Project Management Overview](./octoacme-project-management-overview.md).

### Developers
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — understand daily workflows, PR standards, and quality gates
- [Roles & Personas](./octoacme-roles-and-personas.md) — see developer responsibilities and communication patterns
- [Release & Deployment Guide](./octoacme-release-and-deployment.md) — learn deployment procedures and rollback processes

### Product Managers
- [Project Initiation Guide](./octoacme-project-initiation.md) — define problem statements and success metrics
- [Project Planning](./octoacme-project-planning.md) — understand backlog prioritization and acceptance criteria
- [Risk Management & Communication](./octoacme-risks-and-communication.md) — manage stakeholder communication and risk escalation
- [Roles & Personas](./octoacme-roles-and-personas.md) — review PM responsibilities and communication cadence

### Project Managers
- All documents are relevant; prioritize:
  - [Project Planning](./octoacme-project-planning.md) — scope, estimate, and plan delivery
  - [Execution & Tracking](./octoacme-execution-and-tracking.md) — manage standups, tracking, and escalation
  - [Risk Management & Communication](./octoacme-risks-and-communication.md) — maintain risk register and stakeholder updates
  - [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) — run retrospectives and track improvements

## How to Use These Docs

- **Onboarding**: New team members should read the Project Management Overview and their role-specific guides
- **Project Kickoff**: Use the relevant process guides during project initiation and planning meetings
- **Daily Operations**: Reference execution and tracking guidance during standups and sprint planning
- **Milestones & Retrospectives**: Use retrospective templates after sprints, releases, and major milestones
- **Copilot Spaces**: Add process-specific guidance into `.copilot/` to ground Copilot Spaces in team context
- **Living Documentation**: Keep these docs updated as processes evolve; use pull requests to propose changes

## Contributing to Process Docs

Have suggestions to improve these processes? We welcome feedback and improvements.

**To propose a change:**
1. Open an issue using the [Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) template
2. Describe the update, rationale, and suggested content
3. Submit a pull request with your proposed changes
4. Get feedback from the team and iterate

**Guidelines:**
- Keep changes aligned with existing OctoAcme principles
- Test new checklists and templates with your team before proposing
- Update related documents if your change affects multiple process areas
- Provide rationale for why the change improves clarity or closes a gap

## Key Artifacts & Templates

Across all projects, OctoAcme uses:

- **Project Charter / One-pager** — problem, goal, success metrics, stakeholders, timeline
- **Roadmap and Release Plan** — milestone map and delivery timeline
- **Sprint/Iteration Backlog** — prioritized, estimated work with acceptance criteria
- **Definition of Done** — quality standards before work is considered complete
- **Risk Register** — identified risks, impact, likelihood, mitigation, owner
- **Retrospective Notes** — learnings, action items, and follow-ups
- **Release Notes** — summary of changes, migrations, known issues
- **Status Reports** — weekly updates to stakeholders on progress, risks, and blockers

## Questions or Feedback?

If you have questions about these processes or need clarification, reach out to your Project Manager or Product Lead. If you'd like to suggest improvements, open an issue or start a discussion in the repository.

---

*Last updated: 2026-07-09*
