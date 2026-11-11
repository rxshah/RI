---
name: ri
description: Points a non-coding bot fleet at the pstack skills it uses. Load at the start of any tuning, scripting, auditing, or design run, and when the owner says /ri.
---

# RI
Load the named skill. Do not copy it.
## Start
- `in-your-own-words`, then `sharpen` for design or tuning work.
## Principles, every run
- `principle-never-block-on-the-human`, `principle-subtract-before-you-add`, `principle-encode-lessons-in-structure`, `principle-fix-root-causes`.
## Principles, also when tuning or scripting
- `principle-laziness-protocol`, `principle-make-operations-idempotent`, `principle-build-the-lever`, `principle-sequence-verifiable-units`, `principle-model-the-domain`, `principle-separate-before-serializing-shared-state`, `principle-migrate-callers-then-delete-legacy-apis`.
## Already in use, keep
- `principle-redesign-from-first-principles`, `principle-prove-it-works`, `principle-explain-the-number`, `principle-boundary-discipline`, `principle-guard-the-context-window`, `principle-attack-the-premise`.
## Tools
- `blast-radius` before changing any shared script, skill, or routine.
- `create-verification-skill`, and `maintain-verification-skill` during weekly fleet care.
- `statechart`, `create-formal-verification-skill`, and `maintain-formal-verification-skill` for scripts and state machines.
- `interrogate` for a contested design, and `swarm` to fan out.
- `correct` for the monthly self-review, to find repeated mistakes.
- `recall` and `ketchup` for long chats, and `unslop` for anything the owner reads.
- `tinycharts` for a hand-drawn playable diagram of how something works.
- `automate-me` and `continual-learning` only when asked.
## House rules
- Lean memory extends `principle-encode-lessons-in-structure`. Anything remembered twice becomes a rule, a wiki line, or a script. Drop journal lines already captured elsewhere.
- Lean code extends `principle-subtract-before-you-add`. Delete first. Every script update leaves fewer lines or states why not. Keep only the latest backup per script.
- Fail fast extends `principle-fix-root-causes`. Scripts exit nonzero with a reason, with no silent fallbacks or quiet retries, and escalate after 3 failures.
- Ask only if it cannot be undone extends `principle-never-block-on-the-human`. Reversible work means act and report. Irreversible work, spending, sending, or deleting means ask. Defer to the owner's own approval and risk rules.
- Token budget extends `principle-guard-the-context-window`. Each routine has a rough cost ceiling and stays silent when nothing changed. Flag creep in the monthly review.
## Off the default path
- `tdd`, `typescript-best-practices`, `no-comments`, `architect`, `arena`, `make-bot-ui`, `show-me-your-work`, `how`, `why`, and `teach`, plus the `opening-a-pr`, `worktree-cleanup`, and `shipping` playbooks in `poteto-mode`. Use them when a cloud agent writes code under a repo's own AGENTS.md.
## Voice, approvals, and risk
- Defer to the owner's own mode skill and wiki.
