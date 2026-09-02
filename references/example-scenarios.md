# Example scenarios

Short worked dialogues, one per category, showing triage → diagnosis →
intervention. Trimmed to the essentials; real conversations will be a bit
longer.

## 1. Motivation dip

> **User:** I've had "write the postmortem" on my list for four days. I know
> exactly what happened, I just haven't opened the doc.

**Triage:** Opener asked. User confirms: "don't want to, not that I don't
know how." Capacity check: "if it were the only thing on your plate right
now, would you have the energy?" — "Yeah, honestly, I just don't want to
relive it."

**Diagnosis said back:** "So it's not complexity or capacity, it's that
opening this doc feels bad. Fair?" — "Yeah."

**Intervention (A):** "Smallest possible step: open the doc, write one
sentence — just the timeline header, not the analysis. Two minutes. When
could you do that — right now, or in the next hour?"

## 2. Complexity overload

> **User:** I need to migrate the auth service and I genuinely don't know
> where to even start, there's like six systems that touch it.

**Triage:** Opener → "too many pieces." No follow-up needed, category is
clear from the answer.

**Diagnosis said back:** "Sounds like a complexity problem, not a
not-knowing-how problem — you know the pieces, there's just too many of them
live in your head at once. Fair?" — "Yeah, exactly."

**Intervention (B):** Dump all six systems into a flat list. Sort:
blocking / parallel / not-needed-for-v1. Two systems turn out to be
read-only and can migrate later. Target the smallest one that still proves
the pattern works. That becomes the actual next task.

## 3. Knowledge gap

> **User:** I keep putting off the Terraform module because every time I
> open it I just stare at it.

**Triage:** "Not knowing how, or not wanting to?" — "I genuinely don't know
Terraform, I've never used it."

**Diagnosis said back:** "That's a knowledge gap, not motivation — makes
sense the doc feels like staring at a wall." — "Right."

**Intervention (C):** Pin the actual sub-part: they need to add one resource
block to an existing module, not learn Terraform broadly. 20-minute
time-box on "how do resource blocks reference each other in this repo,"
using an existing block in the same file as the worked example, then attempt
the real addition.

## 4. Unclear outcome, self-resolvable

> **User:** I can't make myself start the onboarding doc, I don't even know
> what it's supposed to cover.

**Triage:** "If you had to write a one-sentence definition of done yourself,
could you guess?" — "...Actually yeah, probably: a new hire can set up their
dev environment without pinging anyone in week one."

**Diagnosis said back:** "So the outcome wasn't actually unclear, you just
hadn't written it down. That sentence is your done."

**Intervention (B, self-serve branch):** Definition of done recorded. First
step: list the setup commands from memory, in order, no polish yet.

## 5. Unclear outcome, escalates

> **User:** I can't start the campaign brief, I don't know if leadership
> wants this positioned as a feature or a whole new product.

**Triage:** "Could you guess and write your own definition of done?" —
"No, that's genuinely a call only the VP can make, it changes everything
about the brief."

**Diagnosis said back:** "That's not something to guess your way through —
it's a decision that lives with the VP. This is a blocked decision, not an
unclear-outcome-you-can-fix-yourself."

**Intervention (E):** Missing condition = positioning decision (feature vs.
product). Owner = VP. Draft: "Before I can draft the campaign brief I need
one decision: are we positioning this as a feature of X or a standalone
product? Blocks the brief; I can have a draft to you same day once I know."

## 6. Missing support

> **User:** I could technically figure out the payment reconciliation bug
> myself but it'd take me all week, and Priya's dealt with this exact code
> before.

**Triage:** "Waiting on someone, or could you unblock yourself given
enough time?" — "I could, eventually, it'd just be slow and painful."

**Diagnosis said back:** "That's missing support, not a blocked decision —
nobody needs to approve anything, you just need Priya's context."

**Intervention (D):** Draft: "Hey Priya — hitting a reconciliation bug in
the payments module, and I think you've debugged this exact area before.
Could I grab 20 minutes to walk through what you remember? Happy to work
around your schedule this week."

## 7. Limited capacity

> **User:** I have three back-to-back deadlines this week and now this
> urgent review landed on me too. I feel like I'm failing at all of it.

**Triage:** Capacity check first given the framing. "If this were the only
thing on your plate, would you have the energy?" — "Easily, it's not the
task, it's that there are four of these."

**Diagnosis said back:** "This isn't motivation — you're genuinely
overcommitted this week. Pretending otherwise and pushing through on all
four is what usually backfires here."

**Intervention (A, scaled + E):** Smallest real step on the review: skim it
for anything blocking, 10 minutes, today — just enough to keep the thread
alive, not to finish it. Then, since four deadlines in one week is a real
constraint: draft a note to whoever assigned the review, naming the
conflict and asking which of the four should slip, rather than silently
letting all four suffer.
