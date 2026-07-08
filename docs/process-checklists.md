# OctoAcme — Process Checklists & Templates

This document provides practical checklists and templates to standardize common project activities and close gaps identified in our process docs.

---

## Project Kickoff Checklist
- [ ] Project One-pager completed and stored in docs/
- [ ] Stakeholder list and communication plan documented
- [ ] Project roles assigned (PM, PdM, Eng Lead, QA Lead, Security)
- [ ] Initial risk register created
- [ ] Initial backlog skeleton added to project board
- [ ] Kickoff meeting scheduled with agenda and outcomes

---

## PR / Merge Checklist (For Authors)
- [ ] Linked issue(s) referenced in PR description
- [ ] Acceptance criteria included and met
- [ ] Tests added/updated (unit/integration as applicable)
- [ ] CI passes (build, tests, linters, security scans)
- [ ] At least one approval from a reviewer (and Eng Lead if architecture impact)
- [ ] No secrets or credentials included
- [ ] Update docs/ as needed (features, runbooks, migrations)
- Suggested PR description template:
  - Summary:
  - Related issue(s):
  - Acceptance criteria:
  - Testing notes:
  - Rollback plan (if applicable):

---

## Release Checklist
- [ ] All included PRs merged and linked to release
- [ ] All automated tests pass in release pipeline
- [ ] Security scans run and high severity issues addressed or mitigated
- [ ] Release notes drafted (summary, notable changes, known issues)
- [ ] Rollback / mitigation plan documented
- [ ] Smoke tests prepared and executed on staging
- [ ] Stakeholders notified for release window
- [ ] Post-deploy verification scheduled

---

## QA Checklist
- [ ] Unit tests cover new logic and critical edge cases
- [ ] Integration tests validate API/contract interactions
- [ ] E2E or smoke test covers critical user flows
- [ ] Test data and environments prepared and stable
- [ ] Test results reported in PR or QA ticket
- [ ] Defects triaged with severity and owner assigned

---

## Security Checklist
- [ ] Threat modeling performed for significant changes
- [ ] SAST/Dependency scanning run in CI
- [ ] Secrets scanning enabled and clean
- [ ] Security Officer review for high-risk features
- [ ] Incident response contact and runbook referenced

---

## Risk Register Template
Columns: ID | Description | Impact | Likelihood | Owner | Mitigation | Status

Example:
- R-001 | Third-party integration SLA risk | High | Medium | Eng Lead | Contract SLA + fallback | Open

---

## How to use these checklists
- Include checklist verification in PRs, sprint planning, and release runbooks.
- Add or adapt items per project needs and keep them versioned in docs/.
