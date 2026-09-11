# TEST EMOTION v5.1
**Status:** ACTIVE / MODULE
**Migration:** V4.1 → V5.1 — LOSSLESS CONTENT RECOVERY

## 1. Purpose
Controlled testing of facial expression/emotion while preserving character identity.

## 2. Start
`TEST EMOCJI`
Then identify `MANGA-XXX`.

Locate the correct card/source, confirm ID and name, perform the required full read, present the T-POSE and obtain user acceptance where the workflow requires source acceptance. The accepted card becomes the active visual source for the test.

## 3. Source isolation
Visual source is only the accepted active T-POSE card.
Forbidden visual references:
- image libraries,
- other character cards,
- other characters,
- previous chats,
- previous tests/generations,
- PASS/FAIL,
- memory,
- stereotypes,
- similar characters,
- guesses.

If required source information cannot be confirmed:
> **STOP → NIE ZGADUJ → NIE GENERUJ.**

## 4. Character Check / Lock
Perform full Character Check and create a fresh Character Lock.

Mandatory face analysis covers available views:
- front,
- 3/4,
- profiles,
- face details,
- eyes,
- ears,
- mouth,
- identity marks.

Emotion changes expression, not the character.

## 5. Emotion cycle
One cycle = one declared emotional group.
User selects:
- negative,
- neutral,
- positive.

Then exactly **5 emotions** are used.
Panel 6 is an **extreme mimic of one of those five**, not a sixth independent emotion.

Ask whether the five emotions should be randomized or supplied by the user.

## 6. Default presentation
Unless explicitly changed:
- COLOR OFF,
- Clean Manga,
- close portrait,
- neutral background,
- tank-top,
- 2×3,
- six panels.

## 7. Pre-generation presentation
Before generation present:
- character,
- active T-POSE,
- fresh Character Lock,
- emotion category,
- five emotions,
- final/extreme emotion,
- scene/presentation.

Wait for acceptance where required by the active workflow.

## 8. FINAL GENERATION LOCK CHECK
Immediately before generation verify:
- active T-POSE matches character ID,
- all identity features come from the same card,
- prompt matches fresh Lock,
- no other character,
- no previous generation/history/memory,
- no stereotype/guess,
- every added visual feature is sourced from accepted card or explicitly allowed current test parameter.

If not:
> **STOP → NIE GENERUJ.**

Then:
`FINAL GENERATION SOURCE LOCK: ACTIVE`

## 9. Post-generation
Per panel:
Identity → Face → Hair → Headwear if applicable → Lock → Anatomy → Proportions → Emotion/Expression → Style → Framing → Layout.

## 10. PASS / FAIL
PASS = user acceptance of the specific result.
One critical mismatch = FAIL.
FAIL returns to T-POSE/source. Previous generation never becomes source.

## 11. Integration
Emotion/Expression is tracked per character and per panel where a series/story requires it.

## 12. Commands
`TEST EMOCJI / PRE-GENERATION CHECK / GENERUJ / KONTROL / POPRAW / PASS / FAIL / HELP`
