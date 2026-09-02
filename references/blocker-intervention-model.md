# Blocker & Intervention Model

Seven reasons work stalls, mapped onto five interventions. Two of the seven
are "hybrid" categories that usually collapse into one of the other five once
a single clarifying question is asked — they're kept separate here because
they're common and easy to misdiagnose, not because they need their own
protocol.

| # | Category | What it feels like from inside | Primary intervention |
|---|---|---|---|
| 1 | Motivation dip | Know what to do, keep not doing it, task feels aversive | A — Take the next meaningful action |
| 2 | Complexity overload | Task feels too big or tangled, don't know where to start | B — Simplify the task |
| 3 | Knowledge gap | Don't know *how* to do a specific part | C — Learn in context |
| 4 | Unclear outcome (hybrid) | Can't picture what "done" looks like | B, escalating to E if only someone else can define it |
| 5 | Missing support | Solvable, but not alone — needs another person's skill or hands | D — Find help |
| 6 | Blocked decision | Waiting on an approval, input, access, or resource someone else controls | E — Escalate a missing condition |
| 7 | Limited capacity (hybrid) | Time/energy genuinely insufficient right now, not avoidance | A in scaled-down form, escalating to E if it threatens a commitment |

## Triage decision tree

Start with the opener in `SKILL.md` step 2. Route on the answer:

- **"Don't want to" / describes dread, boredom, resentment** → check capacity
  first (see below), then default to **Motivation dip**.
- **"Too many pieces / don't know where to start"** → **Complexity overload**.
- **"Don't know how to do [specific part]"** → **Knowledge gap**.
- **"Not sure what finished even looks like"** → **Unclear outcome**. Ask:
  "If you had to guess and write down a definition of done yourself, could
  you?" Yes → treat as Complexity overload (define scope, then simplify). No,
  because it genuinely depends on someone else's intent → **Blocked
  decision**, target = that person's clarification.
- **"Waiting on someone"** → ask what exactly you're waiting on. A decision,
  approval, access, or resource only they can give → **Blocked decision**.
  Their skill, review, or hands-on help, but you could theoretically unblock
  yourself with enough time → **Missing support**.
- **"No bandwidth"** → ask: "If this were the only thing on your plate the
  next hour, would you have the energy for it?" Yes → this is actually
  **Motivation dip** wearing a capacity costume; the "no bandwidth" is about
  everything else competing for attention, not this task. No, genuinely
  running on empty or overcommitted → **Limited capacity**.

If two answers still seem to apply after one follow-up, pick the one that, if
wrong, is cheaper to have gotten wrong — usually the more concrete/mechanical
one (knowledge gap, complexity) over the more emotional one (motivation) — and
say your guess out loud per SKILL.md step 3.

## Intervention protocols

### A — Take the next meaningful action (motivation dip)

1. Ask what a genuinely small first step would look like — one that takes
   under 15 minutes and requires no further decisions once started (open the
   file and write one paragraph, not "start the report").
2. If they can't shrink it themselves, shrink it for them and offer it as a
   suggestion, not an instruction.
3. Strip the step of any embedded decision ("figure out the right approach"
   is not a step; "write three bullet points of options" is).
4. Ask them to say when they'll do it — today, this hour — not "sometime."
5. Do not add encouragement beyond confirming the step is genuinely small
   enough. The smallness *is* the intervention.

Scaled-down variant for limited capacity: same shape, but the step should be
sized to genuinely spare energy (2–5 minutes), and the honest goal is "keep
the thread alive," not progress. Say that explicitly — it removes the guilt
of not doing more.

### B — Simplify the task (complexity overload / unclear outcome)

1. Get the task out of their head and into a flat list — don't organize yet,
   just capture every piece they're carrying.
2. Sort the list into: blocking everything else / can happen in parallel /
   not actually needed for a first usable result.
3. Cut ruthlessly to the smallest slice that produces something real and
   checkable — a draft, a passing test, a rough answer — even if it's not the
   final shape.
4. Name that slice as the actual next target, and set the rest aside
   explicitly (write it down somewhere so it's not being held in memory —
   that relief is part of why this works).
5. If the trigger was "unclear outcome" and they *could* self-define done,
   have them write one sentence: "Done means ___." Test it against "would a
   reasonable reviewer agree this is done?" before moving on.

### C — Learn in context (knowledge gap)

1. Pin down the exact sub-part they don't know how to do — not the whole
   domain. "I don't know Kubernetes" is rarely the real gap; "I don't know
   how to debug a CrashLoopBackOff" usually is.
2. Time-box the learning to what's needed for the next step only, not general
   study. 15–30 minutes, tied to producing the next concrete output.
3. Prefer a worked example or a person who's done it over documentation from
   first principles, if either is available — faster and lower-dread.
4. After the time-box, they attempt the step for real, even if imperfectly.
   Learning that doesn't touch the actual task within the session tends not
   to convert into action.
5. If the gap is large enough that no reasonable time-box closes it, this is
   actually **Missing support** — route there instead of open-ended study.

### D — Find help (missing support)

1. Name the specific capability or bandwidth missing — not "I need help,"
   but "I need someone who knows the deploy pipeline" or "I need a second
   pair of eyes before this goes out."
2. Identify who, specifically, given what's known about them (check the
   profile for known go-to people). If unknown, name the smallest search
   ("who last touched this file / owns this area").
3. Draft a scoped, low-friction ask: what's needed, how long it'll take them,
   and by when. A specific ask gets answered faster than "can you help."
4. Hand the draft to the user. Do not send it, do not imply it was sent.

### E — Escalate a missing condition (blocked decision / capacity threatening a commitment)

1. Name the exact missing condition in one sentence: the decision, approval,
   access, or resource that's absent — not the whole situation.
2. Name who owns that condition. If unclear, name the smallest step to find
   out who does.
3. Draft the escalation: what's blocked, what's needed, what happens if it
   stays unresolved by when (impact, not pressure — state consequences
   factually, don't manufacture urgency).
4. Hand the draft over. This is a message the user sends, never one this
   skill sends.
5. For capacity escalations specifically: the ask is usually a
   renegotiation (scope, deadline, or reassigned priority), not "please give
   me energy." Make the ask about the tradeoff, not the feeling.
