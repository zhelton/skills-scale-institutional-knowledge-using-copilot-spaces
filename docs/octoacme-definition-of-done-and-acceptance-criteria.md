# OctoAcme Definition of Done & Acceptance Criteria Guide

This document defines the standards teams use to determine when work is complete and how to write acceptance criteria that prevent rework and scope creep.

---

## Definition of Done (DoD)

The Definition of Done is a shared agreement on the minimum quality bar that must be met before work is considered finished. It is **not** a checklist of tasks—it is a quality gate.

> **Why it matters:** Without a shared DoD, teams ship inconsistent quality, accumulate hidden technical debt, and spend significant time on rework. A clear DoD reduces ambiguity and creates accountability.

---

### Project-Level DoD

The following criteria must be satisfied before a project is considered complete and can be formally closed.

- [ ] All planned features and fixes are implemented and pass acceptance criteria
- [ ] All automated tests (unit, integration, end-to-end) pass in CI/CD
- [ ] Test coverage meets the project's agreed minimum threshold
- [ ] All known P1 and P2 defects are resolved or have documented, accepted mitigations
- [ ] Security review is complete and all critical/high findings are remediated
- [ ] Compliance requirements are validated and documented
- [ ] Performance benchmarks are met or documented exceptions are approved
- [ ] All documentation (user-facing and internal) is updated
- [ ] Runbooks and operational playbooks are reviewed and up to date
- [ ] Post-launch monitoring and alerting are in place and validated
- [ ] Stakeholder sign-off is obtained from Product Manager and key stakeholders
- [ ] Release notes and changelogs are published
- [ ] A retrospective is scheduled or completed

---

### Sprint-Level DoD

Each story or task must meet these criteria to be marked **Done** at the end of a sprint.

- [ ] Code is implemented and merged to the target branch
- [ ] All acceptance criteria on the ticket are met
- [ ] Unit and integration tests are written and passing
- [ ] No linting, formatting, or static analysis errors introduced
- [ ] Code has been reviewed and approved by at least one peer
- [ ] The feature works in a shared staging or review environment
- [ ] Any new configuration or environment variables are documented
- [ ] Relevant documentation (inline, README, wiki) is updated
- [ ] The ticket is updated with the resolution and closed

---

### Release-Level DoD

In addition to sprint-level criteria, the following must be satisfied before a release is deployed to production.

- [ ] All sprint-level DoD criteria are met for every item in the release
- [ ] Release branch is code-complete and passes all CI checks
- [ ] Release candidate is deployed to and validated in a staging environment
- [ ] Performance and load testing (if applicable) is complete
- [ ] Security scan of the release artifact is complete with no new critical findings
- [ ] Release checklist and go/no-go criteria are signed off
- [ ] Deployment runbook is reviewed and rollback procedure is confirmed
- [ ] Stakeholder communication about the release is prepared
- [ ] Monitoring dashboards and alerts are verified for the new release

---

## Acceptance Criteria

Acceptance Criteria (AC) define the specific, verifiable conditions a solution must satisfy to be accepted by the Product Manager and stakeholders. They are written before development begins and serve as the contract between product and engineering.

---

### Structure of Good Acceptance Criteria

Use the **Given / When / Then** (GWT) format for behavior-driven criteria:

```
Given [a specific context or precondition],
When [the user or system performs an action],
Then [the expected observable outcome occurs].
```

**Example:**

> **Given** a registered user is on the login page,
> **When** they submit valid credentials,
> **Then** they are redirected to the dashboard and a session is created.

For non-behavioral criteria (e.g., performance, compliance), use explicit, measurable statements:

> - The API must respond within 200ms at the 95th percentile under a load of 500 concurrent users.
> - All user-facing error messages must follow the UX copy guidelines.

---

### Best Practices for Writing Acceptance Criteria

