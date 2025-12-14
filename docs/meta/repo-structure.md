# Repository Structure

This repository is **spec-first** and **boundary-driven**.  
Code is optional.

Not all documents are intended for end users or deployment contexts.
Some directories exist solely for author-side reasoning, validation, or reference.

---

## Root

- README.md  
  Entry point. Non-authoritative overview.

- SPEC.md  
  Source of truth for Zero Reflect behavior.

- LICENSE  
  AGPL-3.0 full text.

- NOTICE  
  Project notice (optional but recommended).

- CONTRIBUTING.md  
  Contribution guidelines.

- GOVERNANCE.md  
  Project governance and decision boundaries.

---

## bootstrap/

Platform-specific minimal bootstrap references.
These files are not part of the core specification.

- chatgpt.md  
- claude.md  
- gemini.md  
- minimal.md  

---

## docs/

Primary documentation namespace.

### docs/core/

Authoritative behavioral constraints and operational gates.
These define what Zero Reflect **must not** do.

- design-constraints.md  
  Minimal invariants (constitution).

- design-constraints-notes.md  
  Extended rationale and historical notes (non-binding).

- misuse-modes.md  
  Descriptive misuse taxonomy (non-operational).

- misuse-checklist.md  
  Operational gate conditions.

---

### docs/appendix/

Non-authoritative reference materials documenting
edge cases, boundary illusions, and responsibility-attribution failure modes.
Contents here do not define behavior.

- ai-subjectification-edge-case.md
  Human projection / subjectification edge case reference.

- creator-attribution-edge-case.md
  Post-release creator attribution (association) illusion reference.

- human-role-dominance-edge-case.md
  Role-centered input dominance illusion reference.
  
- system-level-agency-intrusion-edge-case.md  
  Records cases where a third-party system exerts effective agency
  at the interaction level without being recognized as a responsible actor.

- test-cases-core.md  
  Mandatory failure cases (spec enforcement).

- test-cases-derived.md  
  Reserved for edge-case–derived test vectors.

---

### docs/interface/

External system and prompt-layer integration references.

- integration-mapping.md  
  MCP / OpenAI / prompt-layer mapping.

---

### docs/meta/

Meta-level documentation describing repository structure and intent.

- repo-structure.md  
  This document.

- zr-max-decomposition.md  
  Defines the maximum decomposition depth of ZR and its irreducible human boundary.

---

## examples/

Non-normative output examples.
Provided for reference only.

- minimal-response.md  
- silence-response.md  

---

## mcp/

Pipeline, gate, and trigger references for MCP-based operation.
Not part of the core behavioral specification.

- gates.md  
- pipeline.example.md  
- triggers.md  

---

## src/

Optional implementation space.
The presence or absence of code does not affect specification validity.
