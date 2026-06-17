# OctoAcme — Definition of Done (DoD) & Acceptance Criteria Guide

## Purpose
This guide provides clear standards for what constitutes "done" work and how to define acceptance criteria that reduce ambiguity, improve quality, and enable faster delivery.

## Definition of Done (DoD)

Definition of Done is a shared understanding of what must be completed before work moves from one stage to the next. DoD ensures consistent quality and reduces rework.

### Project/Sprint Level DoD
Before work can move to "Done" status:
- [ ] All acceptance criteria have been met and verified
- [ ] Code is written and peer-reviewed (minimum 1 approval)
- [ ] Unit tests written and passing (target: >80% coverage for new code)
- [ ] Integration tests completed where applicable
- [ ] Security scan completed and no critical/high vulnerabilities introduced
- [ ] Code follows team style guide and linting rules
- [ ] Documentation updated (inline comments, README, runbooks if needed)
- [ ] Product Designer has reviewed for design fidelity and UX
- [ ] QA/Testing has validated acceptance criteria
- [ ] Accessibility requirements met (WCAG 2.1 AA minimum)

### Release/Deployment Level DoD
Before a feature can be released to production:
- [ ] All acceptance criteria met and verified in production readiness environment
- [ ] Release notes drafted and reviewed
- [ ] Deployment runbook created and tested
- [ ] Rollback plan documented and tested
- [ ] Smoke tests defined and passing
- [ ] Monitoring and alerting configured
- [ ] Post-deploy verification checklist prepared
- [ ] Security/Compliance Lead approval received
- [ ] Stakeholder sign-off obtained
- [ ] All blockers resolved or escalated

## Acceptance Criteria

Acceptance criteria define the specific, testable conditions that must be satisfied for a work item to be considered complete.

### Structure
Acceptance criteria should follow this format:

```
Given [context]
When [action taken]
Then [expected result]
```

Or:

```
- The system should [specific behavior]
- The system should [another behavior]
```

### Writing Effective Acceptance Criteria

#### DO
- ✅ Be specific and measurable ("Response time < 200ms" not "fast")
- ✅ Focus on user value and outcomes
- ✅ Include both happy path and edge cases
- ✅ Reference acceptance criteria from other related items if needed
- ✅ Involve stakeholders (Product Manager, Product Designer, QA) in definition
- ✅ Update criteria during sprint if scope clarifies

#### DON'T
- ❌ Use vague language ("looks good", "works properly", "as designed")
- ❌ Mix acceptance criteria with implementation details ("use Redis for caching")
- ❌ Create criteria so broad they require subtasks
- ❌ Forget about non-functional requirements (performance, security, accessibility)
- ❌ Leave criteria undefined and clarify "during development"

### Acceptance Criteria Template

```markdown
## Feature: [Feature Name]

### Background
[Context that helps understand why this feature matters]

### Acceptance Criteria
1. **Functional Requirement**
   - Given: [context]
   - When: [user action]
   - Then: [expected result]

2. **Functional Requirement**
   - The system should [specific behavior]
   - [Edge case handling]

3. **Non-Functional Requirement**
   - Performance: Response time should be < 200ms for typical queries
   - Accessibility: All interactive elements should be keyboard accessible and meet WCAG 2.1 AA
   - Security: No sensitive data should be logged; encryption in transit/at rest

4. **Edge Cases & Error Handling**
   - When [invalid input], the system should [appropriate response]
   - When [network failure], the system should [graceful degradation]

### Definition of Done Checklist
- [ ] Code passes all tests
- [ ] Code reviewed and approved
- [ ] Product Designer reviewed for UX fidelity
- [ ] Security review completed
- [ ] Documentation updated
- [ ] QA validates all acceptance criteria
```

## Common Gaps & Anti-Patterns

### Gap: Missing Non-Functional Requirements
**Problem:** Criteria focus only on feature behavior, ignoring performance, security, or accessibility.

**Solution:** Always include acceptance criteria for:
- **Performance:** Response time targets, throughput, scalability expectations
- **Security:** Data handling, encryption, authentication/authorization rules
- **Accessibility:** WCAG compliance, keyboard navigation, screen reader support
- **Reliability:** Error handling, recovery from failures

### Gap: Acceptance Criteria Too Vague
**Problem:** "User can view their dashboard" doesn't specify what data, layout, or interactions are expected.

**Solution:** Break down into specific behaviors:
- "User sees personalized welcome message with name"
- "Dashboard shows 5 recent transactions with date, amount, category"
- "User can click transaction row to view full details"

### Gap: Acceptance Criteria Mixed with Implementation
**Problem:** "Use PostgreSQL to store user data" is implementation, not acceptance criteria.

**Solution:** Focus on "what" not "how":
- **Instead:** "User data persists across sessions"
- **Better:** "When user logs out and logs back in, their saved preferences are restored"

### Gap: No Edge Case Handling
**Problem:** Criteria only describe the happy path.

**Solution:** Add edge cases:
- What happens with empty results?
- What if the user lacks permissions?
- How does the system handle network errors?
- What's the timeout behavior for slow queries?

## Workflow Integration

### During Backlog Refinement
1. Product Manager drafts acceptance criteria with Product Designer
2. Engineering Lead assesses feasibility and suggests technical requirements
3. QA identifies test scenarios and edge cases
4. Team discusses and refines until clear and testable

### During Sprint Planning
1. Team reviews acceptance criteria for selected items
2. Developers ask clarifying questions
3. Criteria are updated if needed (with Product Manager approval)
4. Criteria become the basis for PR review and QA testing

### During Development
1. Developer implements to acceptance criteria
2. PR description links to issue with acceptance criteria
3. Reviewer verifies PR satisfies all criteria
4. Product Designer reviews implementation fidelity

### During Testing & Review
1. QA uses acceptance criteria to define test cases
2. QA manually tests or automates test scenarios
3. Product Designer verifies UX implementation
4. Security/Compliance Lead reviews if needed

### During Retrospective
1. Team reflects on acceptance criteria clarity
2. If criteria caused rework or confusion, capture improvement
3. Update team practices based on feedback

## Quick Reference: DoD Checklist for Developers

Before marking work "Done":

### Code Quality
- [ ] Code compiles/runs without errors
- [ ] Linting passes
- [ ] All unit tests passing (>80% coverage for new code)
- [ ] Integration tests passing if applicable
- [ ] No debug logs or commented-out code

### Review & Collaboration
- [ ] Code reviewed by at least one peer
- [ ] All review comments addressed or discussed
- [ ] Product Designer reviewed for UX compliance
- [ ] Technical lead approved design if needed

### Security & Compliance
- [ ] Security scan passed (no critical/high vulnerabilities)
- [ ] No hardcoded secrets or credentials
- [ ] Data is encrypted in transit/at rest where required
- [ ] Accessibility requirements met

### Documentation & Testing
- [ ] Acceptance criteria demonstrated as met
- [ ] Documentation (comments, README, runbooks) updated
- [ ] Test data or examples provided if needed
- [ ] All acceptance criteria verified by QA or submitter

---

## References
- Related: [Execution & Tracking](octoacme-execution-and-tracking.md)
- Related: [Project Planning](octoacme-project-planning.md)
