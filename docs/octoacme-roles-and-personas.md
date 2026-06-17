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

## Engineering Lead

### Role Summary
Engineering Leads own the technical direction of a product area or team. They partner with Product Managers on feasibility, mentor developers, and ensure engineering standards are upheld across the codebase.

### Responsibilities
- Define and enforce technical standards, patterns, and best practices
- Lead architectural decisions and technical design reviews
- Mentor and grow developers through feedback and pairing
- Collaborate with Product Managers to assess feasibility and trade-offs
- Identify technical debt and plan remediation work

### Goals
- Maintain a healthy, scalable, and well-tested codebase
- Enable the team to deliver sustainably and at high quality
- Reduce unplanned work caused by technical debt or poor design

### Interactions with Other Roles
- **Product Manager**: Aligns on scope, feasibility, and technical constraints
- **Project Manager**: Coordinates engineering capacity and flags technical blockers
- **Developer**: Provides technical guidance, reviews designs, and unblocks implementation
- **SRE/Platform Engineer**: Collaborates on reliability standards and infrastructure changes

### Typical Communication
- Architecture decision records (ADRs) and design documents
- Code review feedback and technical RFCs
- Engineering syncs and sprint planning sessions

---

## Delivery Lead

### Role Summary
Delivery Leads focus on end-to-end flow of work through the team. They remove impediments, optimize processes, and ensure the team operates predictably and sustainably.

### Responsibilities
- Track and unblock work items across the team
- Facilitate ceremonies: standups, sprint planning, retrospectives
- Monitor team velocity, cycle time, and delivery health metrics
- Coordinate cross-team dependencies and escalation paths
- Drive continuous improvement in delivery practices

### Goals
- Maximize predictable, sustainable throughput
- Minimize work-in-progress and queue times
- Keep stakeholders informed with timely, accurate status updates

### Interactions with Other Roles
- **Project Manager**: Shares delivery health data and co-owns risk management
- **Engineering Lead**: Aligns on capacity planning and technical blockers
- **Product Manager**: Ensures roadmap priorities flow smoothly through the backlog

### Typical Communication
- Daily standups and weekly delivery health reports
- Impediment logs and escalation notices
- Sprint review summaries and velocity trend reports

---

## Product Designer / UX Lead

### Role Summary
Product Designers translate user needs and business goals into intuitive, accessible experiences. They bridge research, design, and engineering to ensure solutions are usable and valuable.

### Responsibilities
- Conduct user research, interviews, and usability testing
- Create wireframes, prototypes, and high-fidelity design specs
- Define and maintain the design system and component library
- Validate designs with acceptance criteria tied to user outcomes
- Partner with engineering to ensure implementation fidelity

### Goals
- Deliver experiences that are intuitive, accessible, and delightful
- Reduce usability-related rework through early design validation
- Ensure design consistency across the product

### Interactions with Other Roles
- **Product Manager**: Translates product requirements into design solutions
- **Developer**: Provides specs, assets, and implementation guidance
- **Engineering Lead**: Aligns on component patterns and design system constraints

### Typical Communication
- Design review sessions and prototype walkthroughs
- Figma/design tool links in tickets and documentation
- Usability test findings and design iteration notes

---

## Release Manager

### Role Summary
Release Managers coordinate the end-to-end release process, ensuring changes are deployed safely, consistently, and with minimal disruption to users.

### Responsibilities
- Maintain the release calendar and coordinate deployment windows
- Own the release checklist and go/no-go criteria
- Coordinate with QA, engineering, and operations for release readiness
- Manage release notes, changelogs, and communication to stakeholders
- Lead incident escalation and rollback decisions during deployments

### Goals
- Achieve zero unplanned downtime from releases
- Ensure every release follows a consistent, auditable process
- Reduce time-to-release through process automation and standardization

### Interactions with Other Roles
- **Engineering Lead**: Validates release branch quality and technical readiness
- **SRE/Platform Engineer**: Coordinates deployment execution and monitoring
- **Project Manager**: Aligns release timing with project milestones and stakeholder commitments

### Typical Communication
- Release readiness reports and go/no-go decisions
- Post-release summaries and incident reports
- Changelog updates and stakeholder notifications

---

## Security / Compliance Lead

### Role Summary
Security/Compliance Leads ensure that software is built and operated in accordance with security best practices, regulatory requirements, and organizational policy.

### Responsibilities
- Define and maintain security standards and threat models
- Review designs and code changes for security implications
- Coordinate vulnerability assessments and penetration testing
- Ensure compliance with relevant regulations (e.g., SOC 2, GDPR, HIPAA)
- Lead incident response for security events

### Goals
- Reduce the attack surface and blast radius of potential vulnerabilities
- Ensure audit-readiness and compliance posture at all times
- Embed security practices into the development lifecycle (shift left)

