## Zasada nr 2: Funkcjonalność
Komponenty interfejsu użytkownika oraz nawigacja muszą być możliwe do użycia.

## Wytyczna 2.1 Dostępność z klawiatury
Zapewnij dostępność wszystkich funkcjonalności za pomocą klawiatury.

### 2.1.1 Klawiatura:
Cała treść oraz wszystkie zawarte w niej <a title="definicja: funkcjonalność" href="#functiondef" class="termref">funkcjonalności</a> dostępne są z interfejsu klawiatury, bez wymogu określonego czasu użycia poszczególnych klawiszy, poza tymi przypadkami, kiedy dana funkcja wymaga wprowadzenia informacji przez użytkownika w oparciu o ścieżkę ruchów, a nie w oparciu o punkty końcowe wejścia. 
(Poziom A)

*Uwaga 1:* Ten wyjątek dotyczy danej funkcji, a nie techniki wejścia. Przykładowo, kiedy używa się pisma odręcznego celem 
wprowadzenia tekstu, technika wejścia (pismo odręczne) wymaga wprowadzenia informacji w oparciu o ścieżkę, jednak powiązana z tym funkcja (wprowadzenie tekstu) już tego nie wymaga. 

*Uwaga 2:* To nie powinno blokować ani ograniczać użycia interfejsu innymi metodami niż klawiatura, np. za pomocą myszki. 
### 2.1.2 Brak pułapki na klawiaturę
Jeśli fokus klawiatury można przemieścić do danego komponentu strony za pomocą <a title="definicja: interfejs klawiaturowy" href="#keybrd-interfacedef" class="termref">interfejsu klawiatury</a>, to może on być z niego usunięty również za pomocą interfejsu klawiatury, w przypadku gdy wymagane, a jeśli wówczas jest wymagane użycie czegoś więcej niż samych strzałek, tabulatora lub innych standardowych metod wyjścia, użytkownik musi otrzymać odpowiednią podpowiedź, w jaki sposób usunąć fokus z danego komponentu. (Poziom A)

