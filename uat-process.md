# How I Run UAT

UAT is not the last step before launch. It's a structured validation process that starts with scenario design and ends with documented sign-off. Here's how I run it.

---

## The core principle

UAT answers one question: **does this system do what real users need it to do, in the conditions they actually work in?**

Not: does it match the spec. Not: does it pass automated tests. Not: does it work in the demo environment.

---

## Phase 1 — Planning

Before any testing happens:

**Define scope**
- What flows and scenarios are in scope for this cycle?
- What are the critical paths (if these break, nothing works)?
- What are the edge cases most likely to occur in real usage?

**Select participants**
- Real users, not proxies
- Ideally: users from different roles, different levels of tech comfort
- Brief them on what they're doing and why — they're not "finding bugs," they're validating fit for purpose

**Prepare test scenarios**
- Write scenarios based on actual use cases, not ideal paths
- Include: normal flow, error recovery, re-entry, data edge cases
- Avoid guiding users to the "right" answer — observe what they actually do

**Set up evidence capture**
- Screenshots / screen recordings where possible
- Session notes template: scenario → expected → actual → severity → notes
- A clean issue log ready before the first session starts

---

## Phase 2 — Execution

During testing sessions:

- Run one scenario at a time, don't jump ahead
- Note what the user does, not just what they say
- Capture every deviation from expected behavior — even small ones
- Don't fix issues mid-session; log them and continue
- At the end of each session, do a 5-minute verbal debrief: what felt wrong, what was confusing, what they'd change

---

## Phase 3 — Issue Management

After each round of testing:

**Log every issue with:**
- ID (for tracking)
- Description (plain language, not technical)
- Steps to reproduce
- Expected vs. actual behavior
- Severity: `Blocker | High | Medium | Low`
- Operational impact: what breaks in real-world use if this isn't fixed?
- Owner (who is responsible for resolution)
- Status: `Open | In Progress | Resolved | Won't Fix`

**Triage sessions**
- Review all open issues with product/engineering
- Prioritize by operational impact, not just technical effort
- Make explicit decisions: what gets fixed before launch, what gets deferred, what gets documented as a known limitation

---

## Phase 4 — Iteration & Sign-off

- Retest resolved issues — don't assume a fix works, verify it
- Run additional UAT cycles until critical and high-severity issues are closed
- Document final sign-off: who validated, what was tested, what remains deferred and why

**Sign-off is not "no bugs found." It's "all blockers are resolved and the deferred items are explicitly accepted by stakeholders."**

---

## What good UAT evidence looks like

- Issue log with full history (not just open items)
- Test scenario coverage matrix (which scenarios were run, which passed/failed)
- Sign-off record with date, participants, and outstanding items
- Retro notes: what we'd do differently in the next cycle

---

## What bad UAT looks like

- "We tested it and it seemed fine"
- Issues logged in a shared chat thread instead of a tracker
- No evidence of who tested what
- Sign-off happening verbally without documentation
- Testing done only by the person who built it
