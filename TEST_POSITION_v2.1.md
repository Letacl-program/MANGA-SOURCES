# TEST POSITION v2.1
**Status:** ACTIVE / MODULE
**Purpose:** lossless operational migration of the v1.0 position test into the Universal Test Engine.

## 1. PURPOSE
Checks whether the same approved character preserves identity, anatomy and proportions across different positions.

Dynamic pose never excuses anatomical error.

## 2. SOURCE ORDER
1. Current project sources.
2. Correct T-POSE for the tested character.
3. Full T-POSE read.
4. Fresh Character Lock.
5. Applicable test/layout sources.
6. Explicit test parameters.

If the correct T-POSE cannot be confirmed:
> **STOP → NIE ZGADUJ → NIE GENERUJ.**

Previous generations, PASS and FAIL are never visual sources.

## 3. START CONDITION
Only an approved T-POSE may enter the test.
Confirm ID, T-POSE status, critical anatomy, proportions, FIXED and REMOVABLE.

## 4. TEST POOL
Default pool: 10 positions.
Select 5 positions.
Panel 6 is an extreme version of one selected position, not an independent sixth position.

Preferred classes:
1. neutral/standing where anatomy permits,
2. low/compressed,
3. lying,
4. leaning/reaching,
5. asymmetrical support,
6. twist,
7. dynamic displacement,
8. strong compression,
9. ground contact,
10. high torsional load.

Selection is a test of behavioral/anatomical range, not only illustration appeal.

## 5. DEFAULT SIX-PANEL STRUCTURE
- 2×3
- full body in every panel
- neutral background
- horizontal panorama
- panel numbering
- panel labels

Example labels from the legacy protocol:
1 — LYING ON SIDE
2 — DEEP LOW COIL
3 — FORWARD LEAN / REACHING
4 — ASYMMETRICAL SUPPORT
5 — DYNAMIC TWIST / ARM REACH
6 — EXTREME DYNAMIC TWIST

Actual labels must follow the actual selection.

## 6. EMOTION
Emotion is position-dependent in this test.
Each panel receives an emotion logically compatible with the pose and situation.
Emotion must not alter Character Lock or critical facial identity.

## 7. ACCESSORIES
Distinguish FIXED from REMOVABLE.
All required REMOVABLE elements listed by the active T-POSE must be handled consistently.

Accessory physics checks:
- gravity,
- hanging,
- displacement,
- pressure,
- rotation,
- body contact,
- contact with integral anatomy,
- material behavior,
- movement response.

Accessories may move with the pose but may not change FIXED/REMOVABLE status, become anatomy, disappear without cause, or transfer to another character.

## 8. OUTFIT
Outfit is presentation.
It may respond to pose, gravity, occlusion and body contact.
It must not alter real anatomy.
If opaque material is required, it must remain fully opaque.

## 9. CRITICAL ANATOMY
Check, as applicable:
- eyes,
- arms,
- hands,
- legs,
- extra limbs,
- tails,
- wings,
- horns,
- ears,
- other integral anatomy,
- connections between anatomical elements.

Unusual anatomy must not be normalized.

## 10. LIMB CHECK
For every panel:
- correct limb count,
- correct hand count,
- no extra hand/arm,
- no missing required limb,
- no duplication caused by twisting,
- no incorrect limb connection/assignment.

Panel 6 receives especially strict control.

## 11. PROPORTION CHECK
Check silhouette, humanoid and integral proportions, lengths, widths, T-POSE measurements and characteristic relationships.
Camera, style and outfit do not change real proportions.

## 12. INTEGRAL ANATOMY / TAIL CHECK
Where applicable:
- connection,
- continuity,
- thickness,
- direction,
- taper,
- tip,
- cross-section,
- dorsal/ventral,
- compression behavior,
- twist behavior,
- ground-contact behavior.

The generator must not replace integral anatomy with standard anatomy.

## 13. PRE-GENERATION CHECK
Confirm:
- current sources,
- correct T-POSE,
- full read,
- fresh Character Lock,
- correct character,
- critical anatomy,
- proportions,
- FIXED,
- REMOVABLE,
- 5 selected positions,
- panel 6 extreme,
- emotion assignment,
- accessories,
- accessory physics,
- style/color,
- framing/full body,
- background,
- format/layout,
- numbering/labels.

### FINAL GENERATION CONSISTENCY
Confirm:
- no previous generation as source,
- no foreign traits,
- no unapproved elements,
- no pose/anatomy conflict,
- no uncontrolled Character Lock change.

Unconfirmed critical point:
> **STOP → NIE GENERUJ.**

## 14. REQUISITES
A prop is allowed only when it helps execute the pose, does not block critical anatomy, does not change identity, and does not introduce an unjustified scene element.

## 15. POST-GENERATION CHECK
Per panel:
1. Identity
2. Character Lock
3. Anatomy
4. Limbs
5. Proportions
6. Integral anatomy/tail
7. Accessories
8. Accessory physics
9. Emotion
10. Pose
11. Layout
12. Style/presentation

## 16. FAIL
One critical mismatch = FAIL.
Critical examples:
identity, Lock/T-POSE, critical anatomy, proportions, limb count, integral anatomy, normalization, FIXED/REMOVABLE error, missing required removable element, wrong pose, missing panel-6 extreme, wrong layout, missing full body where required, or inability to verify reliably.

## 17. CORRECTION
**FAIL → DO NOT ACCEPT → RETURN TO T-POSE → CORRECT → NEW PRE-GENERATION CHECK → NEW GENERATION**

The previous FAIL is not a reference and cannot modify T-POSE or Character Lock.

## 18. PASS
PASS applies only to the specific test result.
It does not create a new T-POSE, Character Lock or visual source.

## 19. COMMANDS
`TEST POSITION`
`LOSuj`
`PRE-GENERATION CHECK`
`GENERUJ`
`KONTROL`
`POPRAW`
`PASS`
`FAIL`
`HELP`

## 20. FINAL RULE
**T-POSE DEFINIUJE. CHARACTER LOCK CHRONI. POZYCJA TESTUJE. GENEROWANIE WYKONUJE. KONTROLA WERYFIKUJE.**
