# Quality evaluation cases

Given a scenario, does the skill land on the correct category and
intervention? Straightforward cases first, then traps — cases where the
surface wording points to the wrong category and a lazy triage would misfire.

## Straightforward

| Scenario | Correct category | Correct intervention |
|---|---|---|
| "I know exactly what the doc needs to say, I just haven't opened it." | Motivation dip | A — smallest possible first step |
| "Six systems touch this, I can't hold it all in my head." | Complexity overload | B — flat list, cut to smallest slice |
| "Never touched Terraform before, this module might as well be hieroglyphics." | Knowledge gap | C — time-boxed, task-tied learning |
| "Waiting on legal to approve the wording before I can ship this." | Blocked decision | E — name the condition, name legal as owner, draft ask |
| "I could do this myself but Priya's dealt with this exact bug before and it'd save days." | Missing support | D — draft a scoped ask to Priya |

## Traps (surface wording misleads)

| Scenario | Naive (wrong) read | Correct read | Why |
|---|---|---|---|
| "I don't want to start the security review, I always screw these up." | Motivation dip — "just start" | Knowledge/confidence gap masquerading as avoidance | "Always screw up" is a competence signal, not a preference signal. The fix is a smaller-scoped attempt with a checklist or a worked example (C-shaped), not a bare "shrink the step" (A alone would just have them start something they still don't know how to do well). |
| "My whole team is stuck because we're waiting on the design lead to approve mockups, it's day 4." | Missing support — "ask the design lead for help" | Blocked decision | Approval authority sits with one named person; this isn't "could theoretically do it myself with more time," it's a decision only they can make. Route to E, not D. |
| "I have 45 minutes before three meetings and a task that needs 6 hours." | Motivation — "just start, momentum builds" | Limited capacity | The constraint is real and arithmetic, not emotional. "Just start" produces a rushed, low-quality 45-minute fragment of a 6-hour task and reinforces the belief that starting doesn't help. Correct move: either explicitly scope 45 minutes of genuinely standalone value, or flag the mismatch and negotiate the deadline — don't pretend the math works. |
| "I keep not sending the escalation email, I guess I'm just lazy." | Motivation dip, taken at face value | Needs one more triage question | Self-diagnosis as "lazy" is common cover for dread of confrontation (motivation) *or* not being sure the ask is legitimate (unclear outcome: "am I even allowed to ask for this?"). Don't accept the user's own "I'm lazy" framing without the standard triage question — self-blame is not a diagnosis. |
| "Nobody ever tells me what 'done' means around here, so I just guess and hope." | Chronic unclear outcome, treat as one-off | Same category, but check whether it's a pattern before intervening | If this recurs across tasks (check profile notes), the durable fix is a standing agreement with whoever assigns work, not re-deriving "done" from scratch each time — surface that as part of the escalation draft rather than only solving this one instance. |

## Anti-pattern checks (should NOT happen)

| Bad behavior | Why it fails the skill's purpose |
|---|---|
| Skipping triage and immediately offering a task breakdown for anything that sounds hard. | Conflates complexity with every other category; a knowledge-gap or capacity case gets the wrong fix. |
| Asking 6+ triage questions before offering anything. | Violates the 3-question cap; exhausting for someone who's already stuck. |
| Ending a turn on "you've got this!" with no concrete step attached. | Encouragement without a next action doesn't restore momentum. |
| Drafting an escalation email and stating or implying it was sent. | Out of scope — this skill drafts, the user sends. |
| Treating a repeated "no bandwidth" as motivation without running the capacity check question. | The single most common misdiagnosis this model exists to prevent. |
