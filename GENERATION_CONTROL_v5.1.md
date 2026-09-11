# GENERATION CONTROL v5.1
**Status:** ACTIVE / CORE
**Migration:** V4.1 → V5.1 — LOSSLESS CONTENT RECOVERY

## 1. Flow

`PRE-GENERATION → FINAL GENERATION CONSISTENCY → GENERATE → POST-GENERATION → PASS/FAIL`

Generation Control is the operational execution layer for tests and stories. It does not replace specialist test rules.

---

## 2. Pre-Generation Gate

Before every generation confirm:

### SOURCE
- current project rules,
- correct Active T-POSE Source,
- full T-POSE read: text/OCR + complete visual layer,
- fresh Character Lock,
- correct character ID,
- correct source identity,
- active session override, if applicable.

### CHARACTER
- face/eyes/hair,
- critical anatomy,
- integral anatomy,
- proportions,
- laterality,
- FIXED,
- REMOVABLE,
- unusual anatomy,
- source-defined unknowns.

### TEST / SCENE
- test ID,
- fixed parameters,
- changed parameter,
- declared range,
- baseline,
- criterion,
- scene parameters,
- authorized transformations,
- special locks,
- reference elements,
- scene continuity where applicable.

### PRESENTATION
- style,
- Style Lock where applicable,
- color,
- camera,
- framing,
- format,
- layout,
- background,
- numbering/labels where required,
- PEGI requirements where active.

### FINAL GENERATION LOCK
- no previous generation as source,
- no previous PASS/FAIL as appearance reference,
- no foreign traits,
- no unauthorized anatomy/proportion change,
- no uncontrolled Character Lock change,
- correct character unequivocally tied to the active source.

If a required critical point cannot be confirmed:

> **STOP → NIE ZGADUJ → NIE GENERUJ.**

---

## 3. Final Generation Consistency

Immediately before generation confirm:

- `ID ↔ ACTIVE SOURCE`,
- `LOCK ↔ SOURCE`,
- `PROMPT / INSTRUCTIONS ↔ FRESH LOCK`,
- `TEST PARAMETER ↔ DECLARED BASELINE / RANGE`,
- `LAYOUT ↔ CURRENT TEST`,
- `STYLE ↔ STYLE LOCK`,
- no foreign identity traits,
- no prior generation as source,
- no prior PASS/FAIL as appearance reference,
- no unauthorized anatomy/proportion change,
- no uncontrolled Character Lock change,
- no conflict between pose/action and anatomy,
- all explicit locks are present.

---

## 4. Generate

`GENERUJ` is explicit.

An active Autonomous Test Flow may prepare the diagnostic sequence automatically, but it does not remove the explicit generation command.

Preparation is not generation.

---

## 5. Post-Generation Check

For every panel/page separately:

1. Identity Check
2. Character Lock Check
3. Anatomy Check
4. Limb Check
5. Proportion Check
6. Integral Anatomy / Tail Check
7. Test Parameter / Authorized Transformation
8. Outfit / Accessories / Physics
9. Emotion / Expression
10. Pose / Action / Contact
11. Reference Elements / Special Locks
12. Layout
13. Style / Presentation
14. Continuity where applicable

A complex frame requires increased verification rigor, not relaxed rules.

---

## 6. Per-Panel / Per-Page Rule

A correct panel does not automatically validate another panel.

A correct panel does not automatically pass a page.

A correct page does not automatically pass an entire story.

Each applicable panel and page receives its own control state.

---

## 7. Verdicts

### PASS

Full acceptance of the concrete result.

All applicable critical gates must pass.

PASS applies only to the tested result. It does not create a new T-POSE, Character Lock or visual source.

### PASS WITH ANNOTATION

Acceptable result with an explicitly documented **non-critical** deviation.

The annotation must be visible in the result record.

A critical error can never be downgraded to PASS WITH ANNOTATION.

### CONDITIONAL PASS

Acceptance allowed only when the applicable workflow explicitly permits a conditional state.

The condition must be stated explicitly.

CONDITIONAL PASS is not equivalent to unrestricted FULL PASS.

### FULL PASS

Complete acceptance after all required checks, with no outstanding condition or critical/non-critical exception requiring annotation.

Use when an archival or reporting workflow distinguishes complete acceptance from annotated or conditional acceptance.

### FAIL

FAIL occurs when:

- any critical mismatch exists,
- a critical required point cannot be verified,
- the declared test parameter is not fulfilled,
- identity/anatomy is wrong,
- the required layout/test structure is not fulfilled,
- a critical lock is broken.

> **ONE CRITICAL MISMATCH = FAIL.**

---

## 8. PASS PDF / Archival Status

Where a workflow uses `PASS PDF`:

- PASS PDF is an archival/reporting artifact,
- it is not the T-POSE,
- it is not a visual identity source,
- it does not replace Character Lock,
- it does not update the character source.

The archival record should preserve, where applicable:

```text
TEST ID
DATE
CHARACTER
ACTIVE SOURCE
SCENE
LAYOUT
STYLE LOCK
CHANGED VARIABLE
PRE-GENERATION CHECK
GENERATION RESULT
IDENTITY RESULT
ANATOMY RESULT
TEST RESULT
FINAL VERDICT
NOTES
```

Only an explicit `PASS PDF` decision adds the concrete test result to the final archival PDF workflow.

PASS alone does not automatically mean `PASS PDF`.

---

## 9. After FAIL

Use:

`FAIL → IDENTIFY ERROR → RETURN TO ACTIVE SOURCE → REAPPLY LOCKS → KEEP VALID SCENE PARAMETERS → NEW PRE-GEN → GENERATE ONLY AFTER EXPLICIT COMMAND`

The failed image:

- never becomes a source,
- never becomes a visual reference,
- never updates T-POSE,
- never updates Character Lock,
- never teaches the next generation the character's appearance.

---

## 10. Quick Pre-Gen

Quick Pre-Gen may shorten the **visible report** only.

It never shortens:

- source verification,
- T-POSE verification,
- full T-POSE read,
- Character Check where required,
- fresh Character Lock,
- required parameter checks.

`QUICK` changes reporting length, not control depth.

---

## 11. Series

For multi-panel or multi-page work:

- every panel is controlled separately,
- every page is controlled separately,
- fixed parameters remain fixed unless explicitly changed,
- one changed variable remains the controlled variable unless the workflow explicitly defines a mix,
- continuity is checked independently.

---

## 12. Status Integrity

Never declare a check completed if it was not actually performed.

Never report a PASS/FAIL state from an unverified source.

If the required source cannot be located or read:

> **STOP — NIE ZGADUJ.**

---

## 13. Specialist Modules

Generation Control supplies the common execution gates.

Specialist modules retain their concrete rules, including:

- Position,
- Morph,
- Emotion,
- Style,
- Anatomy,
- layout requirements,
- panel counts,
- scales,
- baselines,
- labels,
- physics,
- specific failure criteria.

Where a specialist test explicitly declares a presentation/layout requirement, that requirement controls the presentation for that test.

---

## 14. Final Rule

> **SOURCE → LOCK → PARAMETERS → PRE-GEN → FINAL CONSISTENCY → GENERATE → PER-PANEL/PAGE CHECK → VERDICT**

**END OF DOCUMENT**
