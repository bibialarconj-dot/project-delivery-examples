# Case: CO-LAB — Local Commerce App
**Client:** IRC / Hilton Foundation
**Role:** Ops–Tech Lead / Quality & Delivery

---

## Context

CO-LAB was a digital transaction platform built to support local commerce in underserved communities. The goal was to enable real financial transactions between vendors and buyers through a mobile-first app — in a context where digital adoption was low and trust in technology was fragile.

The stakes: if the product didn't work reliably in the field from day one, users would not return.

---

## My role

I was not the developer. My job was to make sure what got built actually worked for the people it was built for — and that any gap between design and reality was caught before launch, not after.

**Specifically:**
- Translated field-level needs into end-to-end user flows and operational requirements
- Led UAT (User Acceptance Testing) with real users in context
- Managed issue tracking and coordinated prioritization with the product/engineering team
- Coordinated cross-functional iterations between field teams, product, and tech

---

## Process

### 1. User flow mapping
Before testing began, I mapped the full end-to-end flow from the user's perspective — not the system's. This included:
- Onboarding (registration, profile setup)
- Core transaction flow (listing, browsing, purchasing)
- Edge cases: failed transactions, connectivity issues, re-entry after abandonment

This gave the UAT a clear scope and made sure nothing was assumed to "just work."

### 2. UAT execution
- Recruited real users (vendors and buyers from target communities)
- Designed test scenarios based on actual usage patterns, not ideal paths
- Captured evidence: screenshots, session notes, error logs, verbal feedback
- Tagged issues by: **type** (functional / UX / data), **severity** (blocker / high / medium / low), and **operational impact** (what breaks in the real world if this isn't fixed)

### 3. Issue coordination
- Logged all findings in a structured tracker (not a shared doc — a real issue log with owner, status, and resolution date)
- Ran triage sessions with product/engineering to prioritize by operational impact, not just technical complexity
- Followed up on blockers until resolved; escalated where needed

### 4. Rollout support
- Supported field coordinators with process documentation and Q&A
- Monitored early adoption metrics to catch drop-off patterns post-launch

---

## Outcome

- **~80% of registered users became active users** — sustained engagement beyond the initial onboarding incentive period
- Zero critical blockers at launch (all resolved pre-release through UAT cycles)
- Field team had clear documentation to support users without technical escalation

---

## What this demonstrates

- UAT is not checkbox testing — it requires scenario design, evidence capture, and prioritization discipline
- Translating field reality into system requirements is a specific skill
- Cross-functional coordination (ops ↔ product ↔ tech) requires a common language and a structured handoff process
