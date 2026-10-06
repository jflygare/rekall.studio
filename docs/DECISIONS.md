# Project decisions

Record durable choices that affect future contributions. This log owns decisions; [WORK.md](WORK.md) owns tasks and handoffs. The [brain dump](../BACK_OF_THE_NAPKIN.md) remains exploratory.

Each entry includes an ID, date, status (`proposed`, `accepted`, `superseded`, or `rejected`), decision, rationale, alternatives, consequences, and approval evidence when accepted. Agents may add proposals; only explicit owner approval makes them accepted. Append superseding decisions and link the older entry rather than deleting its history. Dates use Jesse's America/Denver timezone.

## D-001 — Git-tracked, portable project context

- **Date:** 2026-10-06
- **Status:** accepted
- **Decision:** Use README for orientation, AGENTS for contribution instructions, WORK for the authoritative task queue, and this log for durable decisions. Use focused plans under `docs/plans/` when substantial or multi-session work needs them.
- **Rationale:** A fresh checkout should provide sufficient shared context without previous chats, service credentials, or provider-specific memory.
- **Alternatives:** GitHub Issues as the authoritative queue; chat-only context; a larger project-management system.
- **Consequences:** Contributors update relevant records with their changes. GitHub PRs carry review; WORK carries task state. Planning files are created when needed. The original concept is preserved without becoming an approved roadmap.
- **Approval:** Jesse selected repository Markdown for work tracking and explicitly requested implementation of the portable collaboration plan on 2026-10-06.

## D-002 — Agent autonomy through draft PR

- **Date:** 2026-10-06
- **Status:** accepted
- **Decision:** An explicit task assignment authorizes agents to implement, verify, commit task changes, push a dedicated branch, and open a draft PR. Jesse retains approval of merges, deployment, paid resources, destructive actions, and material scope changes.
- **Rationale:** Enable useful autonomous contribution while retaining owner control over publication and consequential changes.
- **Alternatives:** Approval of a plan before every edit; local implementation with owner-managed publishing.
- **Consequences:** Agents preserve unrelated work, report validation and limitations, and leave a durable handoff. A draft PR means awaiting review, not merged. Missing GitHub access must be reported with a local fallback.
- **Approval:** Jesse selected autonomy through draft PR and explicitly requested implementation of the plan on 2026-10-06.

## D-003 — Minimal tooling for this checkpoint

- **Date:** 2026-10-06
- **Status:** accepted
- **Decision:** Continue with the existing Codex setup initially; use Git and GitHub CLI or equivalent access for contributions. Keep shared guidance provider-independent. Defer custom skills, MCP integrations, orchestration, and provider adapters until a concrete task requires them.
- **Rationale:** Establish continuity within a few hours without adding tools or maintenance obligations before their need is known.
- **Alternatives:** Standardize on a required provider-specific toolchain; install a broad agent integration framework immediately.
- **Consequences:** No new runtime, application stack, or paid service is selected. Other harnesses receive an explicit startup prompt if automatic instruction discovery is unverified. Needed adapters reference shared guidance rather than copy it.
- **Approval:** Jesse explicitly requested implementation of the plan on 2026-10-06, including its minimal tooling strategy.

## Open decisions

The first implementation objective, application stack, hosting, AI providers/models, generation budget, and final product roadmap remain undecided. The current log contains no proposals resolving them; future recommendations must be labeled proposed until approved.
