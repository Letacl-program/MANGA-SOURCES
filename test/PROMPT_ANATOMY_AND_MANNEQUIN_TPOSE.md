# Uniwersalne zasady promptów anatomicznych i kart technicznych postaci

**Status:** OBOWIĄZUJĄCA PROCEDURA ROBOCZA  
**Ścieżka:** `test/PROMPT_ANATOMY_AND_MANNEQUIN_TPOSE.md`  
**Zakres:** Wszystkie postacie, style, pozy, testy spójności, ilustracje oraz karty techniczne.

## 1. Zasada nadrzędna

Przed każdym generowaniem lub poprawianiem postaci należy korzystać z jej zatwierdzonych źródeł referencyjnych. Procedura obowiązuje domyślnie i nie wymaga ponownego przypominania przez użytkownika.

Zasady są uniwersalne, ale **wartości anatomiczne, cechy wyglądu i hierarchia konkretnych źródeł muszą pochodzić z dokumentacji danej postaci**. Nie wolno przenosić wymiarów, cech ani ograniczeń jednej postaci na inną.

### Ustal hierarchię źródeł dla konkretnej postaci

Przed generowaniem ustal, które materiały są dostępne i jaką mają rangę. Typowy układ może obejmować:
1. Kanoniczny plik MD postaci — tożsamość, Character Lock, stałe cechy i zatwierdzone parametry.
2. Zatwierdzoną Kartę Manekin T-POSE — nadrzędny wzorzec wizualno-anatomiczny, jeśli istnieje i został wskazany jako taki.
3. Techniczny T-POSE — wymiary, punkty odniesienia i proporcje.
4. Wizualną kartę postaci — wygląd, kolory, materiały i detale.
5. Zatwierdzone ilustracje sceniczne — przykłady pozy, stroju lub ekspresji, o ile nie stoją w sprzeczności ze źródłami wyższego rzędu.

Ten układ jest wzorcem organizacyjnym, nie założeniem, że każda postać ma wszystkie wymienione pliki. Jeśli użytkownik lub dokumentacja określa inną hierarchię, stosuj jawnie zatwierdzoną hierarchię tej postaci.

Jeżeli źródła są sprzeczne, nie poprawiaj ich po cichu. Wskaż konflikt i poproś o rozstrzygnięcie, gdy jest ono konieczne. Nie zakładaj dostępu do plików ani kart z innych rozmów lub środowisk bez upoważnienia.

## 2. Wydobycie danych referencyjnych

Przed promptem zbierz z dokumentacji konkretnej postaci:
- nazwę/ID postaci oraz kanoniczny plik źródłowy;
- stałe cechy tożsamości i anatomii;
- zatwierdzoną sylwetkę i relacje proporcji;
- dostępne wymiary liczbowe, jednostki i sposób ich oszacowania;
- cechy gatunkowe lub konstrukcyjne, liczbę i budowę kończyn, uszu, ogona, rogów, skrzydeł, stóp itp., jeśli występują;
- wygląd głowy, twarzy, włosów, skóry/powierzchni, kolorystykę i znaki szczególne;
- elementy zmienne: strój, fryzurę, ekspresję, pozę, rekwizyty i tło;
- cechy nieustalone, których nie wolno samodzielnie dopowiadać.

### Zasady wymiarów
- Wpisuj do promptu konkretne wartości z dokumentacji, gdy są dostępne i istotne dla testu.
- Zachowuj jednostki oraz nazwy pomiarów z dokumentacji.
- Rozróżniaj wartości zmierzone, szacunki koncepcyjne i proporcje opisowe.
- Nie wymyślaj brakujących liczb ani nie przedstawiaj estymat jako pomiarów fizycznych.
- Gdy brak wymiarów liczbowych, użyj opisów relacyjnych zatwierdzonych w źródle, np. „biodra szersze od barków” albo „głowa stanowi około X wysokości postaci” — tylko jeśli źródło rzeczywiście to określa.
- Jeżeli wymiaru nie da się odczytać lub źródła go nie podają, oznacz go jako nieustalony zamiast zgadywać.

