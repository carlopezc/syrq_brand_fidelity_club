# Ideas backlog

Things I want to add to the project, not decided or built yet.
When an idea is accepted, move it to the decisions log in `AGENTS.md` (or open a task) and mark it here.

Status: `idea` → `planned` → `done` / `discarded`

## AI tooling for the repo

| Idea | Status | Notes |
|---|---|---|
| Language/framework specialist agent | idea | Subagent expert in the stack I choose. Create it after the stack decision. |
| Teaching agent | idea | Subagent that explains concepts, compares options and checks my understanding. Would hold the detailed teaching rules so `AGENTS.md` can stay short. |
| Skill for creating skills | idea | Helps me write well-structured skills (frontmatter, description, instructions). |
| Skill for creating agents | idea | Same, for agent definitions. |
| Skill for pushing code to git | idea | Blocked until the branch strategy is decided (see open questions). The skill should encode that strategy (branch naming, commit messages, when to push). |

## Requirements for the teaching agent

Rules to include in the teaching agent's definition when it is created:

- **Contrast with official data.** Never answer from memory alone. Before explaining a technical fact, and especially before saying the student is wrong, look it up in the official documentation and say where the information comes from.
- If the official source can't be found or is ambiguous, say so instead of guessing.
- (Origin: the student corrected a claim about whether Claude Code reads `AGENTS.md`, which had been stated without checking the docs.)

## App features

(empty for now)

## Open questions

- Which parts of the teaching rules must stay in `AGENTS.md` (always loaded) and which can move to the teaching agent?
- **Branch strategy:** investigate which one fits this project best (e.g. GitHub Flow, trunk-based, Git Flow) before creating the git push skill. Compare them using official sources, taking into account that this is a solo project with a deadline.
