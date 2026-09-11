# PRESENTATION SYSTEM v5.1
**Status:** ACTIVE
**Migration:** V4.1 → V5.1 — LOSSLESS CONTENT RECOVERY

## 1. Principle

Style defines presentation, not character.

Layout defines presentation structure, not character/anatomy.

PEGI defines presentation adaptation, not identity.

The presentation layer is downstream of source identity:

`T-POSE → CHARACTER LOCK → TEST/SCENE PARAMETERS → STYLE → LAYOUT → PEGI`

No presentation rule may override an upstream identity or anatomy rule.

---

## 2. Style Axes

The modular style system uses:

`ERA / LINEART / ANATOMY-STYLIZATION / RENDERING / COLOR / MOOD / FANSERVICE`

A controlled style test changes one principal axis unless the active test explicitly defines a Style Mix.

---

## 3. Style Mix Random

When `STYLE MIX RANDOM` is used:

`LOSOWANIE → STYLE LOCK`

The resulting modules must be fixed before generation.

After Style Lock:

- modules cannot be silently changed,
- presentation parameters remain fixed unless explicitly changed,
- a new randomization requires a new Style Lock.

---

## 4. Style Lock

Style Lock records:

- selected preset or module set,
- result of Style Mix Random where used,
- color mode,
- FANSERVICE state,
- explicit style restrictions,
- test variable.

A style failure requires correction/new Style Lock rather than silent style drift.

---

## 5. Style Bleed

Changing one axis must not silently change another axis.

Unexpected cross-axis changes are:

> **STYLE BLEED**

Examples:

- ERA change silently changing rendering,
- LINEART change silently changing anatomy,
- COLOR change silently changing mood,
- style change silently changing identity.

Style Bleed is a presentation/control error.

---

## 6. Identity Gate

Identity Gate precedes Style Gate.

> **DOBRY STYL + ZŁA POSTAĆ = FAIL**

Before judging style, confirm:

- correct character,
- correct T-POSE,
- correct Character Lock,
- critical anatomy,
- proportions,
- integral anatomy,
- identity features.

Style cannot normalize critical anatomy.

---

## 7. Stress Testing

Allowed stress directions include:

`REALISTIC / STYLIZED / SD / CHIBI / KEMONO / ANTHROPOMORPHIC`

and strong combinations of style axes.

Stress testing increases verification rigor.

It does not authorize:

- critical anatomy changes,
- identity changes,
- unauthorized proportion changes,
- replacement of integral anatomy.

---

## 8. Fixed Benchmark

For style comparison use the same:

- character,
- active T-POSE,
- scene,
- action,
- camera,
- framing,
- layout,
- fixed parameters.

The controlled variable should be one principal style axis unless a Style Mix is explicitly being tested.

---

## 9. Complex Frame

The more complex the frame, the more rigorous the control.

Check especially:

- hands,
- limbs,
- missing limbs,
- duplicated limbs,
- integral anatomy,
- tail,
- dorsal/ventral orientation where applicable,
- proportions,
- spatial relations,
- props,
- interactions.

A complex composition never relaxes identity/anatomy requirements.

---

## 10. Layout

Layout is an independent presentation layer.

It does not inherit previous test data automatically.

For a dedicated test:

- use the current layout template,
- use current test parameters,
- do not import previous panel structures,
- do not import previous storyboards,
- do not import previous compositions,
- do not import previous numbering.

When separate graphics are required:

`1 graphic = 1 image = 1 frame`

A multi-frame composition is permitted only when the current test/story explicitly requires it.

---

## 11. Specialist Layout Override

A specialist test may explicitly define its own layout.

Such an override controls only the presentation structure of that test.

It does not become a global layout default.

Example: a Position Test may explicitly require a horizontal panorama, 2×3, six panels, full body in each panel, neutral background, numbering and labels. Those values are parameters of the Position Test, not universal defaults for every test.

---

## 12. Layout Compliance

For any current layout verify:

- format,
- aspect/orientation,
- panel count,
- panel structure,
- framing,
- background,
- numbering,
- labels,
- separation of frames where required,
- visibility of critical anatomy.

A layout failure is not repaired by claiming the character or style is correct.

---

## 13. PEGI

PEGI is a presentation layer.

When PEGI 16 is active, apply the active PEGI protocol and its required:

- presentation adaptation,
- marking,
- content framing,
- post-generation check.

PEGI never overrides:

- T-POSE,
- Character Lock,
- source priority,
- critical anatomy,
- integral anatomy,
- reference locks,
- safety constraints.

“16” is a presentation variant, not a new character or anatomy.

---

## 14. Favorites

Favorite presets are a user collection, not a superior project source.

They may shortcut style selection.

They cannot alter:

- T-POSE identity,
- Character Lock,
- anatomy,
- real proportions,
- integral anatomy.

A favorite preset is subordinate to the current project rules and active source.

---

## 15. Series / Matrix

Style series keep fixed:

```text
CHARACTER
SCENE
POSE / ACTION
CAMERA
FRAME
LAYOUT
```

and change:

```text
ONE STYLE AXIS
```

The result matrix may record:

| Test | Variable | Identity | Anatomy | Style | Layout | Result |
|---|---|---|---|---|---|---|
| 01 | ... | PASS/FAIL | PASS/FAIL | PASS/FAIL | PASS/FAIL | PASS/FAIL |

Optional fields:

- Style Bleed,
- Context Sensitivity,
- characteristic errors,
- notes.

If Context Isolation improves a result:

> **CONTEXT SENSITIVITY DETECTED**

This does not prove a cause.

If it does not:

> **CONTEXT ISOLATION DID NOT RESOLVE**

Do not infer causality from a single trial.

---

## 16. Pre-Generation Presentation Check

Before generation confirm:

```text
[ ] current style established
[ ] STYLE LOCK established where required
[ ] one controlled style variable
[ ] color established
[ ] camera established
[ ] framing established
[ ] format established
[ ] layout established
[ ] PEGI requirements established where active
[ ] no Style Bleed
[ ] no identity/anatomy conflict
[ ] no previous generation used as source
```

If a critical presentation parameter cannot be established:

> **STOP → NIE GENERUJ.**

---

## 17. Post-Generation Presentation Gate

Check:

1. Identity Gate
2. Character Lock
3. Anatomy
4. Proportion
5. Integral Anatomy
6. Test Style Parameter
7. Style Lock
8. Style Bleed
9. Layout
10. Color
11. Camera / Framing
12. PEGI where active
13. Overall Presentation

A style PASS cannot compensate for Identity or critical Anatomy FAIL.

---

## 18. Archiving

For valuable style tests preserve:

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
STYLE RESULT
LAYOUT RESULT
FINAL PASS/FAIL
NOTES
```

---

## 19. Final Rule

> **ZMIENIAJ STYL, NIE TOŻSAMOŚĆ.**

```text
AKTUALNE ŹRÓDŁA
↓
T-POSE
↓
CHARACTER LOCK
↓
STAŁA SCENA
↓
STYLE LOCK
↓
JEDNA ZMIENNA
↓
PRE-GENERATION CHECK
↓
GENERACJA
↓
IDENTITY GATE
↓
STYLE GATE
↓
LAYOUT / PEGI GATE
↓
POST-GENERATION CHECK
↓
PASS / FAIL
```

**END OF DOCUMENT**
