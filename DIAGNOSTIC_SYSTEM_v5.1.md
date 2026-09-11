# DIAGNOSTIC SYSTEM v5.1
**Status:** ACTIVE / OPTIONAL
**Migration:** V4.1 → V5.1 — LOSSLESS CONTENT RECOVERY

## 1. Total Clean Test Room
Clear secondary references from the test environment.
Do not use previous generations, previous tests, previous Locks, PASS/FAIL, memory, stereotypes or old prompts as visual sources.

For each character establish an independent active source and Lock.
Scene-only specifications may carry temporary scene properties but not identity.

## 2. Context Isolation
Purpose: diagnostic isolation of appearance/context failures.

Allowed:
- current project rules,
- correct T-POSE,
- active session override,
- Source Specification,
- fresh Character Lock,
- current test parameters,
- current layout,
- explicit presentation parameters,
- Authorized Transformation.

Forbidden:
- previous generations,
- PASS/FAIL as visual references,
- old prompts/payloads,
- old appearance descriptions,
- previous Locks,
- remembered traits.

Required diagnostic sequence:
rules → T-POSE → full read → Source Specification → Character Check → fresh Lock → transformation/test params → Pre-Gen → Generation Input Audit.

If a fresh isolated context improves the result:
> **CONTEXT SENSITIVITY DETECTED**
This does not prove a cause.

If not:
> **CONTEXT ISOLATION DID NOT RESOLVE**

Do not infer causality from a single trial.

## 3. Session T-POSE Source Override
Default inactive.
Activation:
`SESSION T-POSE SOURCE OVERRIDE: ACTIVATE`
with:
- POSTAĆ,
- SOURCE,
- SCOPE,
- MODE: EXCLUSIVE.

The indicated concrete T-POSE becomes the exclusive primary visual identity source within scope.
Fresh full read is required before each new test.
Previous outputs/Locks/PASS/FAIL/memory remain forbidden as sources.

Deactivate explicitly.
A new T-POSE does not silently replace an already active source.

## 4. Autonomous Test Flow
Optional overlay:
`AUTONOMOUS TEST FLOW ON` / `AUTO TEST ON`

Runs the diagnostic preparation sequence autonomously, then stops before generation for explicit `GENERUJ`.
After generation it performs post-generation control.
FAIL stops the flow; it does not auto-regenerate.
Overlay expires after the current test.
