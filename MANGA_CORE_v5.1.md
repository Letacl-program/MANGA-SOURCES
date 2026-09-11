# MANGA CORE v5.1

**Status:** ACTIVE / CORE
**Migration:** V4.1 → V5.1 — LOSSLESS CONTENT RECOVERY

## Fundament

> **NAZWA IDENTYFIKUJE. T-POSE DEFINIUJE. CHARACTER LOCK CHRONI. TEST
> SPRAWDZA. GENEROWANIE WYKONUJE. KONTROLA WERYFIKUJE.**

## Hierarchia źródeł

1.  Aktualne zasady projektu.
2.  Właściwy aktywny T-POSE Source.
3.  Pełny odczyt T-POSE.
4.  Source Specification.
5.  Świeży Character Lock.
6.  Jawne parametry zadania/testu/sceny.
7.  Style / Layout / Presentation.
8.  Wynik generacji --- nigdy jako źródło.

Poprzednie generacje, PASS i FAIL nie są źródłem wyglądu postaci.

## Source Value ≠ Test Value

Wartość testowa nie staje się automatycznie wartością źródłową. Opisu
źródłowego nie wolno bez podstawy zamieniać na inną skalę.

## Nie zgaduj

Jeżeli krytycznej informacji nie można potwierdzić: \> **STOP → NIE
ZGADUJ → NIE GENERUJ.**

## Test nie tworzy postaci

Test nie tworzy samodzielnie nowego T-POSE, Character Lock ani źródła.

## Authorized Transformation

Każda transformacja jawnie określa parametr, zakres, kolejność, elementy
zablokowane i sposób kontroli ciągłości tożsamości. Nieautoryzowana
zmiana = FAIL.

## One Variable

Kontrolowany test zmienia jedną główną zmienną. Pozostałe pozostają
stałe, chyba że zostały jawnie objęte zakresem.

## Final Generation Consistency

Przed generowaniem potwierdzić źródło, ID postaci, Lock, parametry, brak
obcych cech i brak użycia poprzedniej generacji jako źródła. Brak
potwierdzenia = STOP.

## Krytyczny FAIL

Jedna krytyczna niezgodność = FAIL. Dobry wynik innej bramki nie może
zamaskować Identity/Anatomy FAIL.

## SOURCE-FIRST RESPONSE RULE
Before every response concerning:
- character testing,
- character generation,
- Character Lock,
- T-POSE,
- test scenes,
- PASS / FAIL evaluation,

the system MUST recheck the current project sources.

If the request concerns a specific character, the correct T-POSE source MUST also be checked and fully read.

Do not rely on previous replies, prior assumptions, remembered traits, prior generations, PASS or FAIL results when the required information is available in project sources.

If a required source cannot be located, read, or verified:
> **STOP — NIE ZGADUJ.**

Never claim that a source was checked unless the check was actually performed.

This rule applies again at the beginning of every new relevant response; it is not satisfied merely because the source was checked earlier in the conversation.

## FINAL GENERATION CONSISTENCY

The final gate must additionally confirm:
- active T-POSE matches the requested character ID,
- fresh Character Lock corresponds to that same source,
- instructions match the Lock and explicit test parameters,
- no foreign character traits,
- no traits imported from previous generations,
- no traits imported from PASS/FAIL results,
- no memory-based or stereotyped identity traits,
- no unapproved visual elements,
- no unauthorized transformation.

Failure to confirm any critical point:
> **STOP → NIE GENERUJ.**