## 3. Budowa promptu do ilustracji

Każdy prompt powinien zawierać następujące warstwy:

1. **Tożsamość i Character Lock:** nazwa postaci, gatunek/typ, stałe cechy wyglądu i anatomii.
2. **Parametry i proporcje:** wpisz kluczowe wartości z pliku MD oraz zatwierdzonych kart. Przy teście anatomicznym dołącz pełen zestaw istotnych wymiarów, a nie tylko ogólny opis.
3. **Wzorzec referencyjny:** nazwij konkretne pliki/karty postaci, które mają pierwszeństwo. Nie odwołuj się do nieudostępnionego materiału tak, jakby generator miał do niego dostęp; jeśli obraz referencyjny nie jest przekazywany do generatora, opisz jego kluczowe cechy tekstowo.
4. **Cel panelu:** określ jedną pozę, emocję, strój, styl, kadr i tło.
5. **Niezmienność anatomii:** zmiana pozy, perspektywy, emocji, stroju, oświetlenia i stylu nie może zmieniać bazowych proporcji ani stałych cech.
6. **Kompozycja:** określ, czy potrzebna jest cała postać, widoki ortogonalne, zbliżenia, konkretne proporcje kadru i widoczność kończyn.
7. **Ograniczenia negatywne:** wypisz typowe błędy, których należy unikać, zgodnie z dokumentacją danej postaci.
8. **Format wyniku:** jeden panel, arkusz techniczny lub plansza wielopanelowa — zgodnie z zamówieniem.

### Uniwersalny szablon promptu

> Użyj [KANONICZNY PLIK MD POSTACI] oraz [ZATWIERDZONE KARTY REFERENCYJNE] zgodnie z określoną hierarchią źródeł. Zachowaj Character Lock i wszystkie stałe cechy postaci. Uwzględnij następujące zatwierdzone parametry: [WSTAW WYMIARY I PROPORCJE Z DOKUMENTACJI, Z JEDNOSTKAMI I OZNACZENIEM ESTYMAT, JEŚLI DOTYCZY]. Zachowaj relacje proporcji i charakterystyczną sylwetkę z karty. Nie zmieniaj anatomii w celu dopasowania postaci do pozy, kadru, stroju ani stylu. Nie dodawaj cech, których źródła nie ustalają. Wykonaj [POZA / AKCJA] w stylu [STYL], z emocją [EMOCJA], w stroju [STRÓJ], na tle [TŁO]. Kadrowanie: [KADR]. Zapewnij czytelność wszystkich istotnych części ciała i unikaj przypadkowego ucinania kończyn. [DODATKOWE OGRANICZENIA WŁAŚCIWE DLA TEJ POSTACI I TESTU].

Przed wysłaniem promptu zastąp wszystkie pola w nawiasach rzeczywistymi danymi ze źródeł. Nie przekazuj generatorowi przykładowych wymiarów należących do innej postaci.

## 4. Generowanie technicznej karty / manekina

Gdy celem jest sprawdzenie proporcji, nie zastępuj karty technicznej zwykłą ilustracją sceniczną.

Wybierz elementy odpowiednie dla zadania:
- Czysty, neutralny arkusz techniczny.
- Widoki z przodu, boku i tyłu w tej samej skali; neutralna pozycja A-pose lub T-pose, o ile anatomia postaci na to pozwala.
- Cała postać widoczna w każdym wymaganym widoku.
- Siatka powierzchniowa, linie osi, przekroje i punkty odniesienia na neutralnym, nieprzezroczystym manekinie lub stroju technicznym, gdy potrzebna jest kontrola anatomii.
- Linie wymiarowe z podpisanymi jednostkami, czytelną legendą i tabelą parametrów.
- Zbliżenia cech charakterystycznych, które wymagają osobnej kontroli.
- Wymiary i adnotacje zgodne z kanonicznym MD i zatwierdzonymi kartami danej postaci.
- Oznaczenie wartości jako pomiarów, szacunków koncepcyjnych lub danych nieustalonych.
- Podpisy nie mogą zasłaniać sylwetki ani utrudniać oceny proporcji.

