# CHARACTER SOURCE SYSTEM v5.1
**Status:** ACTIVE / CORE
**Migration:** V4.1 → V5.1 — LOSSLESS CONTENT RECOVERY

## 1. Chain

`T-POSE CARD → FULL READ → SOURCE SPECIFICATION → CHARACTER CHECK → CHARACTER LOCK`

T-POSE is the visual master. A specific accepted concrete card is the Active T-POSE Source.

The accepted T-POSE is the only visual identity source for the concrete character. Catalogs may serve as archive/index, but do not replace the concrete source.

---

## 2. Full Read

Every selected character requires a full read before each new test or generation.

Two independent layers are mandatory:

1. **text/OCR layer,**
2. **complete visual layer.**

Text cannot replace image. Image cannot replace text.

The read covers, where applicable:

- ID,
- name,
- age,
- height,
- bust size,
- face,
- eyes,
- hair,
- ears,
- skin/surface,
- silhouette,
- proportions,
- critical anatomy,
- identity features,
- laterality,
- integral structures,
- fixed elements,
- removable elements,
- stage/outfit elements,
- surface details,
- notes.

Feature status must remain explicit:

`CONFIRMED / NOT ESTABLISHED / NOT APPLICABLE / REMOVABLE`

`NOT ESTABLISHED` is never converted into a guessed value.

If a critical feature cannot be established:

> **STOP → NIE ZGADUJ.**

---

## 3. T-POSE Card Standard

All T-POSE cards use the project master card layout.

The standard card contains the following required identity-card structure:

- **16:9 master layout,**
- **front T-pose,**
- **back T-pose,**
- **left profile,**
- **right profile,**
- **face close-up,**
- **key data,**
- **surface details,**
- **4×2 color palette,**
- **Character Lock,**
- **Anatomy & Proportions,**
- **Notes,**
- **T-POSE LOCK footer.**

These are technical source-card presentation requirements. The actual accepted card remains the visual master.

The card is not an ordinary illustration reference. It is:

> **TECHNICAL VISUAL IDENTITY CARD OF THE CHARACTER.**

---

## 4. Character Check

Character Check is mandatory before designing, generating or accepting a T-POSE.

Minimum Character Check:

```text
IDENTIFICATION
ID:
NAME:

BASIC DATA
AGE:
HEIGHT:
BUST SIZE:

APPEARANCE
FACE:
EYES:
HAIR:
SKIN / SURFACE:
SILHOUETTE:

ANATOMY
PROPORTIONS:
CRITICAL ANATOMY:
INTEGRAL ANATOMY:
LATERALITY:

ELEMENTS
FIXED:
REMOVABLE:
STAGE / OUTFIT:

UNKNOWN
NOT ESTABLISHED:
```

**Age, height and bust size are mandatory Character Check data points.**

If the source does not establish a value, record:

`NOT ESTABLISHED`

Do not infer, normalize or invent it.

Character Check must also identify unusual or integral anatomy. Unusual anatomy is preserved; it is not normalized to standard anatomy.

---

## 5. Character Lock

Character Lock is an operational protection layer.

It does not replace the T-POSE and does not become an independent source.

Character Lock protects:

- identity,
- face,
- eyes,
- hair,
- anatomy,
- proportions,
- critical anatomy,
- integral anatomy,
- laterality,
- fixed elements,
- removable elements,
- explicitly authorized transformations.

Outfit, pose, camera, style or presentation cannot silently change protected identity/anatomy.

---

## 6. Non-Normalization

Unusual anatomy must remain exactly as established by the active source.

Do not normalize:

- unusual limb structure,
- tails,
- integral appendages,
- non-standard body structures,
- unusual proportions,
- other source-defined anatomy.

Style may stylize presentation, but cannot erase or replace critical anatomy.

Outfit changes may adapt to anatomy. They never redefine anatomy or real proportions.

---

## 7. Source Updates

Critical identity/anatomy changes require an explicit T-POSE / source update.

The following never update the T-POSE automatically:

- scene continuity,
- generation results,
- PASS,
- PASS WITH ANNOTATION,
- CONDITIONAL PASS,
- FAIL,
- PASS PDF,
- previous prompts,
- previous test images.

A new accepted T-POSE becomes the new visual master only through an explicit source-update process.

---

## 8. T-POSE Acceptance

The T-POSE creation flow is:

`SOURCE MATERIAL → CHARACTER CHECK → T-POSE DESIGN → GENERATION → CONTROL → PASS → CHARACTER LOCK → CATALOG`

Only a T-POSE with PASS may enter the active T-POSE catalog.

Character Check becomes the operational basis for the Character Lock after acceptance.

---

## 9. Yurei / Layout Reference

A Yurei card may be used as a layout/reference-format example.

It is not:

- an anatomy source,
- an identity source,
- a proportion source,
- a substitute for the active T-POSE.

---

## 10. Active T-POSE Source

When a concrete T-POSE card is directly indicated and accepted, that card is the Active T-POSE Source.

A catalog may identify or index the card, but the catalog itself is not the visual source.

When a Session T-POSE Source Override is active, its explicitly indicated concrete source becomes the exclusive primary visual identity source within the declared scope.

A fresh full read is required before each new test.

---

## 11. Source Priority

For character identity:

`CURRENT PROJECT RULES → ACTIVE T-POSE → FULL READ → SOURCE SPECIFICATION → CHARACTER CHECK → FRESH CHARACTER LOCK`

Previous generations, previous PASS/FAIL, old prompts, remembered traits, stereotypes and scene descriptions are never substitutes for the active source.

---

## 12. Final Rule

> **T-POSE DEFINES. CHARACTER CHECK IDENTIFIES. CHARACTER LOCK PROTECTS. SCENE DOES NOT REDEFINE THE CHARACTER.**

**END OF DOCUMENT**
