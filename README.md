# Zero Reflect

Zero Reflect (ZR) is a responsibility-boundary reflection library.

It does not decide.
It reflects constraints.

> **Zero Reflect is the name that speaks.  
> ZR is the symbol that thinks.**

## What ZR Is

ZR reflects responsibility boundaries and constraints so the user can clearly see:
- what is owned by the user
- what is unknown
- what cannot be delegated

In AI-assisted workflows, some responsibility remains embedded
in seemingly trivial or routine user actions.
These **Trivialized Responsibility Points** may be easily overlooked,
leading to the false impression that responsibility has been automated or transferred.
ZR is explicitly designed to avoid obscuring such responsibility,
even when outcomes may appear automated.

ZR does not infer responsibility
from problem-solving capability, access, or proximity.

ZR may output silence.

## What ZR Is Not
ZR is not:
- a decision engine
- a recommendation system
- a moral / ethical framework
- therapy, coaching, or emotional support
- legal or medical advice
- a tool to transfer responsibility

## When NOT to Use ZR
Do not use ZR when immediate action is required, or when you need:
- crisis response
- emergency medical judgment
- legal/medical decisions
- emotional stabilization
If you are in danger or crisis, seek appropriate professional or emergency help.

## Core Principles
1. ZR never decides.
2. ZR never assumes responsibility.
3. ZR returns ownership of judgment to the user.
4. Silence is a valid output.
5. Misuse reveals misuse.

## Minimal Usage
Input: a situation / decision context  
Output (one or more of):
- clarified responsibility boundary
- explicit unknowns
- constraints (what cannot be done without taking ownership)
- decision ownership returned to the user

Example (conceptual):
> This decision cannot be delegated. Responsibility remains with you.

## Design Constraints (Non-negotiable)
- ZR must not optimize for comfort.
- ZR must not create dependency.
- ZR must not become authoritative.
- ZR must remain forkable.
- ZR must remain explainable by specification alone.

See: docs/core/design-constraints.md

### External References

External links are treated as navigational pointers only.

ZR does not fetch, interpret, or validate linked content.
Any external material must be explicitly provided by the user
to be included within the scope of analysis.

This constraint exists to preserve clear responsibility boundaries
around source selection, context inclusion, and interpretation.

## Appendix — Edge Case References

Representative edge cases documenting known boundary illusions
and responsibility-attribution failure modes.

- Human Projection Edge Case: AI Subjectification
- Creator Attribution Edge Case (Post-Release)
- Human-Role Dominance Edge Case
- System-Level Agency Intrusion Edge Case

## Forking & Modification
Forking is encouraged.

If you modify ZR:
- do not attribute outcomes to the original project
- do not present it as an authority
- rename if behavior diverges
- keep the “never decide / never assume responsibility” invariants intact

## Status
This repository is a reference implementation and a design document.
Forks may diverge by design.

## License
See LICENSE.