Nie wszystkie postacie mają ludzką anatomię ani standardowe kończyny. Układ widoków, siatkę i punkty odniesienia należy dostosować do zatwierdzonej anatomii konkretnej postaci, nie zaś normalizować ją do uniwersalnego humanoida.

Jeżeli obraz wygenerowany i źródła się różnią, pierwszeństwo ma zatwierdzona hierarchia źródeł. Karta techniczna nie staje się kanoniczna tylko dlatego, że została wygenerowana; wymaga osobnej akceptacji użytkownika, jeśli taki jest proces projektu.

## 5. Kontrola po wygenerowaniu

Porównaj wynik z właściwymi źródłami i sprawdź:
- tożsamość i wszystkie stałe cechy;
- sylwetkę oraz relacje proporcji;
- zgodność wymiarów i adnotacji z dokumentacją;
- liczbę, budowę i położenie kończyn oraz cech gatunkowych/konstrukcyjnych;
- spójność głowy, twarzy, włosów, skóry/powierzchni i znaków szczególnych;
- czy strój nie maskuje błędów, nie zmienia wizualnie bazowej anatomii ani nie dodaje cech sprzecznych ze źródłem;
- czy cała postać jest widoczna, a istotne części nie są przypadkowo zasłonięte;
- czy perspektywa powoduje normalne skróty optyczne, czy rzeczywisty błąd rysunku;
- czy styl zmienia jedynie sposób prezentacji, a nie tożsamość lub anatomię.

### Status wyniku
- `PASS` — rezultat zgodny z zatwierdzonym wzorcem w ocenianym zakresie.
- `PARTIAL` — podstawowa tożsamość jest zachowana, ale część kryteriów jest nieczytelna lub wymaga korekty.
- `FAIL` — naruszono kluczowy element Character Lock, istotne proporcje lub wymagania zadania.
- `PASS — Perfecto` — jawny werdykt użytkownika; sam w sobie nie oznacza zapisu do repozytorium ani zmiany źródeł kanonicznych.

Nie twierdź, że konkretne wymiary fizyczne zostały zweryfikowane na podstawie ilustracji. Wizualna ocena zgodności nie zastępuje pomiaru technicznego.

## 6. Ciągłość i stosowanie domyślne

Ta procedura obowiązuje domyślnie przy kolejnych promptach, poprawkach, testach anatomii oraz generowaniu kart technicznych dla wszystkich postaci objętych projektem. Nie wymaga ponownej prośby użytkownika.

Przy każdej nowej postaci:
1. Odszukaj i wykorzystaj wyłącznie źródła dostępne i autoryzowane w bieżącym środowisku.
2. Ustal jej własny Character Lock i hierarchię źródeł.
3. Wstaw do promptu jej własne parametry — nigdy parametry Elary ani innej postaci.
4. Jeśli brakuje źródeł lub istotnych danych, wskaż brak zamiast rekonstruować je na podstawie innych rozmów.
5. Nie aktualizuj automatycznie kanonicznej dokumentacji na podstawie pojedynczej wygenerowanej ilustracji.

---

## Źródła i zakres

Dokument definiuje **uniwersalną metodę pracy**, a nie kanoniczną anatomię żadnej konkretnej postaci. Szczegóły każdej postaci pochodzą z jej własnych plików źródłowych i zatwierdzonych kart.

**Przykład zastosowania:** `char/Elara/ELARA.md` może być źródłem parametrów Elary, ale jego wymiary i cechy nie są domyślnymi parametrami innych postaci.

**Uwaga:** zapis procedury nie zatwierdza żadnej ilustracji, nie tworzy automatycznie kart źródłowych i nie zmienia Character Lock.
