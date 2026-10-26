# Zasady generowania promptów anatomii i kart technicznych

**Status:** OBOWIĄZUJĄCA ZASADA ROBOCZA  
**Ścieżka:** `test/PROMPT_ANATOMY_AND_MANNEQUIN_TPOSE.md`  
**Zakres:** Elara / testy spójności anatomii / generowanie ilustracji Cartoon / karty techniczne

## 1. Zasada nadrzędna

Przy każdym generowaniu lub poprawianiu ilustracji Elary należy jawnie korzystać z parametrów i zasad z dokumentacji źródłowej. To obowiązuje domyślnie, bez potrzeby ponownego przypominania przez użytkownika.

Hierarchia źródeł:
1. `char/Elara/ELARA.md` — kanoniczna tożsamość, Character Lock, ustalone cechy i zatwierdzone estymaty wymiarów.
2. **Karta Manekin T-POSE** — nadrzędny wzorzec wizualno-anatomiczny i układ proporcji.
3. Techniczny T-POSE — szczegółowe wymiary i proporcje, interpretowane zgodnie z dwoma wyższymi źródłami.
4. Wizualna karta T-POSE — wygląd, kolory i detale.

Jeżeli źródła wydają się sprzeczne, nie zmieniaj ich po cichu. Wskaż konflikt i poproś o decyzję, gdy rozstrzygnięcie jest konieczne.

## 2. Dane referencyjne Elary

Poniższe liczby to **szacunkowe wartości projektu odczytane z zaakceptowanej ilustracji**, przeskalowane według wzrostu 170 cm i zaokrąglone do 5 cm. Nie są pomiarami fizycznymi.

### Główne proporcje
- Wzrost bez rogów: **170 cm**.
- Wzrost do czubków rogów: **185 cm**.
- Wysokość oczu: **160 cm**.
- Długość/głębokość głowy: **25 cm**.
- Długość tułowia: **65 cm**.
- Długość nóg: **80 cm**.
- Długość ogona: **75 cm**.
- Rozstaw czubków rogów: **35 cm**.
- Szerokość barków: **45 cm**.
- Szerokość bioder: **60 cm**.
- Głębokość klatki piersiowej: **50 cm**.

### Obwody referencyjne
- Głowa: **55 cm**.
- Szyja: **35 cm**.
- Biust: **130 cm**.
- Talia: **85 cm**.
- Biodra: **120 cm**.
- Udo w górnej części: **70 cm**.
- Łydka: **45 cm**.
- Kostka: **30 cm**.

### Cechy anatomiczne
- Dwa gładkie, kości słoniowej, łagodnie zakrzywione rogi; wysokość około **15 cm**, szerokość podstawy około **6 cm**.
- Szerokie bydlęce uszy z różowym wnętrzem; długość około **18 cm**, wysokość około **12 cm**. Bez ludzkich małżowin usznych.
- Długi brązowy ogon zakończony ciemniejszą, puszystą kitą; kokarda ogona około **25 cm**.
- Ciemne rozszczepione kopyta; widok z przodu około **10 cm szerokości × 8 cm wysokości**, widok z boku około **12 cm długości × 8 cm wysokości**.
- Skóra jasna, kremowa; włosy długie, falowane, kasztanowobrązowe, jaśniejsze złoto-blond pasma przy twarzy i ku końcom.
- Duże niebieskie oczy, zaokrąglona twarz.
- Wyraźnie krągła sylwetka, szerokie biodra, grube uda, miękko wcięta talia, łagodnie zaokrąglony brzuch oraz **bardzo duży, ciężki biust**.
- Nie dodawaj pełnego futra na ciele — jego występowanie nie jest ustalone.
- Dłonie pozostają humanoidalne.

## 3. Jak budować prompt do ilustracji

Każdy prompt powinien zawierać wszystkie poniższe warstwy:

1. **Tożsamość i Character Lock:** dorosła postać Elary jako bovine Beastfolk, stałe cechy głowy, włosów, rogów, uszu, ogona, kopyt i skóry.
2. **Stałe proporcje:** wpisz najważniejsze wartości liczbowe, zwłaszcza 170 cm bez rogów, biust 130 cm, talia 85 cm, biodra 120 cm, szerokość barków 45 cm i szerokość bioder 60 cm. Wymień pełną tabelę, gdy test dotyczy dokładniejszej kontroli anatomii.
3. **Wzorzec obrazkowy:** jawnie wskaż Kartę Manekin T-POSE jako nadrzędny wzorzec proporcji i sylwetki, a `ELARA.md` jako źródło tożsamości i parametrów.
4. **Zadanie panelu:** określ jedną pozę, emocję, strój, styl, tło i kadr.
5. **Ochrona anatomii:** zmiana pozy, perspektywy, emocji, ubrania, oświetlenia lub stylu nie może zmieniać proporcji bazowych.
6. **Kontrola kompozycji:** pełna postać od rogów po kopyta, kończyny nieucięte, czytelne dłonie/kopyta/ogon, bez nadmiernego skrótu perspektywicznego, chyba że jest on celowo testowany.
7. **Negatywne ograniczenia:** nie zmniejszaj ani nie powiększaj biustu względem wzorca; nie zwężaj bioder ani ud; nie wydłużaj lub skracaj tułowia/nóg dla dopasowania do pozy; nie dodawaj ludzkich uszu ani pełnego futra; nie zmieniaj liczby i rodzaju kończyn.
8. **Format:** dla pojedynczych testów używaj jednego pionowego panelu z pełną sylwetką. Planszę wielopanelową stosuj tylko wtedy, gdy została wyraźnie zamówiona.

