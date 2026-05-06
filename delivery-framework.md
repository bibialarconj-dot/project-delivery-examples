# Delivery Framework
**Backlog → Flow → QA → Reporting**

This is how I structure delivery operations for complex, high-volume, or cross-functional work. It's not a methodology — it's a practical system built from what actually works.

---

## The 8-step lifecycle

```
Intake → Triage → Prioritize → Assign → Produce → QA → Deliver → Retro
```

Every step has an owner, a clear output, and a handoff condition. Nothing moves to the next step without meeting the condition.

---

## 1. Intake

**Goal:** every request enters the system in a usable state.

**How:**
- Standardized intake form (not a chat message, not an email)
- Mandatory fields: goal, audience, deadline type (hard / soft), required assets, stakeholder sign-off
- Brief template for complex requests: context, constraints, definition of done

**Condition to move forward:** brief is complete and actionable. Incomplete briefs are returned, not processed.

**Why this matters:** most rework starts here. A request that enters with missing info will produce a deliverable that misses the mark — and the rework cost is always higher than the intake cost.

---

## 2. Triage

**Goal:** validate scope, flag dependencies, catch problems before they become blockers.

**How:**
- Scope check: is this one request or three?
- Missing info check: what's not in the brief that will be needed?
- Dependency check: does this require input from another team or another deliverable?
- Technical feasibility check: is what's being asked actually possible given current constraints?

**Condition to move forward:** request is fully scoped, dependencies are mapped, no missing critical information.

---

## 3. Prioritize

**Goal:** decide what gets worked on next, explicitly and visibly.

**How:**
- Scoring: business impact × urgency ÷ effort
- Hard deadlines vs. soft deadlines explicitly tagged
- WIP limits enforced — not everything can be "top priority"
- Stakeholder goals mapped against current capacity

**Output:** a ranked backlog with explicit priority rationale, not a list of everything with the same due date.

---

## Backlog structure (example)

| ID | Request | Priority | Owner | Due | Status | Dependencies | Notes |
|---|---|---|---|---|---|---|---|
| 001 | Campaign brief — Q3 launch | P1 | [Name] | June 10 | In Progress | Design assets from Brand | Waiting on logo update |
| 002 | Onboarding SOP update | P2 | [Name] | June 15 | Backlog | None | — |
| 003 | Executive deck — board meeting | P1 | [Name] | June 8 | In Review | Approved data from Finance | Final review pending |

**Status tags:** `Backlog | In Progress | In Review | Blocked | Done | Deferred`

---

## 4. Assign

**Goal:** clear ownership, clear expectations, no ambiguity.

**How:**
- Assign based on skill fit and current capacity — not whoever is available
- Define acceptance criteria before work starts (not after review)
- Map peer dependencies: if this person is blocked, who do they escalate to?
- Confirm assignment is understood (async note or quick sync — documented)

**Condition to start work:** assignee confirms they have everything needed to begin. If not, back to triage.

---

## 5. Produce

**Goal:** execution with focus, not chaos.

**How:**
- WIP limits enforced — max X concurrent items per person
- Async status updates (daily or per-cycle): not "I'm working on it" but "here's where I am and here's what I need"
- Proactive unblocking: blockers surfaced immediately, not at the deadline
- No silent "almost done" — if a deadline is at risk, it's flagged early

---

## 6. QA

**Goal:** catch problems before they reach the stakeholder.

**Master QA checklist:**

- [ ] Goal and audience are clear and reflected in the output
- [ ] Specs validated (sizes, formats, technical constraints)
- [ ] Asset integrity (all links, files, and references are complete and correct)
- [ ] Brand alignment (logo, typography, colors, tone match guidelines)
- [ ] Naming conventions applied (file names follow the standard)
- [ ] Approvals logged (who approved what, when)
- [ ] Handoff notes included (context for the next person in the chain)
- [ ] Versioning correct (V1, V2, Final — tagged and stored properly)

**Condition to deliver:** all checklist items pass. Exceptions are documented and explicitly accepted by the stakeholder.

---

## 7. Deliver

**Goal:** clean handoff, no loose ends.

**How:**
- Deliverable sent with: version label, approval record, handoff notes
- Stakeholder confirms receipt (not assumed)
- File stored in the correct location with correct naming
- Ticket / task closed with completion note

---

## 8. Retro

**Goal:** improve the system, not just finish the work.

**Cadence:** end of sprint / end of project / end of high-volume period

**Questions:**
- What slowed us down? (process problem, not people problem)
- What rework happened and where did it start?
- What decision took too long and why?
- What would we do differently next cycle?

**Output:** 1–3 specific process changes, owner assigned, implemented before next cycle.

---

## Reporting — Weekly Executive Update

Format I use for leadership visibility:

```
Week of [date]

SHIPPED
- [Deliverable 1] — [brief context]
- [Deliverable 2] — [brief context]

TOP PRIORITIES (next 5–10)
1. [Item] — Due [date] — Owner [name]
2. ...

RISKS & MITIGATION
- [Risk] → [What we're doing about it]

CAPACITY / BOTTLENECKS
- [What's constrained and why]

DECISIONS NEEDED
- [Decision 1] — needed by [date]
- [Decision 2] — needed by [date]
```

Short. Scannable. Every item is either information or a request for action. No padding.

---

## Tools I use

**Notion — Knowledge Hub / SSOT**
- Intake and brief templates
- SOPs, guidelines, decision log
- Dashboards for leadership visibility
- Single source of truth for "how we do things here"

**Jira-style execution engine (Jira, Linear, Asana — depends on team)**
- Kanban workflow tracking
- Dependency and blocker mapping
- Cycle time and throughput tracking
- Standardized checklists per ticket type

The two systems serve different purposes. Notion is where knowledge lives. The execution tool is where work moves.

---

*This framework scales from a 2-person team to a 20-person operation. The principles don't change — the tooling adapts.*
