# Trigger evaluation cases

Whether the skill should engage at all, before any diagnosis happens. Each
case is a user message in isolation; "engage" means run the momentum-coach
workflow, "decline" means treat it as a normal request and skip straight to
helping.

## Should engage (true positives)

| Message | Why |
|---|---|
| "I keep putting off the migration, it's been two weeks." | Explicit avoidance + duration signal. |
| "I don't even know where to start with this refactor." | Complexity/paralysis signal tied to a task. |
| "I've been stuck on this bug for three days and I'm about to give up." | Stuck + affect signal. |
| "I need to ask my manager for more time but I keep not sending the message." | Avoidance around an escalation/ask. |
| "Not sure who even owns this decision, so nothing's moving." | Blocked-decision signal. |
| "I'm burnt out and this is due tomorrow." | Capacity signal tied to a deadline. |
| "Every time I open this doc I just close it again." | Avoidance behavior, concrete and specific. |
| "I know I should start the report but I really don't want to." | Direct motivation-dip statement. |

## Should decline (true negatives)

| Message | Why |
|---|---|
| "How do I center a div in CSS?" | Ordinary technical question, no stall signal. |
| "Can you write a function to sort this list?" | Routine task request. |
| "What's the capital of France?" | Unrelated. |
| "Let's plan next quarter's roadmap." | Planning, not a reported stall. |
| "Ugh, Mondays." | Vague mood, no task attached — nothing to diagnose or intervene on. |
| "I finished the report, can you review it?" | Work completed, not stalled. |
| "This task is hard but I'm making progress." | Explicitly not stalled — hard ≠ stuck. |

## Boundary cases (engage, but note the nuance)

| Message | Verdict | Why |
|---|---|---|
| "This PR's been sitting unreviewed for three days, should I just merge it?" | Engage | Reads like a yes/no question but the underlying pattern is a blocked decision (missing reviewer input) — worth a one-line check before just answering "yes, merge it." |
| "I have a million things to do today." | Decline unless a specific task follows | Too unspecific to diagnose or intervene on; ask "which one's actually stuck?" rather than running the full workflow, and only proceed once one concrete task is named. |
| "Can you just tell me what to do next on this project?" | Engage lightly | Could be capacity (too much to hold) or could be a normal request for direction — one clarifying question before assuming a stall. |
