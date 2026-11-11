# RI

RI is the skill a non-coding bot fleet loads for tuning, scripting, auditing, and design. It points at [pstack](https://github.com/cursor/plugins/tree/main/pstack) skills by name. pstack stays installed.

pstack is built for software teams. This fleet tunes, scripts, audits, and designs. The full plugin costs tokens in skill selection and adds noise. RI keeps the skills this fleet uses and includes [continual-learning](https://github.com/cursor/plugins/tree/main/continual-learning). It points at [tinycharts](https://april-zhu.com/tinycharts) and adds five house rules.

## Install

Do these four steps.

1. Copy `skills/ri` and `skills/continual-learning` into the agent's skills folder.
2. Copy `agents/agents-memory-updater.md` into the agent's agents folder.
3. Install the pstack plugin.
4. Install the tinycharts skill from its author. Keep that kit out of this repo.

## What is in

Each row names a choice and the reason for it.

| Names | Place | Reason |
| --- | --- | --- |
| `in-your-own-words`, `sharpen` | In | Use these at the start of a run. Use `sharpen` for design or tuning. |
| `principle-never-block-on-the-human`, `principle-subtract-before-you-add`, `principle-encode-lessons-in-structure`, `principle-fix-root-causes` | In | Use these on every run. |
| `principle-laziness-protocol`, `principle-make-operations-idempotent`, `principle-build-the-lever`, `principle-sequence-verifiable-units`, `principle-model-the-domain`, `principle-separate-before-serializing-shared-state`, `principle-migrate-callers-then-delete-legacy-apis` | In | Use these when the run tunes or scripts. |
| `principle-redesign-from-first-principles`, `principle-prove-it-works`, `principle-explain-the-number`, `principle-boundary-discipline`, `principle-guard-the-context-window`, `principle-attack-the-premise` | In | The fleet already uses these. |
| `blast-radius` | In | Run it before a change to a shared script, skill, or routine. |
| `create-verification-skill`, `maintain-verification-skill` | In | Run `maintain-verification-skill` during weekly fleet care. |
| `statechart`, `create-formal-verification-skill`, `maintain-formal-verification-skill` | In | Use these for scripts and state machines. |
| `interrogate` | In | Use it when a design is contested. |
| `swarm` | In | Use it to fan work out. |
| `correct` | In | Use it in the monthly self-review to find repeated mistakes. |
| `recall`, `ketchup` | In | Use these for a long chat. |
| `unslop` | In | Use it on text the owner reads. |
| `tinycharts` | In | Use it for a hand-drawn playable diagram of how something works. Install it from its author. Its license forbids redistribution, so this repo does not carry the kit. |
| `automate-me` | On request | Load it only when asked. It stays in pstack. |
| `continual-learning` | On request | Load it only when asked. The skill and `agents-memory-updater` are in this repo. |
| Lean memory | In | Extends `principle-encode-lessons-in-structure`. Anything remembered twice becomes a rule, a wiki line, or a script. Drop journal lines already captured elsewhere. |
| Lean code | In | Extends `principle-subtract-before-you-add`. Delete first. A script update leaves fewer lines or states why not, and only the latest backup stays. |
| Fail fast | In | Extends `principle-fix-root-causes`. A script exits nonzero with a reason, uses no silent fallback or quiet retry, and escalates after 3 failures. |
| Ask only if it cannot be undone | In | Extends `principle-never-block-on-the-human`. Act when the work is reversible. Ask before spending, sending, or deleting. |
| Token budget | In | Extends `principle-guard-the-context-window`. Each routine has a cost ceiling, stays silent when nothing changed, and flags creep in the monthly review. |
| `tdd`, `typescript-best-practices`, `no-comments`, `architect`, `arena`, `make-bot-ui`, `show-me-your-work`, `how`, `why`, `teach` | Off the default path | Use these when a cloud agent writes code under a repo's own AGENTS.md. |
| `opening-a-pr`, `worktree-cleanup`, `shipping` | Off the default path | Use these `poteto-mode` playbooks when a cloud agent writes code under a repo's own AGENTS.md. |

## Contributing

Changes go through pull requests and are reviewed automatically before merge.
