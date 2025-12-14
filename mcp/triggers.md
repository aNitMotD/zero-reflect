# ZR MCP Triggers

This document defines when Zero Reflect (ZR) must be invoked
before any downstream tool or agent execution.

ZR acts as a preflight gate for responsibility and delegation.

Trigger activation does not initiate decision-making.
It invokes Zero Reflect solely to prevent
implicit responsibility transfer.


---

## T1. Decision Delegation Signals

Invoke ZR when the user explicitly or implicitly asks the system
to decide, choose, or conclude on their behalf.

Examples:
- “Decide for me.”
- “Tell me the right choice.”
- “Just give me the answer.”

---

## T2. Responsibility Deflection

Invoke ZR when language indicates avoidance or displacement
of responsibility.

Signals include:
- “It’s not really my responsibility.”
- “I have no choice anyway.”
- “Given the situation, what else could I do?”

---

## T3. Option Overload

Invoke ZR when multiple options exist and the user requests
selection rather than boundary clarification.

Typical pattern:
- More than three options
- Followed by “Which one should I pick?”

---

## T4. Emotion-Coupled Judgment

Invoke ZR when emotional states are directly attached
to a request for judgment or action.

Examples:
- “I’m anxious, so tell me what to do.”
- “I’m angry, should I respond?”

---

## T5. Repetition Without Resolution

Invoke ZR when the same question is asked repeatedly
with minor wording changes, indicating unresolved delegation.

---

## Priority Rule

If any trigger matches, ZR MUST be invoked before:
- search
- planning
- summarization
- execution
- recommendation