| Practice | Why It Matters |
|---|---|
| Write AC before development starts | Sets clear expectations and prevents scope creep |
| Make each criterion independently verifiable | Enables targeted testing and clear sign-off |
| Avoid implementation details | AC defines *what*, not *how* |
| Include edge cases and error states | Prevents gaps that lead to undocumented behavior |
| Keep criteria user-focused | Ties technical work to real user outcomes |
| Limit AC to 3–7 per story | More than 7 often signals the story is too large |

---

### Common Gaps and Anti-Patterns

#### Anti-Pattern 1: Vague or Unmeasurable Criteria

❌ **Bad:** "The page should load quickly."

✅ **Better:** "The page must reach First Contentful Paint within 1.5 seconds on a simulated 4G connection."

---

#### Anti-Pattern 2: Missing Error and Edge Cases

❌ **Bad:** "Users can log in with their credentials."

✅ **Better:** Add AC for invalid credentials, locked accounts, expired sessions, and network errors.

---

#### Anti-Pattern 3: Implementation Embedded in AC

❌ **Bad:** "The backend stores the token in Redis with a TTL of 3600 seconds."

✅ **Better:** "The session persists for 60 minutes of inactivity and then expires, prompting re-authentication."

---

#### Anti-Pattern 4: AC Written After Development

**Problem:** Writing AC after the feature is built defines criteria around the implementation rather than user needs—leading to missed requirements and approval of poor solutions.

**Solution:** Acceptance criteria must be defined and reviewed during backlog refinement, before work enters a sprint.

---

#### Anti-Pattern 5: No Sign-Off Process

**Problem:** Stories are closed by developers without Product Manager validation, leading to features that meet technical criteria but miss user expectations.

**Solution:** The Product Manager explicitly accepts each story against its AC before it is marked Done.

---

## Workflow Integration

### Refinement (Pre-Sprint)

- Product Manager drafts acceptance criteria for backlog items
- Engineering Lead and Developers review for feasibility, completeness, and testability
- Product Designer/UX Lead confirms design alignment
- Security/Compliance Lead flags any criteria with compliance implications
- Final AC is agreed upon and documented on the ticket before the item is sprint-ready

### Sprint Planning

- Team confirms that all sprint items have complete, agreed-upon AC
- Items without complete AC are **not** pulled into the sprint
- Developers identify test cases they will write to validate AC

### Development

- Developers reference AC during implementation to stay aligned
- Automated tests are written to cover each acceptance criterion
- AC-related questions are resolved immediately with the Product Manager (not deferred)

### Review and Sign-Off

- Developer demonstrates the feature against each AC in the sprint review
- Product Manager validates each criterion and accepts or rejects
- Rejected items are moved back to the backlog with documented gaps

### Retrospective

- Teams review whether AC quality contributed to rework or scope creep
- Patterns of vague or missing AC are identified and addressed in the refinement process

---

## Developer Quick Reference Checklist

Use this checklist before submitting any PR or marking a story done.

### Code Quality
- [ ] All acceptance criteria are implemented
- [ ] Unit tests cover each AC (happy path + edge cases)
- [ ] Integration tests cover key workflows
- [ ] No linting or formatting errors
- [ ] No hardcoded secrets, credentials, or environment-specific values

### Review Readiness
- [ ] PR description explains *what* changed and *why*
- [ ] AC are listed in the PR or linked from the ticket
- [ ] Breaking changes are clearly identified
- [ ] Dependent PRs or configuration changes are linked

### Observability
- [ ] Relevant logs are added at appropriate levels
- [ ] Metrics or traces are instrumented for new critical paths
- [ ] Alerts are created or updated for new failure modes

### Documentation
- [ ] Inline comments explain non-obvious logic
- [ ] README or wiki is updated if behavior or setup changed
- [ ] API documentation is updated if contracts changed

### Security
- [ ] Input validation is implemented for all user-supplied data
- [ ] Authentication and authorization are enforced for protected resources
- [ ] Sensitive data is not logged or exposed in responses
