# T-POSE PDF STANDARD

## Cel

Ten standard definiuje sposób tworzenia archiwalnych plików PDF dla wszystkich kart referencyjnych **T-POSE** w projekcie.

Standard jest uniwersalny. Dotyczy kart T-POSE niezależnie od rasy, gatunku, postaci, klasy, linii rozwojowej ani innego typu projektu.

## Zasada nadrzędna

**Oryginalna karta T-POSE jest źródłem nadrzędnym.**

PDF ma być jedynie opakowaniem/formatem archiwalnym dla dostarczonego obrazu. Grafika nie może być generowana ponownie, poprawiana ani modyfikowana podczas tworzenia PDF.

## Standard techniczny

- Format strony PDF: **A3 poziomo**
- Wymiary strony: **420 × 297 mm**
- Orientacja: **landscape**
- Obraz źródłowy: zachować w **oryginalnej rozdzielczości**
- Obraz należy osadzić w PDF **bezpośrednio**
- Nie wykonywać resamplingu
- Nie zmieniać liczby pikseli obrazu źródłowego
- Nie deformować proporcji
- Nie stosować JPEG
- Nie stosować kompresji stratnej
- Nie stosować filtrów ani automatycznej optymalizacji obrazu
- Nie zmieniać kolorów
- Nie zmieniać przezroczystości
- Nie dodawać żadnych elementów graficznych lub tekstowych, których nie było w źródłowej karcie
- Nie generować ponownie grafiki

### Ważne

**A3 jest formatem strony PDF, a nie docelową rozdzielczością obrazu.**

Dopasowanie obrazu do strony nie może oznaczać jego przeskalowania pikselowego. Obraz powinien zachować swoją natywną rozdzielczość, a jego rozmiar fizyczny na stronie należy dobrać proporcjonalnie.

## Workflow

1. Przyjmij dostarczoną kartę T-POSE jako źródło.
2. Nie edytuj i nie regeneruj obrazu.
3. Utwórz stronę PDF A3 poziomo.
4. Umieść oryginalny obraz na stronie proporcjonalnie.
5. Osadź obraz bezstratnie i bez zmiany jego danych pikselowych.
6. Nie dodawaj żadnych dodatkowych elementów.
7. Zweryfikuj wynik po utworzeniu PDF.

## Weryfikacja

Po utworzeniu PDF należy, w miarę możliwości technicznych, wyodrębnić z niego osadzony obraz i porównać go ze źródłem.

Kontrola powinna obejmować:

- rozdzielczość obrazu,
- liczbę pikseli,
- proporcje,
- dane obrazu,
- brak konwersji do JPEG,
- brak stratnej kompresji,
- brak niezamierzonego resamplingu,
- zgodność wizualną ze źródłem.

**Docelowy rezultat: obraz wyciągnięty z PDF powinien być pikselowo identyczny ze źródłem.**

Jeżeli nie można zagwarantować zachowania obrazu bez zmian, pliku nie należy oznaczać jako zgodnego z tym standardem.

## Czego nie robić

Nie:

- zwiększać rozdzielczości obrazu tylko dlatego, że strona ma format A3,
- zmniejszać rozdzielczości obrazu do „standardu A3”,
- konwertować PNG do JPEG,
- stosować stratnej kompresji,
- poprawiać jakości obrazu automatycznie,
- wyostrzać lub odszumiać obrazu,
- zmieniać kolorystyki,
- zmieniać proporcji postaci lub elementów karty,
- rekonstruować brakujących fragmentów,
- generować nowej wersji grafiki,
- dodawać tekstów, ramek, opisów lub innych elementów do gotowej karty.

## Nazewnictwo

Zalecany schemat:

`NAZWA_KARTY_A3_ORIGINAL_LOSSLESS.pdf`

Przykład:

`MAMKA_A3_ORIGINAL_LOSSLESS.pdf`

## Zastosowanie

Standard jest przeznaczony dla wszystkich kart T-POSE projektu, w tym między innymi:

- kart postaci,
- kart ras,
- kart wariantów anatomicznych,
- kart klas/linii,
- kart referencyjnych,
- kart porównawczych,

o ile źródłem jest gotowy obraz karty T-POSE.

## Krótki prompt wykonawczy

> Utwórz A3 poziomy PDF z dostarczonego obrazu karty T-POSE. Osadź oryginalny obraz bezpośrednio w PDF, bez JPEG, bez kompresji stratnej, bez resamplingu i bez jakiejkolwiek modyfikacji pikseli. Zachowaj oryginalną rozdzielczość, proporcje, kolory i przezroczystość. A3 ma być wyłącznie formatem strony PDF, a nie docelową rozdzielczością obrazu. Nie generuj ponownie ani nie edytuj grafiki. Po utworzeniu zweryfikuj, że obraz wyciągnięty z PDF jest pikselowo identyczny ze źródłem.

## Status

**STANDARD — AKTYWNY**

Ten dokument stanowi uniwersalną instrukcję tworzenia bezstratnych PDF-ów dla kart T-POSE.
