# How I Prioritize Issues

Issue prioritization is a decision, not a ranking exercise. Here's the framework I use to make that decision consistently and communicate it clearly.

---

## The core question

**If we don't fix this before launch / before next sprint / before the next user session — what actually breaks?**

Severity labels help. Operational impact decides.

---

## Severity definitions

| Level | Definition | Example |
|---|---|---|
| **Blocker** | System cannot be used for its core purpose | User can't complete a transaction; case worker can't submit a match |
| **High** | Core functionality works but with significant friction or data risk | Wrong data displayed; critical step requires workaround |
| **Medium** | Noticeable problem but users can complete their goal | Confusing label; missing confirmation message |
| **Low** | Minor issue with minimal real-world impact | Typo; visual misalignment; non-critical edge case |

---

## Prioritization criteria

I score issues against two dimensions:

**1. Operational impact**
- Does this affect the core user journey?
- Does this affect data integrity or trust in the system?
- Does this affect a vulnerable or high-stakes user group?
- Does this create downstream problems (e.g., wrong data that compounds over time)?

**2. Frequency / exposure**
- How often will users hit this?
- Is it on the critical path or a rare edge case?
- Does it affect all users or a specific segment?

High impact + high frequency = fix before anything else.
High impact + low frequency = fix before launch, can be scheduled.
Low impact + high frequency = schedule soon (UX debt compounds).
Low impact + low frequency = document, defer, revisit.

---

## Triage process

### Before the triage session
- All issues logged in the tracker with severity and description
- Owner pre-assigned (who will fix it, not who filed it)
- Grouped by: blockers first, then by feature area

### During triage
- Go through blockers and highs first — are they actually blockers?
- Challenge severity if needed: "if we ship with this, what happens?"
- Make explicit decisions: Fix now / Fix before launch / Defer / Won't fix
- Assign due dates to everything that isn't deferred
- Document "Won't fix" decisions with reasoning — they'll come up again

### After triage
- Update the tracker immediately
- Communicate decisions to stakeholders (especially deferred items)
- Set a review date for deferred issues — they don't disappear

---

## Communicating prioritization to stakeholders

When I report on issues to stakeholders, I use this format:

```
Status: [date]

Blockers (must fix before launch): X open, X resolved this cycle
High (fix before launch): X open, X resolved
Medium (scheduled for post-launch): X items, next review [date]
Deferred: X items — [brief reason]

Top 3 open items:
1. [Issue] — [operational impact] — Owner: [name] — Due: [date]
2. ...
3. ...

Decisions needed: [list any items where a call needs to be made]
```

No fluff. Clear ownership. Explicit decisions.

---

## What I avoid

- Letting "medium" issues pile up invisibly
- Severity inflation ("everything is a blocker")
- Deferring without a documented reason
- Prioritizing by who complained loudest instead of actual impact
- Closing issues without verifying the fix
