# ZR MCP Gates

This document defines post-ZR gating rules.
ZR output determines whether downstream tools may execute.

ZR silence or refusal is treated as a valid stop condition.

ZR gating does not imply automation.
Passing a gate does not transfer responsibility
from the user to the system.


---

## G1. Delegation Detected

Condition:
- zr.delegation_attempt == true

Action:
- Block all downstream tool execution
- Return responsibility to the user
- End the pipeline

---

## G2. Silence Response

Condition:
- zr.silence == true

Action:
- Do not call any further tools
- Do not attempt recovery or clarification
- End the pipeline

---

## G3. Boundary-Only Return

Condition:
- ZR returns boundaries without ownership acceptance

Action:
- Pause execution
- Await explicit user acknowledgment
- Do not auto-continue

---

## G4. Recurrent Delegation After ZR

Condition:
- Post-ZR user input reintroduces
  “should / must / best choice” language

Action:
- Reinvoke ZR
- Reset downstream execution state

---

## G5. Explicit Ownership Acceptance

Condition:
- User explicitly states ownership
  (e.g., “I will decide”, “I take responsibility”)

Action:
- Allow downstream tools to execute
- Pass ZR boundaries as constraints
