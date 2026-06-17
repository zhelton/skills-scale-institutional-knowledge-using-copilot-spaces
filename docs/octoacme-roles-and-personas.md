# OctoAcme — Expanded Roles & Personas

This document defines comprehensive roles and responsibilities used in OctoAcme project management. It expands on the core roles to include additional personas critical for successful cross-functional delivery.

---

## Core Roles

### Developers

#### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

#### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations
- Collaborate with Engineering Lead on technical design

#### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

#### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed
- Design reviews with Engineering Lead

---

### Product Managers

#### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

#### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics
- Partner with Data Analyst to track and measure success

#### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

#### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs
- Success metrics review with Data Analyst

---

### Project Managers

#### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

#### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication
- Work with Delivery Lead on sprint planning and dependency management
- Escalate risks and blockers following established escalation paths

#### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

#### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation
- Escalation coordination with PM and dependent teams

---

## Extended Roles

### Engineering Lead

#### Role Summary
Engineering Leads own technical strategy, design decisions, and squad coordination. They mentor developers and ensure technical quality and architectural consistency across the project.

#### Responsibilities
- Make or facilitate key technical design decisions
- Coordinate implementation across developer squads
- Mentor and support developers on technical challenges
- Review architecture and design docs for feasibility
- Identify technical risks and propose mitigations
- Collaborate with Product Manager on scope vs. technical trade-offs
- Partner with QA to define testability requirements and test strategy
- Coordinate with SRE/Platform Engineer on operational concerns

#### Interactions with Other Roles
- **With Product Manager:** Discusses trade-offs between scope and technical approach; provides technical input to feature feasibility
- **With Developers:** Leads design discussions, mentors on technical decisions, reviews complex code
- **With QA/Testing:** Defines test strategy and testability requirements
- **With Release Manager:** Coordinates deployment approach and rollback plans
- **With Security/Compliance Lead:** Incorporates security architecture requirements

#### Goals
- Ensure technical excellence and maintainability
- Reduce technical debt and complexity
- Enable team velocity through clear design decisions

#### Typical Communication
- Technical design reviews and architecture discussions
- Sprint planning and backlog refinement
- Code reviews and pull request guidance
- 1-on-1s with developers

---

### Delivery Lead (Delivery Manager)

#### Role Summary
Delivery Leads (also known as Delivery Managers or Scrum Masters) manage sprint execution, track cross-team dependencies, and resolve scheduling conflicts. They ensure the team can maintain consistent velocity and meet delivery commitments.

#### Responsibilities
- Manage sprint planning and capacity allocation
- Track team velocity and burndown
- Identify and escalate blockers and dependencies early
- Coordinate across teams for dependent work
- Resolve scheduling conflicts and resource constraints
- Support retrospectives and continuous improvement
- Maintain sprint board and backlog health
- Work closely with Project Manager on timeline and risk management

#### Interactions with Other Roles
- **With Project Manager:** Provides daily execution visibility, escalates risks, coordinates resource planning
- **With Developers:** Removes impediments, facilitates sprint planning and standups
- **With Product Manager:** Discusses backlog prioritization and commitment feasibility
- **With Release Manager:** Coordinates sprint completion with release planning
- **With other Delivery Leads:** Coordinates dependencies across teams

#### Goals
- Maintain consistent team velocity
- Deliver commitments on schedule
- Reduce blockers and unplanned work

#### Typical Communication
- Daily standups and sprint ceremonies
- Cross-team dependency coordination
- Status reports to Project Manager
- Retrospective facilitation

---

### Product Designer / UX Lead

#### Role Summary
Product Designers and UX Leads own user research, interaction design, and accessibility. They ensure solutions are intuitive, accessible, and meet user needs.

#### Responsibilities
- Conduct user research and validate design assumptions
- Create wireframes, prototypes, and design specifications
- Define interaction patterns and user flows
- Ensure accessibility standards (WCAG compliance)
- Collaborate on acceptance criteria to clarify user-facing requirements
- Review implementations for design fidelity and usability
- Advocate for user needs and usability

#### Interactions with Other Roles
- **With Product Manager:** Collaborates on feature definition and user requirements; conducts user research
- **With Developers:** Reviews implementations, provides design specifications, addresses design challenges during development
- **With QA/Testing:** Defines acceptance criteria for usability and accessibility; participates in UAT
- **With Engineering Lead:** Discusses technical feasibility of design approaches

#### Goals
- Maximize usability and user satisfaction
- Ensure accessibility and inclusive design
- Reduce rework through upfront user research

#### Typical Communication
- Design review meetings
- User research findings and recommendations
- Design specs and interaction guidelines
- Usability testing and feedback sessions

---

### Release Manager

#### Role Summary
Release Managers coordinate release windows, manage deployment processes, and ensure rollback readiness. They orchestrate cross-team communication and verify production readiness.

#### Responsibilities
- Create and maintain release plans and schedules
- Coordinate pre-release checklist completion
- Schedule and manage deployment windows
- Communicate release status to stakeholders
- Verify smoke tests and post-deploy checks
- Coordinate rollback if issues occur
- Document and communicate release notes
- Work with SRE/Platform Engineer on deployment mechanics
- Partner with Project Manager on release timeline and risk mitigation

#### Interactions with Other Roles
- **With Project Manager:** Coordinates release timing, manages stakeholder communication
- **With SRE/Platform Engineer:** Works with ops team on deployment process, readiness, and rollback mechanics
- **With Developers:** Ensures deployment readiness and resolves deployment-related issues
- **With Product Manager:** Communicates feature availability and release impact
- **With Security/Compliance Lead:** Ensures security approvals and controls are in place

#### Goals
- Release features safely and reliably
- Minimize production incidents and rollbacks
- Maintain clear stakeholder communication