*Uwaga:* Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi skorzystanie z całej 
strony, cała zawartość danej strony (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić powyższe kryterium. Więcej informacji: <a href="http://www.w3.org/TR/WCAG/#cc5">Spełnienie wymagań: brak zakłóceń: Non-Interference</a>.

### 2.1.3 Klawiatura (bez wyjątków)
Cała treść oraz wszystkie zawarte w niej <a title="definicja: funkcjonalność" href="#functiondef" class="termref">funkcjonalności</a> dostępne są z <a title="definicja: interfejs klawiaturowy" href="#keybrd-interfacedef" class="termref">interfejsu klawiatury</a>, bez wymogu określonego czasu użycia poszczególnych klawiszy. (Poziom AAA)


## Wytyczna 2.2 Wystarczająca ilość czasu
Zapewnij użytkownikom wystarczająco  dużo czasu na przeczytanie i skorzystanie z treści.

### 2.2.1 Możliwość dostosowania czasu
Dla każdego limitu czasowego, ustawionego na odbiór treści, spełnione jest przynajmniej jedno z poniższych założeń: (Poziom A)

- **Wyłączenie:** Użytkownik może wyłączyć limit czasowy zanim czas upłynie; lub:
- **Dostosowanie:** Użytkownik może swobodnie dostosować limit czasowy (przynajmniej o wartość 10 razy większą od 
wartości domyślnej) zanim czas upłynie; lub
- **Wydłużenie:** Użytkownik jest ostrzegany przed upłynięciem limitu czasowego i ma przynajmniej 20 sekund na wydłużenie limitu za pomocą prostej czynności (np. „wciśnij klawisz spacji”) oraz może wydłużyć limit przynajmniej dziesięciokrotnie, lub:
- **Wyjątek dotyczący czasu rzeczywistego:** Limit czasowy jest wymaganym komponentem jakiejś czynności w czasie 
rzeczywistym (np. aukcji) i nie ma możliwości zmiany limitu, lub:
- **Wyjątek dotyczący istoty czynności:** Limit czasowy jest <a title="definicja: istotny" href="#essentialdef" class="termref">istotny</a> i wydłużenie go anulowałoby lub zaburzałoby daną czynność, lub:
- **Wyjątek 20 godzin:** Limit czasowy przekracza 20 godzin.

*Uwaga:* To kryterium sukcesu ma na celu zapewnienie użytkownikowi wystarczającego czasu na wykonanie czynności, bez 
niespodziewanych zmian treści lub kontekstu, które mogą być wynikiem limitu czasowego. Powinien on być rozpatrywany w połączeniu z <a href="#consistent-behavior-receive-focus">kryterium sukcesu 3.2.1</a>, które nakłada ograniczenia na zmiany treści lub kontekstu w wyniku działania użytkownika.

### 2.2.2: Wstrzymywanie (pauza), zatrzymywanie, ukrywanie:**
Wszystkie poniższe zasady obowiązują w przypadku informacji, która przesuwa się, porusza, <a title="definicja: migotanie" href="#blinksdef" class="termref">migota</a> lub automatycznie jest aktualizowana: (Poziom A)

- <p>**Poruszanie się, przesuwanie, migotanie:** Każdą informację, która porusza się, przesuwa lub mruga, a takie działanie (1) włącza się automatycznie, (2) jest widoczne dłużej niż 5 sekund, (3) jest przedstawiane równolegle z inną treścią — użytkownik może <a title="definicja: wstrzymane" href="#pauseddef" class="termref">wstrzymać</a>, zatrzymać lub ukryć za pomocą dostępnego mechanizmu, chyba, że poruszanie się, przesuwanie lub migotanie jest częścią czynności gdzie takie działanie jest <a title="definicja: istotny" href="#essentialdef" class="termref">istotne</a>, oraz:
- **Automatyczna aktualizacja:** Każdą automatycznie aktualizującą się informację, która (1) włącza się automatycznie oraz (2) jest przedstawiana równolegle z inną treścią — użytkownik może wstrzymać, zatrzymać lub kontrolować częstotliwość aktualizacji za pomocą dostępnego mechanizmu, chyba, że automatyczna aktualizacja jest częścią takiej czynności, gdzie takie działanie jest niezbędne

*Uwaga 1:* <a href="#seizure">Wytyczna 2.3</a> zawiera więcej informacji na temat treści migoczącej lub zawierającej błyski.

*Uwaga 2:* Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi skorzystanie z całej strony, cała zawartość danej strony (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić powyższe kryterium. Więcej informacji: <a href="#cc5">Spełnienie wymagań: brak zakłóceń: Non-Interference</a>.

*Uwaga 3:* Treść, która jest aktualizowana okresowo przez aplikację lub przesyłana w sposób ciągły do programu użytkownika, nie musi być przechowywana lub przedstawiana, w czasie pomiędzy wstrzymaniem a wznowieniem prezentacji, ponieważ może to być technicznie nie możliwe, a w wielu przypadkach mogłoby wprowadzać użytkownika w błąd.

*Uwaga 4:* Animacja, która pojawia się w czasie poprzedzającym załadowanie treści, może być uznana za istotną, jeśli 
wszyscy użytkownicy nie mogą dokonać interakcji w tym czasie oraz jeśli brak wskazania etapu załadowania mógłby wprowadzić użytkownika w błąd lub mogłoby mu się wydawać, że załadowanie treści zostało zawieszone albo przerwane.

### 2.2.3 Brak ograniczeń czasowych
Ograniczenie czasowe nie jest <a title="definicja: istotny" href="#essentialdef" class="termref">istotną</a> częścią czynności prezentowanej na stronie, chyba, że są to nieinteraktywne, <a title="definicja: zsynchronizowane multimedia" href="#synchronizedmediadef" class="termref">zsynchronizowane multimedia</a> lub  <a title="definicja: wydarzenia w czasie rzeczywistym" href="#real-time-eventsdef" class="termref">wydarzenia w czasie rzeczywistym</a>. (Poziom AAA)

### 2.2.4 Zakłócenie pracy użytkownika
Zakłócenia mogą być odłożone w czasie lub odrzucone przez użytkownika, chyba, że jest to <a title="definicja: zagrożenie" href="#emergencydef" class="termref">sytuacja wyjątkowa</a> (np. zagrożenie życia lub zdrowia). (Poziom AAA)

### 2.2.5 Ponowne potwierdzenie autentyczności
Kiedy kończy się czas sesji autoryzowanej przez użytkownika, może on kontynuować czynność bez utraty danych po ponownej autoryzacji. (Poziom AAA)

## Wytyczna 2.3 Ataki padaczki
Nie należy projektować treści w taki sposób, aby prowokować ataki padaczki.

### 2.3.1 Trzy błyski lub wartości poniżej progu:** 
<a title="definicja: strona internetowa" href="#webpagedef" class="termref">Strony internetowe</a> nie zawierają w swojej treści niczego, co migocze częściej niż trzy razy w ciągu jednej sekundy, lub też <a title="definicja: błysk" href="#flash-def" class="termref">błysk</a> nie przekracza <a title="definicja: informacje o granicznych wartościach dowolnych błysków i czerwonych błysków" href="#general-thresholddef" class="termref">wartości granicznych dla błysków ogólnych i czerwonych</a>. (Poziom A)

*Uwaga:* Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi skorzystanie z całej 
strony, cała zawartość danej strony (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić powyższe kryterium. Więcej informacji: <a href="http://www.w3.org/TR/WCAG/#cc5">Spełnienie wymagań: brak zakłóceń: Non-Interference</a>.

### 2.3.2 Trzy błyski:** <a title="definicja: strona internetowa" href="#webpagedef" class="termref">Strony internetowe</a> nie 
zawierają w swojej treści niczego, co <a title="definicja: błysk" href="#flash-def" class="termref">migocze</a> częściej niż trzy razy w 
ciągu jednej sekundy. (Poziom AAA)

### Wytyczna 2.4 Możliwość nawigacji
Dostarczenie narzędzi ułatwiających użytkownikowi nawigowanie, znajdowanie treści i ustalanie, gdzie się w danym momencie znajduje.

### 2.4.1 Możliwość pominięcia bloków
Dostępny jest <a title="definicja: mechanizm" href="#mechanismdef" class="termref">mechanizm</a>, który umożliwia pominięcie bloków treści powtarzanych na wielu <a title="definicja: strona internetowa" href="#webpagedef" class="termref">stronach internetowych</a>. (Poziom A)

### 2.4.2 Tytuły stron
<a title="definicja: strona internetowa" href="#webpagedef" class="termref">Strony internetowe</a> posiadają tytuły, które opisują ich cel lub przedstawiają ich temat. (Poziom A)

### 2.4.3 Kolejność fokusa
Jeśli <a title="definicja: strona internetowa" href="#webpagedef" class="termref">strona internetowa</a> może być <a title="definition: nawigowane sekwencyjnie" href="#nav-seqdef" class="termref">nawigowana sekwencyjnie</a>, a kolejność nawigacji wpływa na zrozumienie lub funkcjonalność strony, komponenty przyjmujące fokus zachowują kolejność, dzięki której zachowany jest sens i funkcjonalność treści. (Poziom A)

### 2.4.4 Cel linku (w kontekście)
<a title="definicja: cel linku" href="#linkpurposedef" class="termref">Cel każdego linku</a> może wynikać z samej treści linku, lub też z treści linku powiązanej z <a title="definicja: kontekst linku określony programistycznie" href="#pdlinkcontextdef" class="termref">programistycznie określonym kontekstem</a>, poza tymi przypadkami, kiedy cel łącza i tak byłby <a title="definicja: ogólnie niejednoznaczny dla użytkowników" href="#ambiguouslinkdef" class="termref">niejasny dla użytkowników</a>. (Poziom A)

### 2.4.5 Wiele dróg
Istnieje więcej niż jedna droga umożliwiająca zlokalizowanie <a title="definicja: strona internetowa" href="#webpagedef" class="termref">strony</a> w danym <a title="definicja: zestaw stron internetowych/serwis internetowy" href="#set-of-web-pagesdef" class="termref">serwisie internetowym</a>, za wyjątkiem sytuacji, kiedy dana strona jest wynikiem jakiejś <a title="definicja: procedura" href="#processdef" class="termref">procedury</a> lub jednym z jej etapów. (Poziom AA)

### 2.4.6 Nagłówki i etykiety
Nagłówki i <a title="definicja: etykieta" href="#labeldef" class="termref">etykiety</a> opisują temat lub cel treści. (Poziom AA)

### 2.4.7 Widoczny fokus
Każdy interfejs możliwy do nawigacji za pomocą klawiatury, posiada widoczny wskaźnik fokusa klawiatury. (Poziom AA)

### 2.4.8 Lokalizacja
Dostępna jest informacja, w którym miejscu w danym <a title="definicja: zestaw stron internetowych/serwis internetowy" href="#set-of-web-pagesdef" class="termref">serwisie internetowym</a> znajduje się użytkownik. (Poziom AAA)

### 2.4.9 Cel linku (z samego linku)
Dostępny jest 
<a title="definicja: mechanizm" href="#mechanismdef" class="termref">mechanizm</a> umożliwiający zidentyfikowanie celu każdego linku z samej jego treści, poza tymi przypadkami, kiedy cel łącza i tak byłby <a title="definicja: ogólnie niejednoznaczny dla użytkowników" href="#ambiguouslinkdef" class="termref">niejasny dla użytkowników</a> (Poziom AAA)

### 2.4.10 Nagłówki sekcji
Nagłówki <a title="definicja: sekcja" href="#sectiondef" class="termref">sekcji</a> są używane do porządkowania treści. (Poziom AAA)

*Uwaga 1:* Termin „nagłówek” został tu użyty w swoim ogólnym znaczeniu, obejmując tytuły i inne sposoby przypisywania 
nagłówków do różnego rodzaju treści.

*Uwaga 2:* Powyższe kryterium sukcesu dotyczy sekcji samych
 tekstów, a nie <a title="definicja: komponent interefejsu użytkownika" href="#user-interface-componentdef" class="termref">komponentów interfejsu użytkownika</a>, które omawiane są osobno w ramach <a href="http://www.w3.org/TR/2008/REC-WCAG20-20081211/#ensure-compat-rsv">kryterium sukcesu 4.1.2</a>.
