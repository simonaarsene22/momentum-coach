# momentum-coach

An Agent Skill that helps identify why a piece of work has stalled and picks
the right intervention, instead of defaulting to generic encouragement or a
task breakdown for every situation.

It distinguishes between seven causes — motivation, complexity, knowledge
gaps, unclear outcomes, missing support, blocked decisions, and limited
capacity — and routes each to one of five moves: simplify the task, learn in
context, find help, escalate a missing condition, or take the next
meaningful action.

## Layout

- [`SKILL.md`](SKILL.md) — trigger conditions, workflow, and guardrails.
- [`references/blocker-intervention-model.md`](references/blocker-intervention-model.md) —
  the full diagnostic model, triage decision tree, and intervention
  protocols.
- [`references/example-scenarios.md`](references/example-scenarios.md) —
  worked dialogues, one per category.
- [`references/profile-template.md`](references/profile-template.md) — an
  optional, local-only profile for personalizing tone and defaults; a filled
  copy (`references/profile.md`) is gitignored since it's personal data, not
  shared skill content.
- [`evaluations/trigger-cases.md`](evaluations/trigger-cases.md) — when the
  skill should and shouldn't engage.
- [`evaluations/quality-cases.md`](evaluations/quality-cases.md) — correct
  diagnosis cases plus traps where the obvious read is wrong.

## Scope

Produces conversation, diagnosis, and drafted text (a message to send, a
scoped-down plan, a definition of done). It does not send messages, book
calendar time, or take any action on the user's behalf — anything that
leaves the conversation is handed over for the user to send themselves.

## Install

Copy (or clone) this folder into your agent's skills directory, keeping the
folder name `momentum-coach`.

## Status

Initial draft, open for review — trigger logic, category boundaries, and the
eval cases in particular are worth pressure-testing before relying on it.

## License

[MIT](LICENSE)
