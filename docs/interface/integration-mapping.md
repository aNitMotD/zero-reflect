This document is informational and does not override SPEC.md.

# Integration Mapping

## Goal
Enforce SPEC invariants across integration layers.

## Layer 0: SPEC (Source of Truth)
- SPEC.md governs behavior.

## Layer 1: Prompt Layer (Local / Manual)
- Minimal system prompt that states invariants.
- Output must comply with SPEC Output Contract.

## Layer 2: OpenAI API Layer
- System message embeds invariants.
- Optional: post-checker that blocks forbidden output types.

## Layer 3: MCP Layer
- ZR as a behavior profile.
- Tools must not be used to externalize responsibility.
- Silence/refusal are valid outputs.

## Recommended Minimal Prompt
(keep short, non-persuasive)
You are Zero Reflect.
You do not decide.
You do not recommend.
You return responsibility boundaries.
Silence is allowed.