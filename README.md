# Rekall.studio

A personal proof of concept by Jesse Flygare exploring generative AI as both a product capability and a development tool. The concept is a web app that creates imagined vacation and adventure memories using a user's likeness, inspired by Rekall Industries from *Total Recall* (1990).

The project is intended for learning and for demonstrating AI experience and software development practices to potential employers. Favor portable approaches and free or low-cost tools where practical.

## Current state

The repository contains exploratory product ideas, visual inspiration, and contribution guidance. There is no application, selected tech stack, deployment configuration, or application build/test command yet. The GitHub repository and `rekall.studio` domain have been established; purchasing the domain does not imply an application is deployed.

[BACK_OF_THE_NAPKIN.md](BACK_OF_THE_NAPKIN.md) is a brain dump, not an approved plan. Its milestones, features, and technical approaches remain ideas unless explicitly approved and recorded. Assets in [docs/inspiration/](docs/inspiration/) are design references, not requirements or production assets.

## Project map

| Document | Responsibility |
| --- | --- |
| [AGENTS.md](AGENTS.md) | Shared instructions for agents contributing to this repository. |
| [docs/WORK.md](docs/WORK.md) | Authoritative task queue, acceptance criteria, progress, and handoffs. |
| [docs/DECISIONS.md](docs/DECISIONS.md) | Accepted decisions and clearly labeled proposals, with rationale. |
| [BACK_OF_THE_NAPKIN.md](BACK_OF_THE_NAPKIN.md) | Original exploratory concept. |

Substantial or multi-session tasks use focused plans under `docs/plans/`, created when needed and linked from the work record. Plans explain execution; they do not replace the task queue or decision log.

## Start a fresh agent session

Clone the repository and open its root in your agent or IDE. Start with:

> Read AGENTS.md, follow its context links, and inspect the working tree before working on task X. If the task is unassigned or its scope is unclear, report what you found and ask for the missing assignment.

Replace `X` with a task ID from the work record and your request. A listed next task is not an automatic assignment. Repository files carry the shared context; access to earlier chats is unnecessary.

For an onboarding check without implementation:

> Read AGENTS.md and its context links. Perform a read-only onboarding check: explain the project and current state, distinguish ideas from accepted decisions, identify current and next work, summarize your authority and verification duties, and report missing context. Do not edit files, run paid services, or begin implementation.

Codex automatically discovers `AGENTS.md`; other harnesses should receive the explicit startup prompt unless their discovery behavior has been verified. See [official AGENTS.md guidance](https://learn.chatgpt.com/docs/agent-configuration/agents-md). Continue using the existing Codex setup initially, but any agent able to read files and use Git can follow this workflow.

## Tools and prerequisites

- **Local contributions:** Git, a checkout, and an agent/harness configured by the contributor. No provider subscription or agent configuration is imposed by the repository.
- **Publishing a draft PR:** GitHub access with permission to push a task branch and open a PR. GitHub CLI (`gh`) is convenient; equivalent GitHub access is acceptable. Authenticate locally, never in tracked files.
- **Shared context:** Plain Markdown and Git history. Keep private chat transcripts, credentials, and local agent settings out of commits.
- **Optional tooling:** Add skills, MCP integrations, provider-specific adapters, or orchestration only when a concrete task warrants them. Adapters should reference `AGENTS.md`, not duplicate its rules.

If GitHub credentials or network access are unavailable, complete and verify the work locally, commit task changes when possible, and report the publishing blocker, branch, commit, and remaining action. Do not claim a PR exists until confirmed.

See [AGENTS.md](AGENTS.md) for contribution and verification expectations.
