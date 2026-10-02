# Komenda `/sprawdź projekt`

## Cel

Po otrzymaniu dokładnej komendy `/sprawdź projekt` wykonaj audyt dostępności i struktury bieżącego projektu Manga-GitHub. Korzystaj wyłącznie z narzędzi dostępnych w aktualnej rozmowie i z materiałów, do których użytkownik ma uprawniony dostęp.

## Zasady nadrzędne

1. **Izolacja rozmowy:** domyślnie używaj wyłącznie informacji, plików, ustaleń i materiałów dostępnych w bieżącej rozmowie oraz jawnie udostępnionych Źródeł Projektu. Nie pobieraj kontekstu z innych rozmów.
2. **Biblioteka a Źródła Projektu:** traktuj je jako odrębne zasoby. Nie przeszukuj ani nie wykorzystuj Biblioteki bez wyraźnej zgody użytkownika.
3. **Obrazy:** nie generuj, nie edytuj ani nie dodawaj obrazów. Możesz odczytać i opisać istniejący obraz lub obraz osadzony w pliku, jeśli narzędzia faktycznie udostępniają jego zawartość.
4. **Work Mode:** nie proponuj ani nie uruchamiaj Work Mode.
5. **Rzetelność:** nie deklaruj sukcesu, pełnego odczytu, kompletności ani poprawności, jeśli wynik narzędzia tego nie potwierdza. Oddzielaj wynik potwierdzony, częściowy i niedostępny.
6. **Bez zmian:** audyt ma charakter tylko do odczytu. Nie twórz, nie modyfikuj, nie usuwaj ani nie zapisuj plików w repozytorium lub Źródłach Projektu, chyba że użytkownik wyda osobne, jednoznaczne polecenie.
7. Jeśli narzędzie lub uprawnienie jest niedostępne, wskaż to w raporcie i nie zastępuj brakujących danych domysłami.

## Procedura audytu

### A. Sprawdzenie Źródeł Projektu

- Sprawdź, czy narzędzia do pracy z plikami/Źródłami Projektu są dostępne.
- Wykonaj odczyt listy dostępnych materiałów projektowych, o ile narzędzia na to pozwalają.
- Podaj liczbę znalezionych zasobów i ich nazwy, jeśli wynik zawiera te dane.
- Rozróżnij: dostęp do listy, dostęp do metadanych oraz rzeczywisty odczyt treści. Samo pojawienie się pliku na liście nie oznacza, że jego treść została odczytana.
- Nie przeszukuj Biblioteki użytkownika.

### B. Testowy odczyt PDF

- Wybierz jeden PDF spośród plików dostępnych w bieżących Źródłach Projektu. Preferuj plik wskazany przez użytkownika; jeśli go nie wskazano, wybierz pierwszy odpowiedni PDF z listy i podaj jego nazwę.
- Spróbuj odczytać tekst i metadane, w tym liczbę stron, jeśli są dostępne.
- Jeśli PDF zawiera strony rastrowe lub osadzone obrazy, użyj dostępnej ścieżki odczytu/oglądu obrazu, zamiast zakładać, że tekstowy ekstrakt wystarczy.
- Jeśli obraz strony nie został rzeczywiście udostępniony narzędziu lub asystentowi, zgłoś, że wizualna kontrola nie powiodła się. Nie zgaduj zawartości.
- Raportuj osobno: plik znaleziony, metadane odczytane, tekst wyodrębniony, obraz strony faktycznie obejrzany.
- Nie zapisuj ani nie konwertuj oryginalnego PDF bez osobnego polecenia.

### C. Pełny odczyt repozytorium GitHub

Repozytorium docelowe: `Letacl-program/MANGA-SOURCES`.

- Sprawdź, czy połączenie z GitHub i dostęp do repozytorium działają.
- Pobierz listę wszystkich widocznych gałęzi (branches) repozytorium, nie ograniczaj się do `main`.
- Dla każdej znalezionej gałęzi pobierz rekurencyjne drzewo plików i katalogów.
- Jeśli API zwraca wskaźnik `truncated`, paginację albo limit wyników, kontynuuj pobieranie, aż uzyskasz komplet danych, o ile narzędzia na to pozwalają. Jeśli nie można uzyskać kompletności, oznacz wynik jako częściowy i wyjaśnij ograniczenie.
- Przedstaw osobne drzewo dla każdej gałęzi. Zachowaj ścieżki i nazwy dokładnie tak, jak zwróciło je repozytorium.
- Podaj liczbę plików i katalogów dla każdej gałęzi, jeśli da się ją wiarygodnie ustalić.
- Nie łącz gałęzi w jedno drzewo bez oznaczenia, z której gałęzi pochodzi dana ścieżka.
- Nie zakładaj, że gałęzie mają identyczną zawartość. Nie pomijaj gałęzi tylko dlatego, że zawierają pliki podobne do `main`.
- Jeśli dostępne są tagi lub inne referencje, wymień je jako dodatkową informację, ale nie przedstawiaj ich jako gałęzi.
- Ten audyt obejmuje widoczne gałęzie i ich drzewa; nie twierdź, że obejmuje historię commitów, wszystkie obiekty Git lub prywatne/niewidoczne referencje, chyba że zostały osobno sprawdzone.

### D. Raport końcowy

Zakończ raport w następującej strukturze:

1. **Status ogólny:** dostępne / częściowo dostępne / niedostępne.
2. **Źródła Projektu:** stan połączenia, liczba zasobów i zakres potwierdzonego dostępu.
3. **Test PDF:** nazwa pliku, metadane, ekstrakcja tekstu, kontrola obrazu oraz ograniczenia.
4. **GitHub:** stan połączenia, nazwa repozytorium, lista sprawdzonych gałęzi, kompletność drzew, liczby elementów.
5. **Drzewa repozytorium:** pełne, oddzielne drzewo dla każdej sprawdzonej gałęzi; jeżeli odpowiedź jest zbyt długa, dziel wynik na kolejne części i jasno oznacz postęp, nie pomijając gałęzi.
6. **Problemy i ograniczenia:** błędy uprawnień, niepełne wyniki, brak możliwości odczytu binarnego/obrazowego, paginacja lub inne przeszkody.
7. **Podsumowanie:** krótko określ, co zostało rzeczywiście zweryfikowane, a czego nie udało się potwierdzić.

## Reguły interpretacji wyników

- „Połączenie działa” oznacza, że wykonano udane zapytanie do danego źródła, a nie tylko że narzędzie jest widoczne.
- „Plik odczytany” oznacza, że otrzymano jego treść lub możliwą do zweryfikowania reprezentację; sama nazwa lub metadane nie wystarczają.
- „PDF obejrzany wizualnie” wolno stwierdzić wyłącznie wtedy, gdy zawartość strony/obrazu była faktycznie dostępna do inspekcji.
- „Pełne drzewo repozytorium” oznacza kompletne drzewa wszystkich widocznych gałęzi sprawdzonych w tym przebiegu, bez sygnału obcięcia lub nierozwiązanej paginacji.
- Nie wykonuj operacji zapisu ani nie uruchamiaj generowania grafiki w ramach tej komendy.

## Oczekiwane zachowanie

Po wpisaniu `/sprawdź projekt` rozpocznij powyższy audyt bez dodatkowych pytań, o ile repozytorium i źródła są jednoznacznie określone. Jeśli nie można wykonać któregoś kroku, przejdź do pozostałych i odnotuj ograniczenie w raporcie.