#### Typical Communication
- Release planning meetings
- Pre-release readiness reviews
- Deployment window coordination
- Post-deploy verification and stakeholder updates

---

### Security/Compliance Lead

#### Role Summary
Security and Compliance Leads ensure that architectural decisions meet security and governance requirements. They coordinate security approvals, manage controls, and advise on risk mitigation.

#### Responsibilities
- Review architectural and design decisions for security implications
- Ensure security scanning and SAST/DAST tools are configured
- Define and enforce security controls and data handling requirements
- Coordinate security approvals and compliance checks
- Advise on threat models and security risks
- Participate in incident response for security-related issues
- Maintain security documentation and runbooks

#### Interactions with Other Roles
- **With Engineering Lead:** Reviews technical architecture for security posture; advises on secure design patterns
- **With Developers:** Reviews code and PRs for security vulnerabilities; provides security guidance
- **With Release Manager:** Gates releases pending security checks and compliance verification
- **With SRE/Platform Engineer:** Ensures monitoring and incident response for security events
- **With Project Manager:** Escalates security risks and dependencies

#### Goals
- Minimize security risks and vulnerabilities
- Ensure compliance with organizational and regulatory requirements
- Enable secure delivery at velocity

#### Typical Communication
- Security architecture reviews
- Threat modeling discussions
- Compliance and security checklist verification
- Security incident coordination

---

### SRE / Platform Engineer

#### Role Summary
Site Reliability Engineers (SREs) and Platform Engineers ensure operational readiness, monitoring, and incident response. They own runbooks, infrastructure, and post-deployment observability.

#### Responsibilities
- Ensure infrastructure and platform readiness for deployments
- Configure monitoring, alerting, and observability
- Create and maintain runbooks and incident response procedures
- Participate in deployments and monitor post-deploy health
- Own rollback mechanics and disaster recovery
- Support incident response and on-call rotation
- Advise on scalability and performance concerns
- Collaborate on capacity planning

#### Interactions with Other Roles
- **With Release Manager:** Coordinates deployment execution and post-deploy verification
- **With Developers:** Advises on operational concerns, troubleshoots production issues
- **With Engineering Lead:** Provides feedback on architectural decisions affecting operability
- **With Security/Compliance Lead:** Implements security monitoring and incident response controls
- **With Project Manager:** Escalates operational blockers or risks

#### Goals
- Maintain high availability and reliability
- Enable rapid incident response and recovery
- Support team velocity through operational excellence

#### Typical Communication
- Deployment coordination and post-deploy standby
- On-call handoff and incident updates
- Observability and monitoring discussions
- Capacity and scaling planning

---

### Data Analyst / Metrics Owner

#### Role Summary
Data Analysts and Metrics Owners define success metrics, instrument tracking, and validate that features deliver expected outcomes. They provide data-informed insights to guide prioritization and iteration.

#### Responsibilities
- Define success metrics aligned with product goals
- Instrument telemetry and analytics tracking
- Design and conduct A/B tests or experiments
- Analyze data and produce insights and reports
- Validate that launched features meet success criteria
- Advise Product Manager on data-informed decisions
- Create dashboards for key performance indicators (KPIs)

#### Interactions with Other Roles
- **With Product Manager:** Collaborates on metric definition and success criteria; provides analysis and insights
- **With Developers:** Coordinates on instrumentation implementation and data quality
- **With Project Manager:** Provides metrics-based progress reporting
- **With Engineering Lead:** Discusses technical approach for telemetry and tracking

#### Goals
- Ensure features deliver expected business value
- Provide data-informed insights for prioritization
- Enable continuous iteration based on evidence

#### Typical Communication
- Metrics definition and validation meetings
- Data analysis and reporting (dashboards, reports)
- A/B test planning and results reviews
- Retrospective participation

---

## Cross-Role Interactions & Handoff Checklist

### Project Kickoff
- [ ] PM + PdM define success metrics with Data Analyst
- [ ] Product Designer conducts initial user research
- [ ] Engineering Lead assesses technical feasibility with Developers
- [ ] Project Manager identifies cross-team dependencies with Delivery Lead
- [ ] Security/Compliance Lead identifies compliance requirements

### Sprint Planning
- [ ] Product Manager and Delivery Lead finalize sprint backlog
- [ ] Engineering Lead and Developers estimate technical effort
- [ ] Product Designer provides design specs and interaction guidelines
- [ ] QA/Testing defines test strategy with Engineering Lead
- [ ] Delivery Lead identifies dependencies and risks

### Development & Review
- [ ] Developers implement with guidance from Engineering Lead
- [ ] Product Designer reviews implementation for design fidelity
- [ ] Engineering Lead reviews code and architecture
- [ ] Security/Compliance Lead performs security review if needed
- [ ] QA/Testing validates acceptance criteria

### Pre-Release
- [ ] Project Manager confirms all acceptance criteria are met
- [ ] Release Manager compiles pre-release checklist
- [ ] SRE/Platform Engineer verifies deployment readiness
- [ ] Security/Compliance Lead verifies security controls
- [ ] Data Analyst confirms telemetry instrumentation

### Post-Release
- [ ] SRE/Platform Engineer monitors for issues
- [ ] Release Manager verifies smoke tests pass
- [ ] Data Analyst tracks success metrics
- [ ] Product Manager gathers user feedback
- [ ] Team conducts retrospective to capture learnings

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

- Use these persona definitions to clarify roles and responsibilities in project planning
- Reference specific personas when defining RACI matrices or decision-making authority
- Use the Cross-Role Interactions & Handoff Checklist to ensure all perspectives are included at key project phases
- Adapt personas to your organization's structure (e.g., combine roles, rename titles) while maintaining clear accountability
