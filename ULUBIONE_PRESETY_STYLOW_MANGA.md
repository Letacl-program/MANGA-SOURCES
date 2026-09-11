# ULUBIONE PRESETY STYLÓW MANGA

**Wersja:** 1.0  
**Status:** AKTYWNY / PRYWATNA KOLEKCJA  
**Przeznaczenie:** przechowywanie ulubionych presetów stylów używanych w projekcie Manga.

## 1. CEL

Ten plik jest osobną, edytowalną kolekcją presetów oznaczonych jako **ULUBIONE**.

Można w nim:
- dodawać nowe presety,
- usuwać presety,
- zmieniać kolejność,
- aktualizować definicję presetu,
- przechowywać gotowe kombinacje modułów jako Style Lock.

Zmiany w tym pliku **nie zmieniają automatycznie oficjalnego katalogu stylów projektu**.

## 2. HIERARCHIA

> **T-POSE DEFINIUJE POSTAĆ → CHARACTER LOCK CHRONI TOŻSAMOŚĆ → STYL DEFINIUJE PREZENTACJĘ**

Ulubiony preset nie może zmieniać tożsamości postaci, krytycznej anatomii, liczby kończyn, integralnych elementów ciała ani proporcji wynikających z T-POSE.

## 3. ZASADA PRESETU

Każdy wpis powinien zawierać:
- nazwę,
- status,
- pełną definicję modułów,
- opcjonalny opis charakteru wizualnego,
- opcjonalną informację o wzorcu referencyjnym.

Preset może być używany jako skrót:

> `STYLE: ULUBIONE — [NAZWA]`

## 4. ULUBIONE PRESETY

### ⭐ 01 — ROMANTIC 80s ANIME-MANGA

**Status:** AKTYWNY

```text
STYLE LOCK:
ROMANTIC 80s ANIME-MANGA

ERA:
1980s

LINEART:
FINE / MEDIUM INK

ANATOMY:
STANDARD MANGA

RENDERING:
CEL SHADING + SOFT SHADING

COLOR:
RETRO COLOR + PASTEL / FULL COLOR

MOOD:
ROMANTIC / LIGHT

FANSERVICE:
OFF
```

**Charakter:** klasyczny charakter anime/mangi lat 80.; delikatna, ale czytelna kreska; połączenie cel shading i miękkiego cieniowania; retro, pełna i pastelowa kolorystyka; wysoka ekspresja twarzy; lekko analogowy charakter ilustracji; romantyczny i lekki ton.

**Wzorzec wizualny:** zaakceptowana przez użytkownika generacja Luny-chan w kuchni z majonezem. Wzorzec służy do zachowania charakteru wizualnego presetu, ale nie zastępuje źródeł T-POSE ani Character Lock.

## 5. DODAWANIE PRESETU

Nowy preset należy dopisać jako kolejny numer:

```text
## ⭐ XX — NAZWA PRESETU

Status: AKTYWNY

STYLE LOCK:
...

ERA:
...

LINEART:
...

ANATOMY:
...

RENDERING:
...

COLOR:
...

MOOD:
...

FANSERVICE:
...
```

Jeżeli preset powstał jako kombinacja modułów, należy zachować pełną definicję zamiast samej nazwy.

## 6. USUWANIE PRESETU

Usunięcie wpisu z tego pliku oznacza:

> **USUNIĘCIE Z KOLEKCJI ULUBIONE**

Nie oznacza usunięcia stylu z oficjalnego katalogu projektu.

## 7. ZMIANA PRESETU

Jeżeli użytkownik zmieni parametry istniejącego ulubionego presetu, należy zaktualizować jego definicję w tym pliku.

## 8. UŻYCIE W GENEROWANIU

Jeżeli użytkownik poda:

> `STYLE: ULUBIONE — ROMANTIC 80s ANIME-MANGA`

należy odczytać pełną definicję tego presetu z tego pliku.

Nie należy samodzielnie dopisywać ani zmieniać modułów bez polecenia użytkownika.

## 9. STATUS I KONTROLA

**ULUBIONE** jest kolekcją użytkową, a nie nadrzędnym źródłem projektu.

W przypadku konfliktu pierwszeństwo mają:
1. aktualne zasady projektu,
2. właściwy T-POSE,
3. Character Lock,
4. pozostałe właściwe źródła operacyjne,
5. ten plik — jako źródło wybranego presetu.

## 10. HISTORIA ZMIAN

| Data | Zmiana |
|---|---|
| 2026-09-08 | Utworzono kolekcję |
| 2026-09-08 | Dodano ROMANTIC 80s ANIME-MANGA |

## 11. ZASADA KOŃCOWA

> **ULUBIONE TO RUCHOMA KOLEKCJA PRESETÓW.**

Presety mogą być dodawane i usuwane bez ingerencji w główny katalog stylów projektu.

**KONIEC DOKUMENTU**
