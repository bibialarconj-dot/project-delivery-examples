# Case: Migration Program — Matching Algorithm
**Client:** CCB / SDDE (Colombian government program)
**Role:** Ops–Tech Bridge / Validation Lead

---

## Context

This was an algorithm-based matching tool designed to improve allocation decisions for a migration assistance program. The system matched beneficiaries to services, resources, or opportunities based on a set of defined criteria — with real consequences for real people if the matching logic was wrong or inconsistent.

Sensitive context: the data involved vulnerable populations. Data governance and privacy were not optional considerations.

---

## My role

My job was to bridge the gap between what the operational team needed the system to do and what the technical team was building. I was not the data scientist or the engineer — I was the person who made sure the logic made sense in the real world, and that it was validated before it affected decisions.

**Specifically:**
- Translated operational needs into functional requirements and system logic documentation
- Designed user flows for case workers who would interact with the tool daily
- Led UAT and iterative validation cycles with real users
- Ensured alignment between data inputs, system outputs, and field execution
- Maintained attention to data governance and privacy throughout

---

## Process

### 1. Requirements translation
The operational team had clear instincts about what "good matching" looked like but couldn't express it in system terms. I facilitated structured sessions to extract:
- What inputs the algorithm needed (data fields, quality thresholds)
- What outputs case workers expected to see (match score, ranked options, reasoning)
- What edge cases and exceptions had to be handled
- What "wrong" looked like — cases the algorithm must not produce

This became a functional requirements document and a logic map — not a technical spec, but a shared reference that both ops and tech could validate against.

### 2. Data governance review
Before UAT began, I mapped the data flow:
- What data was collected, from whom, and under what consent framework
- Where data was stored and who had access
- What happened to data after a decision was made

Flagged gaps to the technical team before they became compliance issues.

### 3. UAT with case workers
- Designed test scenarios based on real allocation cases (anonymized)
- Ran sessions with actual case workers — the people who would use the tool daily
- Captured: what outputs they trusted, what confused them, where the logic felt wrong
- Documented mismatches between expected and actual outputs with severity ratings

### 4. Iteration cycles
- Prioritized fixes by impact on allocation accuracy and user trust
- Ran multiple UAT rounds until case workers could use the tool confidently without workarounds
- Documented final validation sign-off with evidence

---

## Outcome

- Improved allocation decisions: reduced inconsistency in how beneficiaries were matched to services
- Case workers adopted the tool without resistance — because they were part of the validation process
- No critical data governance issues at launch (caught and resolved during review phase)

---

## What this demonstrates

- Functional requirements work requires listening carefully to operational logic, not just writing down what people say
- UAT in sensitive contexts requires privacy awareness and careful scenario design
- Algorithm validation is not just "does it run" — it's "does the output make sense to the person responsible for the decision"
