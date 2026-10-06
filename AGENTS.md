# Agent contribution guidance

## Read and orient

Read [README.md](README.md), [docs/WORK.md](docs/WORK.md), and [docs/DECISIONS.md](docs/DECISIONS.md). Follow the assigned task's plan link, if present. Inspect the working tree and current branch before making changes.

The README describes the project; WORK owns task state; DECISIONS owns durable decisions. `BACK_OF_THE_NAPKIN.md` is exploratory, including its milestones and technical ideas. Inspiration assets are design references. Do not infer an approved roadmap or stack from either.

Follow the user's current instructions and the harness's applicable instruction hierarchy. If repository records disagree, identify the discrepancy and resolve it from explicit instructions; ask when scope or approval remains unclear. Do not silently promote a proposal to an accepted decision.

## Work on an assigned task

- A backlog item is not an assignment. Confirm the requested task and its acceptance criteria from the user's instruction and WORK; ask only for material missing information.
- Work in a dedicated task branch. Preserve unrelated changes and do not reset, discard, or include someone else's work. If another task is already active on the checkout, use an isolated worktree or ask when isolation cannot be established safely.
- For routine work, task acceptance criteria are enough. For substantial or multi-session work, create a focused plan under `docs/plans/` and link it from WORK. Include objective, approach, checks, progress, and open questions; obtain owner approval for material scope changes.
- Implement within the assigned scope. Use appropriate existing tools and conventions. Add dependencies, skills, MCP connections, or provider adapters only for a concrete task need; explain the choice.
- Record decisions that affect future work, including rationale and consequences. Mark unapproved recommendations as proposed. Accepted entries must identify the owner's approval; later changes should supersede rather than erase their history.
- Update WORK at meaningful checkpoints and before handoff. Record actual results, outstanding checks, blockers, and the next action; do not copy chat transcripts or rely on private agent memory.

## Verify and deliver

No application build or test commands exist yet. Do not invent successful checks. Add verified setup/build/test commands to project documentation when application scaffolding introduces them.

For documentation changes, check local links and paths, consistency between records, and `git diff --check`. Review the full task diff for unrelated edits and sensitive data. For code changes, run checks appropriate to the behavior changed and report anything not run and why.

Commit only task changes, push the dedicated branch, and open a **draft** PR against the repository's default branch. GitHub CLI or equivalent access is acceptable. The PR must describe the outcome, validation, and remaining limitations. Confirm the PR URL and record it in WORK. Keep a task awaiting review until the owner merges or otherwise closes it; a draft PR is not a completed release.

If publishing is blocked, finish locally as far as possible and report the exact blocker, branch, commit, and next publishing step. Do not weaken authentication or alter repository permissions to work around it.

## Authority and boundaries

An assigned task authorizes local implementation, appropriate checks, task commits, branch pushes, and draft PR creation. Owner approval is required for merges, deployment, paid resources, destructive actions, and material scope changes. Do not provision paid services or use paid generation APIs merely to validate onboarding.

Never commit credentials, personal reference media, or private session transcripts. Keep local secrets and agent settings untracked; shared project guidance must remain tracked. Ignored files are not a substitute for reviewing staged changes.

## Handoff format

In the task's WORK entry, maintain: status, acceptance criteria, branch/PR, concise completed work and validation, blockers or unresolved questions, and next action. For a successor, explain what remains actionable without requiring prior conversation access.