### Interactions with Other Roles
- **Engineering Lead**: Reviews architectural decisions for security implications
- **Release Manager**: Validates security gates before each release
- **Developer**: Provides secure coding guidance and reviews high-risk changes

### Typical Communication
- Security review findings and risk assessments
- Compliance reports and audit artifacts
- Vulnerability disclosure notices and remediation tracking

---

## SRE / Platform Engineer

### Role Summary
SRE/Platform Engineers build and maintain the infrastructure, tooling, and observability systems that enable teams to deliver and operate software reliably at scale.

### Responsibilities
- Design and maintain CI/CD pipelines, infrastructure, and developer tooling
- Define and track Service Level Objectives (SLOs) and error budgets
- Respond to and lead resolution of production incidents
- Build observability solutions (logging, tracing, alerting)
- Drive reliability improvements and post-incident reviews

### Goals
- Maintain system reliability within defined SLO targets
- Reduce mean time to detection (MTTD) and mean time to recovery (MTTR)
- Enable development teams to self-serve on infrastructure needs

### Interactions with Other Roles
- **Engineering Lead**: Aligns on reliability requirements and infrastructure constraints
- **Release Manager**: Supports deployment execution and rollback procedures
- **Security/Compliance Lead**: Implements security controls in infrastructure and pipelines

### Typical Communication
- SLO dashboards and error budget reports
- Incident postmortems and action item tracking
- Runbooks, on-call documentation, and infrastructure change notifications

---

## Data Analyst / Metrics Owner

### Role Summary
Data Analysts and Metrics Owners ensure the team has reliable, actionable data to make informed decisions. They design metrics frameworks, build dashboards, and support data-driven retrospectives.

### Responsibilities
- Define and instrument key product, quality, and delivery metrics
- Build and maintain dashboards and reporting pipelines
- Analyze trends and surface actionable insights for the team
- Support A/B testing, feature flag analysis, and experiment design
- Validate that data pipelines are accurate and well-documented

### Goals
- Provide timely, trustworthy data for decision-making
- Reduce time-to-insight for product and delivery questions
- Ensure metric definitions are shared, stable, and well-understood

### Interactions with Other Roles
- **Product Manager**: Supports outcome measurement and experiment analysis
- **Engineering Lead**: Aligns on instrumentation and telemetry standards
- **Delivery Lead**: Provides delivery health metrics and trend analysis

### Typical Communication
- Weekly metrics digests and sprint health reports
- Dashboard links and data documentation in project wikis
- Ad-hoc analysis summaries shared in team channels

---

## Cross-Role Interaction Checklist

Use this checklist to ensure appropriate collaboration at each key project phase.

### Project Kickoff
- [ ] **Engineering Lead** + **Product Manager**: Align on scope, feasibility, and technical constraints
- [ ] **Project Manager** + **Delivery Lead**: Establish timelines, milestones, and delivery cadence
- [ ] **Product Designer/UX Lead**: Present initial research findings and design direction
- [ ] **Security/Compliance Lead**: Review for compliance and regulatory requirements
- [ ] **SRE/Platform Engineer**: Confirm infrastructure and tooling readiness
- [ ] **Data Analyst/Metrics Owner**: Define success metrics and instrumentation plan

### Sprint Planning
- [ ] **Product Manager**: Confirms acceptance criteria are clear and complete for all backlog items
- [ ] **Engineering Lead**: Validates technical feasibility and estimates
- [ ] **Delivery Lead**: Ensures capacity is accounted for and WIP limits are respected
- [ ] **Product Designer/UX Lead**: Confirms designs are ready and handed off for sprint items
- [ ] **Release Manager**: Flags items with release dependencies or deployment windows

### Development Phase
- [ ] **Engineering Lead**: Reviews PRs for technical quality and standards compliance
- [ ] **Security/Compliance Lead**: Reviews high-risk changes for security implications
- [ ] **SRE/Platform Engineer**: Validates observability and infrastructure changes
- [ ] **Data Analyst/Metrics Owner**: Confirms instrumentation is implemented correctly

### Pre-Release
- [ ] **Release Manager**: Confirms go/no-go criteria and release checklist are complete
- [ ] **Security/Compliance Lead**: Signs off on security review for the release
- [ ] **SRE/Platform Engineer**: Verifies deployment runbook and rollback plan
- [ ] **Product Manager**: Validates that acceptance criteria for release scope are met
- [ ] **Data Analyst/Metrics Owner**: Confirms monitoring and alerting for new features

### Post-Release
- [ ] **Release Manager**: Publishes release notes and notifies stakeholders
- [ ] **SRE/Platform Engineer**: Monitors SLOs and error budgets post-deployment
- [ ] **Delivery Lead**: Captures delivery metrics and schedules retrospective
- [ ] **Data Analyst/Metrics Owner**: Reviews post-launch metrics and shares findings
- [ ] **Project Manager**: Updates project status and closes delivery artifacts

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

