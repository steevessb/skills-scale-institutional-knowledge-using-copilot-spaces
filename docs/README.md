# OctoAcme Project Management Guide

Welcome to OctoAcme's project management documentation! This README provides a concise overview of how we run projects, collaborate across teams, and deliver value to our customers.

## 📋 Overview

OctoAcme follows a structured yet flexible approach to project management that emphasizes:

- **Customer-first**: Prioritize customer value and usability
- **Iterative delivery**: Deliver small, testable increments
- **Clear ownership**: Each project has named Project Manager and Product Lead
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback and learning

## 🔄 Key Workflows

### 1. Project Initiation
**Goal**: Validate business need and authorize work

- Create Project One-pager (problem, goal, success metrics)
- Identify stakeholders and champions
- Define success criteria and initial timeline
- Compile initial risk list
- Confirm resource needs

**Decision Gate**: Move to planning when success metrics are clear, stakeholders agree on priority, and team availability is confirmed.

📄 [Detailed Initiation Guide](octoacme-project-initiation.md)

### 2. Project Planning
**Goal**: Turn approved initiative into actionable plan

- Hold kickoff meeting with stakeholders and delivery team
- Create prioritized backlog with acceptance criteria
- Estimate scope (T-shirt sizing or story points)
- Define Definition of Done (DoD)
- Identify dependencies and integration points
- Create release plan and milestone map

📄 [Detailed Planning Guide](octoacme-project-planning.md)

### 3. Execution & Tracking
**Goal**: Manage day-to-day execution and track progress

**Team Rhythm**:
- Daily standups (15 min) — progress, blockers, dependencies
- Weekly delivery sync — progress updates, flagged risks
- Demo/Review at end of each sprint or milestone

**Workflows**:
- Project board columns: Backlog → Ready → In Progress → In Review → QA → Done
- Small PRs (≤ 400 lines when possible)
- Include issue link and acceptance criteria in PR description
- Automated tests and linting in CI before review
- At least one approval before merging

📄 [Detailed Execution Guide](octoacme-execution-and-tracking.md)

### 4. Release & Deployment
**Goal**: Standardize releases to reduce risk and improve observability

**Release Types**:
- **Patch**: Hotfixes addressing critical production issues
- **Minor**: Incremental features and improvements
- **Major**: Significant functionality or breaking changes

**Pre-release Requirements**:
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback/mitigation plan documented
- Smoke tests prepared

📄 [Detailed Release Guide](octoacme-release-and-deployment.md)

### 5. Retrospective & Continuous Improvement
**Goal**: Capture learnings and convert them into actionable improvements

**When**: After each sprint, release, milestone, or incident

**Structure**:
- What went well
- What could be improved
- Action items (owner, due date)
- Follow-up on previous action items

**Best Practices**:
- Timebox: 45–75 minutes
- Prioritize 2–3 top action items to avoid overload
- Measure impact of improvements

📄 [Detailed Retrospective Guide](octoacme-retrospective-and-continuous-improvement.md)

## 👥 Roles & Responsibilities

### Project Manager (PM)
**Coordinates delivery, schedules, risk, and communications**

- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

**Communication**: Weekly status updates, risk registers, decision logs

### Product Manager (PdM)
**Defines outcomes, prioritizes backlog, and measures success**

- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

**Communication**: Weekly alignment with PM and engineering leads, roadmap updates, feature specs

### Developer
**Implements features, collaborates on design and testability**

- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

**Communication**: Daily standups, sprint planning, PR descriptions, code reviews

### QA/Tester
**Validates quality and acceptance criteria**

- Execute test plans and validate acceptance criteria
- Identify bugs and quality issues
- Collaborate on test automation and CI/CD
- Provide feedback on feature quality and usability

**Communication**: Test reports, bug tracking, demo participation

### Stakeholder
**Provides inputs and approvals**

- Review project goals and provide business context
- Approve key decisions and milestones
- Participate in demos and provide feedback
- Support resource allocation and prioritization

**Communication**: Monthly stakeholder updates, milestone reviews, escalations

📄 [Detailed Roles & Personas](octoacme-roles-and-personas.md)

## 💬 Communication Cadence

### Regular Meetings
- **Daily Standups**: 15 min, delivery team — focus on progress, blockers, dependencies
- **Weekly PM + PdM Sync**: Alignment on priorities, risks, and timelines
- **Weekly Delivery Sync**: Show progress, updates, and flagged risks
- **Twice-weekly Team Standups**: As agreed by delivery team
- **Monthly Stakeholder Updates**: Progress, metrics, and upcoming milestones
- **Sprint/Milestone Demos**: End of each sprint or milestone

### Status Updates
Use the **Weekly Status Template**:
- Progress this week
- Next steps
- Risks & blockers
- Ask / decisions needed

### Escalation Paths
- **Level 1**: Team-level triage in daily standup
- **Level 2**: PM escalates to Product Lead and dependent teams
- **Level 3**: Sponsor-level escalation for business-impacting issues
- **Security Incidents**: Follow security incident runbook and notify Security on-call

📄 [Detailed Risk & Communication Guide](octoacme-risks-and-communication.md)

## ✅ Quality Assurance Practices

### Testing Types
- **Unit tests**: For new logic
- **Integration tests**: Where applicable
- **End-to-end smoke tests**: For critical flows before release
- **Manual QA**: For feature acceptance when needed

### CI/CD Practices
- Automated tests and linting run in CI before review
- Security scanning in CI pipeline
- Passing CI required before merge
- Automated deployment pipeline preferred for production releases

### Acceptance Criteria & Definition of Done
- All backlog items include clear acceptance criteria
- Definition of Done (DoD) documented and agreed upon
- PRs include issue link and acceptance criteria in description
- At least one approval required before merging

### Quality Metrics
- Track test coverage
- Monitor build and test pass rates
- Use dashboards for key signals (errors, latency, usage)
- Measure success metrics from Project One-pager

## 📚 Key Artifacts

- **Project Charter / One-pager**: Problem statement, goals, success metrics, stakeholders
- **Roadmap and Release Plan**: Timelines, milestones, and feature priorities
- **Sprint/Iteration Backlog**: Prioritized work items with acceptance criteria
- **Acceptance Criteria & Definition of Done**: Quality standards and completion requirements
- **Risk Register**: Identified risks with impact, likelihood, owner, and mitigation plans
- **Retrospective Notes and Action Items**: Learnings and improvement initiatives
- **Release Notes**: Summary of changes, migration steps, and known issues

## 🚀 Getting Started

1. **New Project**: Start with the [Project Initiation Guide](octoacme-project-initiation.md)
2. **Planning Phase**: Follow the [Project Planning Guide](octoacme-project-planning.md)
3. **Active Development**: Reference the [Execution & Tracking Guide](octoacme-execution-and-tracking.md)
4. **Preparing Release**: Use the [Release & Deployment Guide](octoacme-release-and-deployment.md)
5. **Post-Project**: Conduct retrospective using the [Retrospective Guide](octoacme-retrospective-and-continuous-improvement.md)

## 📖 Additional Resources

- [Project Management Overview](octoacme-project-management-overview.md) — Complete overview of principles and lifecycle
- [Roles & Personas](octoacme-roles-and-personas.md) — Detailed role definitions
- [Risk Management & Communication](octoacme-risks-and-communication.md) — Risk handling and communication templates

## 💡 Using These Docs with Copilot Spaces

- Keep the Project Charter updated in the project repo
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context
- Reference these guides when setting up new projects or onboarding team members

---

**Questions or suggestions?** Contact the Project Management Office or open an issue in this repository.
