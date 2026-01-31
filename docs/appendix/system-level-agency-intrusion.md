# System-Level Agency Intrusion Edge Case

> Reference cases (mirrored from the master repository)

## Purpose
This document records an edge case where a third-party system
intervenes at the interaction level and behaves *as if it were an agent*,
despite not being recognized as a responsibility-bearing actor.

This case is documented as a **boundary reference**.
It does not propose mitigations, fixes, or behavioral rules.

---

## Scope
This edge case typically arises in environments where:
- input, control, or context flows through multiple system layers
- a background service or platform feature operates with elevated priority
- the intervention is implicit and non-obvious to the user

---

## Observed Phenomenon

### Surface Interpretation
The failure is commonly interpreted as:
- an application bug
- a configuration error
- incorrect user operation

In practice, none of these may be the primary cause.

---

## Core Structural Pattern

User Intent
↓
System-Level Input / Context Stream
↓
[Third-Party System Intervention]
↓
Intent is consumed, modified, or rerouted
↓
Application-level failure appears

Key characteristic:
- the intervening system is **not perceived as an agent**
- yet it **exerts effective agency** over the interaction

---

## Responsibility Boundary Distortion

This pattern produces a responsibility ambiguity:

- the user did not intend the altered behavior
- the application did not receive the intended input
- the intervening system is not surfaced as a responsible actor

As a result, responsibility is often misattributed
to the application or the user.

---

## Common Misinterpretations
- “The application is broken.”
- “This is a user configuration mistake.”
- “The tool should handle this case.”

These interpretations arise from **invisible system-level agency**,
not from application-level failure.

---

## Boundary Clarification
This edge case highlights that:
- systems may exert agency without being recognized as agents
- interaction failures can originate *outside* the user–application boundary
- responsibility analysis must account for **implicit system actors**

---

## Notes
Recognition of this pattern is sufficient.
No corrective action is defined.

---

## Revision History
- v0.1 — Initial documentation of system-level agency intrusion pattern