### Szablon promptu

> Użyj `char/Elara/ELARA.md` oraz Karty Manekin T-POSE jako obowiązujących źródeł. Zachowaj Character Lock i stałe proporcje Elary. Wzrost bez rogów 170 cm; wzrost do czubków rogów 185 cm; biust 130 cm; talia 85 cm; biodra 120 cm; szerokość barków 45 cm; szerokość bioder 60 cm; tułów 65 cm; nogi 80 cm; ogon 75 cm. To są estymaty projektowe, nie pomiary fizyczne. Zachowaj bardzo duży, ciężki biust, szerokie biodra, grube uda, miękką talię i zaokrąglony brzuch zgodnie z kartą. Zachowaj dwa rogi, bydlęce uszy bez ludzkich uszu, ogon z puszystą kitą, ciemne rozszczepione kopyta, niebieskie oczy i długie falowane kasztanowe włosy z jaśniejszymi pasmami. Nie dodawaj pełnego futra. Wykonaj [poza] w stylu [styl], z emocją [emocja], w stroju [strój], na prostym tle. Pokaż pełną postać w pionowym kadrze od rogów po kopyta. Poza i perspektywa nie mogą zmieniać bazowej anatomii ani proporcji.

## 4. Generowanie technicznej karty / manekina

Gdy celem jest test proporcji lub baza techniczna, nie zastępuj karty technicznej zwykłą ilustracją sceniczną.

Wymagany rezultat:
- Jeden arkusz techniczny o czystym, neutralnym tle.
- Widok z przodu, z boku i z tyłu w tej samej skali; najlepiej neutralna pozycja A/T-pose.
- Cała sylwetka widoczna w każdym widoku.
- Siatka powierzchniowa lub linie przekrojów na nieprzezroczystym, neutralnym manekinie/stroju technicznym.
- Punkty odniesienia i linie wymiarowe, opisane jednostkami.
- Zbliżenia elementów charakterystycznych: głowa, rogi, uszy, ogon, kopyta.
- Tabela wymiarów zgodna z `ELARA.md` i kartą techniczną.
- Wymiary oznacz jako „szacunki projektowe”, nie jako pomiary anatomiczne.
- Nie pozwól, by podpisy lub grafika pomiarowa zasłaniały sylwetkę.
- W razie konfliktu między wygenerowaną planszą a źródłem, pierwszeństwo ma hierarchia źródeł z sekcji 1.

## 5. Kontrola po wygenerowaniu

Po wygenerowaniu sprawdzaj:
- Czy biust nadal odpowiada opisowi „bardzo duży, ciężki” i estymacie 130 cm?
- Czy talia, brzuch, biodra i uda zachowują ustalony typ sylwetki?
- Czy tułów i nogi nie zmieniają pozornie długości w sposób wynikający z błędu rysunku (odróżniaj to od normalnego skrótu perspektywicznego)?
- Czy rogi, uszy, ogon, kopyta i dłonie są prawidłowe?
- Czy pokazano całą postać i czy kończyny nie są przypadkowo ukryte lub ucięte?
- Czy ubranie jest zgodne z zamówionym wariantem?
- Czy styl zmienił jedynie prezentację, a nie anatomię?

Status wyniku:
- `PASS` — rezultat zgodny z ustalonym wzorcem w ocenianym zakresie.
- `PARTIAL` — podstawowa tożsamość jest zachowana, ale część kryteriów pozostaje nieczytelna lub wymaga korekty.
- `FAIL` — naruszono kluczowy element Character Lock lub istotne proporcje.
- `PASS — Perfecto` — jawny werdykt użytkownika; nie oznacza automatycznego zapisu do repozytorium ani zmiany karty źródłowej.

Nie twierdź, że konkretne centymetry zostały fizycznie zweryfikowane na ilustracji. Wymiary są parametrami projektowymi, a widoczna zgodność obrazu jest oceną wizualną.

## 6. Zasada ciągłości

Ta procedura obowiązuje domyślnie przy kolejnych promptach i korektach Elary. Nie wymaga ponownej prośby użytkownika. Karta Manekin T-POSE pozostaje wzorcem anatomicznym; zaakceptowane ilustracje sceniczne nie nadpisują jej samoistnie.

---

## Źródła
- `char/Elara/ELARA.md` — https://github.com/Letacl-program/MANGA-SOURCES/blob/main/char/Elara/ELARA.md
- Karta Manekin T-POSE — zaakceptowany przez użytkownika wzorzec wizualno-anatomiczny z bieżącego kontekstu pracy.

**Uwaga:** plik definiuje procedurę pracy i nie zatwierdza automatycznie żadnej ilustracji ani nie zmienia Character Lock.
