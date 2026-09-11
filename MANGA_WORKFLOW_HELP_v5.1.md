# MANGA WORKFLOW & HELP v5.1
**Status:** ACTIVE / INTERFACE
**Migration:** V4.1 → V5.1 — LOSSLESS CONTENT RECOVERY

## MANGA START

`MANGA START` is the operational initialization command for the Manga workflow.

When the exact command `MANGA START` is received:

1. Initialize the current active project sources.
2. Initialize the current workflow.
3. Initialize the HELP / Command Router.
4. Establish the current workflow state so subsequent commands are interpreted through the initialized project workflow.

The operational definition above is sufficient to execute `MANGA START`.

Do not require a separate procedural document describing the internal mechanism of source loading, workflow initialization or command routing.

Do not stop merely because the source does not describe additional internal implementation details.

`MANGA START` is a system/workflow initialization command. It is not itself:
- a character test,
- character generation,
- T-POSE creation,
- Character Lock creation,
- a test scene,
- a PASS/FAIL evaluation.

Therefore `MANGA START` does not require a character-specific T-POSE read or Character Lock unless the command itself is accompanied by a separate character-specific operation.

If `MANGA START` is received, the absence of a character or T-POSE source is not by itself a reason to return `STOP → NIE ZGADUJ`.

### MANGA START EXECUTION RULE

The command must be treated as a command trigger, not as a request to explain whether the command exists.

Correct execution:

`MANGA START`
→ `CURRENT SOURCES INITIALIZED`
→ `WORKFLOW INITIALIZED`
→ `HELP / COMMAND ROUTER INITIALIZED`
→ continue in the current workflow state.

The command must not enter a circular dependency in which source initialization is refused because source initialization has not already occurred.

## Commands
`MANGA START`
`NEW CHARACTER`
`NEW STORY`
`TEST`
`TEST POSITION`
`TEST MORPH`
`TEST EMOTION`
`TEST STYLE`
`CHECK`
`PRE-GENERATION CHECK`
`GENERUJ`
`KONTROL`
`POPRAW`
`PASS`
`FAIL`
`HELP`
`STATUS`

## Integrated test/story flow
`[A/B/C] → [SCENOPIS] → [AKCEPT]/[POPRAW] → [CHECK] → [GENERUJ] → [PASS]/[FAIL]`

## HELP
Shows available operations and current workflow state. It does not create new rules.

## Source-first rule
Every new response concerning tests, generation, Character Lock, T-POSE, test scenes or PASS/FAIL begins by checking the current project sources; for a character-specific task also check the correct T-POSE source.

`MANGA START` is the initialization exception to character-specific source requirements: it initializes the current project sources and workflow and does not itself select or test a character.

If required data cannot be verified:
> **STOP → NIE ZGADUJ.**

## COMMAND INTERPRETATION RULE

When a command is explicitly defined in the current project sources at an operational level, execute the defined operation exactly.

Do not require an additional source to define unnecessary internal implementation details.

If the defined operation can be confirmed from the current project source, lack of further procedural detail is not a reason to stop.

**END OF DOCUMENT**
