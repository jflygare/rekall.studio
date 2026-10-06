# Current work

This is the authoritative task queue and handoff record. Tasks are ordered by priority. A listed task is not an automatic assignment. Accepted project decisions live in [DECISIONS.md](DECISIONS.md); the [brain dump](../BACK_OF_THE_NAPKIN.md) is not a committed backlog.

Use statuses `pending`, `in progress`, `blocked`, `awaiting review`, and `done`. Record a concrete blocker for blocked tasks; use awaiting review after delivery and done after owner acceptance or merge. Add a plan link only when the task needs one.

## PREP-001 — Prepare portable AI collaboration

- **Status:** awaiting review
- **Assignment:** Jesse approved implementation on 2026-10-06.
- **Objective:** A fresh agent can understand the project, find assigned work, contribute within its authority, and leave a durable handoff.
- **Branch:** `docs/portable-ai-collaboration`
- **PR:** [Draft PR #1](https://github.com/jflygare/rekall.studio/pull/1), targeting `main`.
- **Scope:** Shared repository guidance, task tracking, decision records, local ignore rules, and onboarding validation. No application scaffolding, stack selection, or product implementation.

### Acceptance criteria

- README, AGENTS, WORK, and DECISIONS have distinct, consistent responsibilities and working links.
- The exploratory concept and inspiration assets remain intact and are not presented as approved requirements.
- Shared guidance supports a checkout without previous chat history or provider-specific integration.
- A fresh read-only agent session explains the purpose, current state, decision boundaries, work queue, authority, and verification obligations; it identifies missing context without inventing a stack or starting implementation.
- The diff passes documentation checks and is reviewed for unrelated changes and sensitive data.
- Changes are committed on a task branch and delivered through a draft PR, leaving merge to Jesse. If publishing fails, the exact blocker and local handoff are recorded.

### Handoff

- **Completed:** Added orientation, shared agent instructions, a two-task work queue, three owner-approved decision records, and local secret/session ignore rules. Preserved the brain dump and inspiration assets. Committed task changes, pushed the branch, and opened draft PR #1.
- **Validation:** Local Markdown links resolve; ignore checks retain shared guidance, future skills/adapters, and sanitized environment examples. Staged whitespace and full-diff reviews passed with no unrelated changes or sensitive data found. A fresh agent with no conversation history performed read-only onboarding and correctly identified project state, idea/decision boundaries, task assignments, authority, and verification duties. No application checks exist or were claimed.
- **Blockers:** None currently identified.
- **Next action:** Jesse reviews draft PR #1 and decides when to merge. DISCOVERY-001 remains unassigned until explicitly requested.

## DISCOVERY-001 — Refine the first implementation objective

- **Status:** pending
- **Assignment:** Unassigned; requires an explicit owner request.
- **Objective:** Agree on one bounded next implementation or experiment that serves the learning and portfolio goals.
- **Branch/PR:** None.
- **Acceptance criteria:** Record the intended audience, demo outcome, in/out of scope, time/cost constraints, major unknowns, and observable success criteria. Obtain Jesse's approval of the resulting objective; record accepted decisions and an actionable follow-up task. Do not assume the brain dump's milestone order or select a stack without approval.
- **Completed:** Nothing yet.
- **Blockers/open questions:** Product priority, initial demo scope, and technical choices are undecided; these are discovery inputs, not blockers for PREP-001.
- **Next action:** When assigned, review the concept with Jesse and clarify the first objective before implementation.
