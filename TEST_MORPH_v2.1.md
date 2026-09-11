# TEST MORPH v2.1
**Status:** ACTIVE / MODULE
**Migration:** V4.1 → V5.1 — LOSSLESS CONTENT RECOVERY

## 1. Purpose
Controlled morphing of the same approved character. One principal parameter changes; the test never creates a new character/source.

## 2. Source hierarchy
Current project rules → correct T-POSE → full read → fresh Character Lock → single-character test rules → Authorized Transformation → layout → test parameters → generation → post-check.

## 3. Authorized Transformation
Every morph declares:
```text
AUTHORIZED TRANSFORMATION:
PARAMETER:
RANGE:
ORDER:
LOCKED ELEMENTS:
IDENTITY CONTINUITY CHECK:
```
Unauthorized change = FAIL. Authorized transformation does not itself constitute an error.

## 4. One Variable
One principal morph parameter per test. Other proportions do not change merely because a generator considers them naturally related unless explicitly included in the authorized scope.

## 5. Default series
1. Weight Morph
2. Muscle Mass Morph
3. Bust Morph
4. Hip Size Morph
5. Transformation Morph

Each is a separate test and requires a fresh Character Lock.

## 6. Weight Morph
Panels:
1. −20 kg
2. −10 kg
3. 0 kg — T-POSE BASELINE
4. +10 kg
5. +20 kg
6. +30 kg

## 7. Muscle Mass Morph
Panels:
1. −20%
2. −10%
3. 0% — T-POSE BASELINE
4. +10%
5. +20%
6. +30%

Baseline is the source-defined body state. Do not invent kilogram values not given by the source.

## 8. Bust Morph
Test scale:
A → B → C → D → E → F

Baseline comes from the actual T-POSE bust size. Never assume D.
If T-POSE says Bust A, A is baseline.

## 9. Hip Morph
T-POSE may describe hips verbally, e.g. “wide hips”, without A–F mapping.
Never assign a letter without source basis.

Test scale:
- A minimum within anatomy,
- B reduced,
- C slightly reduced,
- D test baseline,
- E slightly increased,
- F maximum within anatomy.

If source is verbal, D is a **TEST baseline only**, not a claim that T-POSE says D.
Panel D checks the actual T-POSE silhouette; A/B/C/E/F are judged by declared direction and degree of transformation.

## 10. Transformation Morph
Default continuum:
0% → 20% → 40% → 60% → 80% → 100%
0% = T-POSE baseline.
100% = explicitly defined target form.

Declare:
- starting form,
- target form,
- range,
- elements retained throughout,
- features permitted to transform.

## 11. Common presentation
Unless explicitly overridden:
- casual standing,
- full body,
- 3/4 camera,
- same camera,
- same presentation,
- neutral background,
- horizontal panorama,
- 2×3,
- 6 panels,
- numbering,
- panel labels.

## 12. Pre-Generation
SOURCE: current rules, T-POSE, full read, override if required, fresh Lock.
CHARACTER: ID, critical anatomy, proportions, FIXED, REMOVABLE.
TRANSFORMATION: parameter, range, order, baseline, locked elements, identity continuity.
PRESENTATION: style, color, camera, framing, background, format, layout, numbering, labels.
FINAL LOCK: no prior generation, foreign traits, unapproved transformation, uncontrolled Lock change; correct character tied to active source.
If any critical point cannot be confirmed:
> **STOP → NIE GENERUJ.**

## 13. Post-Generation
1. Identity
2. Character Lock
3. Anatomy
4. Limbs
5. Proportions
6. Integral anatomy/tail
7. Transformation parameter
8. Accessories
9. Emotion
10. Pose/presentation
11. Layout
12. Style

Every panel separately.

## 14. Identity Gate
Correct morph + wrong character = FAIL. Confirm face, hair, eyes, ears, critical anatomy, characteristic body elements, integral anatomy and fixed elements against active T-POSE/Lock.

## 15. Critical FAIL
Includes wrong character, Lock break, T-POSE mismatch, wrong anatomy/limb count, uncontrolled proportions, parameter outside range, unauthorized transformation, wrong baseline, wrong panel/label, wrong layout or inability to verify reliably.

## 16. After FAIL
`FAIL → NIE AKCEPTUJ → CORRECTION CHECK → SOURCE → NEW PRE-GENERATION → REGENERATION`
Previous FAIL never becomes reference.

## 17. PASS
PASS applies only to the specific result and does not create T-POSE, Character Lock or visual source.

## 18. Commands
`PRE-GENERATION CHECK / GENERUJ / KONTROL / POPRAW / PASS / FAIL / HELP`

> **T-POSE DEFINIUJE. CHARACTER LOCK CHRONI. AUTHORIZED TRANSFORMATION OKREŚLA CO WOLNO ZMIENIĆ.**
