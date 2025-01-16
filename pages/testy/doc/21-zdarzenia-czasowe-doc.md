---
title: 21. Zdarzenia czasowe (dokumenty)
last_updated: 16 stycznia 2025

sidebar: testy_sidebar
permalink: 21-zdarzenia-czasowe-doc
folder: testy/doc
---

## Wymagania dostępności
- {% include ks/1-4-2.md %}
- {% include ks/2-2-1.md %}
- {% include ks/2-2-2.md %}
-   [5.2 Wymagania zgodności: Bez zakłóceń](https://wcag.irdpl.pl/guidelines/22/#cc5) - Poniższe kryteria sukcesu dotyczą wszystkich treści na stronie, włącznie z treściami, które w&nbsp;innych przypadkach nie są podstawą spełnienia wymogów zgodności, ponieważ ich niespełnienie może zakłócać korzystanie ze strony:
    -   1.4.2 - Kontrola odtwarzania dźwięku,
    -   2.1.2 - Bez pułapki na klawiaturę,
    -   2.3.1 - Trzy błyski lub wartości poniżej progu, oraz
    -   2.2.2 - Pauza, zatrzymanie, ukrycie.
	
## Uzasadnienie metody testowej
Określenie, w jaki sposób użytkownik może modyfikować limity czasowe, automatyczne odtwarzanie i automatyczną aktualizację, a następnie wykonanie tych modyfikacji.

## Ograniczenia, założenia lub wyjątki
- Ograniczenie czasu uzasadnione którymkolwiek z poniższych kryteriów nie jest uwzględniane w tym teście:
    -   **Wyjątek dotyczący czasu rzeczywistego:** Limit czasowy jest wymaganym komponentem jakiejś czynności w czasie rzeczywistym (np. aukcji) i nie ma możliwości zmiany limitu, lub:
    -   **Wyjątek dotyczący istoty czynności:** Limit czasowy jest istotny i wydłużenie go anulowałoby lub zaburzałoby daną czynność, lub:
    -   **Wyjątek 20 godzin:** Limit czasowy przekracza 20 godzin.
	-   Treści, które powtarzają się lub są synchronizowane z innymi treściami, o ile informacje i dane są sterowane lub w inny sposób znajdują się pod kontrolą użytkownika. Przykłady ograniczeń czasu, do których to kryterium sukcesu nie ma zastosowania, obejmują przewijanie tekstu, który się powtarza, napisy i karuzele. Są to sytuacje, które obejmują limity czasowe, ale treść jest nadal dostępna dla użytkownika, ponieważ istnieją kontrolki dostępu do niej.
-   Zmiana treści jest uważana za „przedstawianą równolegle” z inną treścią, gdy pojawia się obok innych treści. Na przykład dynamiczna aktualizacja migawek na dole lub z boku strony byłaby uważana za „przedstawianą równolegle”, gdy dokument zawiera także wideo z wiadomościami i artykuły tekstowe (oba przykłady treści statycznej). Przycisk umożliwiający użytkownikom wstrzymanie zmiany treści nie będzie uważany za inną treść statyczną.
-   Poruszanie się, przesuwanie, migotanie lub automatyczna aktualizacja treści są uważane za „niezbędne”, jeżeli ich usunięcie zasadniczo zmieniłoby informacje lub funkcje, a informacji i funkcji nie można uzyskać w inny sposób, który byłby zgodny z wymogami dostępności.
-   Uwagi do KS 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie:
    -   *Uwaga 1*: Wytyczna 2.3 zawiera więcej informacji na temat treści migoczącej lub zawierającej błyski.
    -   *Uwaga 2*: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi skorzystanie z całego dokumentu, cała zawartość dokumentu (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić powyższe kryterium. Więcej informacji: [Wymagania zgodności: Bez zakłóceń](https://wcag.irdpl.pl/guidelines/22/#cc5).
    -   *Uwaga 3:* Treść, która jest aktualizowana okresowo przez aplikację lub przesyłana w sposób ciągły do programu użytkownika, nie musi być przechowywana lub przedstawiana, w czasie pomiędzy wstrzymaniem a wznowieniem prezentacji, ponieważ może to być technicznie niemożliwe, a w wielu przypadkach mogłoby wprowadzać użytkownika w błąd.
    -   *Uwaga 4:* Animacja, która pojawia się w czasie poprzedzającym załadowanie treści, może być uznana za istotną, jeśli wszyscy użytkownicy nie mogą dokonać interakcji w tym czasie oraz jeśli brak wskazania etapu załadowania mógłby wprowadzić użytkownika w błąd lub mogłoby mu się wydawać, że załadowanie treści zostało zawieszone albo przerwane.
-   Uwaga do KS 1.4.2 Kontrola odtwarzania dźwięku:
    -   *Uwaga 1*: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi odczytanie całego dokumentu, wszelkie treści dokumentu (bez względu na to, czy spełniają inne kryteria sukcesu, czy nie) muszą spełnić niniejsze kryterium. Więcej informacji: [Wymagania zgodności: Bez zakłóceń](https://www.w3.org/TR/WCAG20/#cc5)
-   Zgodnie z [Objaśnieniem KS 1.4.2 Kontrola odtwarzania dźwięku](https://wcag.irdpl.pl/understanding/kontrola-odtwarzania-dzwieku.html): Kontrola nad głośnością obejmuje możliwość zmniejszenia jej do zera. Wyciszenie głośności systemu nie oznacza „wstrzymania lub zatrzymania” automatycznego odtwarzania dźwięku. Zarówno „pauza lub stop”, jak i kontrola głośności dźwięku muszą być niezależne od ogólnej głośności systemu.

## 21.A Procedura testowa możliwości dostosowania czasu
Identyfikator testu podstawowego: _21.A-TimingAdjustable_

### Identyfikacja treści
Wykryj wszelkie przypadki ograniczeń czasowych treści (nie uwzględniaj wyjątków opisanych powyżej).

### Instrukcja testowania
Dla każdego wystąpienia ograniczenia czasu:
1.  Przed upływem limitu czasu sprawdź, czy spełniono przynajmniej jeden z poniższych warunków [KS 2.2.1]:
    -  Użytkownik ma możliwość wyłączenia limitu czasu.
    -  Użytkownik ma możliwość zwiększenia limitu czasu przed jego przekroczeniem o wartość co najmniej dziesięciokrotnie większą od wartości domyślnej.
    -  Użytkownik jest ostrzegany przed upływem limitu czasowego **ORAZ**:
        -   ma przynajmniej 20 sekund na wydłużenie limitu za pomocą prostej czynności (np. „wciśnij klawisz spacji”), **ORAZ**
        -   może wydłużyć limit limitu czasu co najmniej dziesięciokrotnie.

### Wynik testów
<p id="d21aTR">Jeżeli żaden z powyższych warunków nie jest spełniony, test podstawowy <em>21.A-TimingAdjustable</em> kończy się niepowodzeniem.</p>

## 21.B Procedura testowa ruchomych informacji 
Identyfikator testu podstawowego: _21.B-MovingInfo_

### Identyfikacja treści
Wszelkie ruchome, migające lub przewijane informacje, które spełniają WSZYSTKIE z poniższych kryteriów:
-   uruchamiają się automatycznie **ORAZ**
-   trwają dłużej niż 5 sekund, **ORAZ**
-   Są prezentowane równolegle z innymi treściami, **ORAZ**
-   Ich poruszanie, przesuwanie, migotanie nie jest konieczne

### Instrukcja testowania
1.  Sprawdź, czy istnieje mechanizm umożliwiający użytkownikowi ich wstrzymanie, zatrzymanie lub ukrycie. [KS 2.2.2]

### Wynik testów
<p id="d21bTR">Jeżeli powyższy warunek nie jest spełniony, test podstawowy <em>21.B-MovingInfo</em> kończy się niepowodzeniem.</p>

## 21.C Procedura testowa automatycznej aktualizacji treści
Identyfikator testu podstawowego: _21.C-AutoUpdate_

### Identyfikacja treści
Wszelkie treści, które aktualizują się automatycznie, spełniające WSZYSTKIE poniższe kryteria:
-   aktualizacja uruchamia się automatycznie **ORAZ**
-   są prezentowane równolegle z innymi treściami, **ORAZ**
-   nie są istotną (niezbędną) częścią działania.

### Instrukcje testowe
1.  Sprawdź, czy istnieje mechanizm umożliwiający użytkownikowi [KS 2.2.2]
    - wstrzymanie, zatrzymanie lub ukrycie **ALBO**
	- kontrolowanie częstotliwości aktualizacji.

### Wynik testów
<p id="d21cTR">Jeżeli żaden z warunków powyżej nie jest spełniony, test podstawowy <em>21.C-AutoUpdate</em> kończy się niepowodzeniem.</p>

## 21.D Procedura testowa kontroli odtwarzania dźwięku 
Identyfikator testu podstawowego: _21.D-AudioControl_

### Identyfikacja treści
Elementy strony odtwarzające dźwięk dłużej niż 3 sekundy.
### Instrukcje testowe
1.  Sprawdź jedną z poniższych możliwości
    -  Na początku dokumentu lub w funkcjach dostępności do platformy istnieje mechanizm wstrzymania lub zatrzymania dźwięku, **ALBO**
    -  Na początku dokumentu lub w funkcjach dostępności do platformy istnieje mechanizm regulacji głośności niezależny od ogólnego poziomu głośności systemu.

### Wynik testów
<p id="d21dTR">Jeżeli żaden z warunków powyżej nie jest spełniony, test podstawowy <em>21.D-AudioControl</em> kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

-   Przypomnij testerom, że w przypadku przekroczenia limitu czasu wskaźnik fokusu powinien się przemieścić  do komunikatu o limicie czasu, aby spełnić kryteria sukcesu dotyczące dostępności klawiatury i kolejności fokusu.
-   W niektórych przypadkach może być konieczne skontaktowanie się z autorami aplikacji w celu wyjaśnienia warunków przekroczenia limitu czasu.
-   Błędy KS 1.4.2 lub 2.2.2 powodują  również niespełnienie [Wymagania dotyczącego zgodności: Bez zakłóceń](https://www.w3.org/TR/WCAG20/#cc5) i powinny być zaznaczone w raporcie z testów, aby wskazać poważny wpływ na dostępność.
-   Przed rozpoczęciem testu odtwarzacze muszą być skonfigurowane tak, aby zezwalały na odtwarzanie dźwięku. Instrukcje dotyczą wyłącznie zgodnych odtwarzaczy. Wyniki testu mogą zależeć od od używanego odtwarzacza multimedialnego.
-   Treść, która została uznana za niezgodną z KS 2.2.2, może zostać oznaczona do dalszego przeglądu pod kątem wyjątku, jeśli automatyczna aktualizacja jest niezbędna. Jednak wyjątek dla KS 2.2.2 należy rozważyć ostrożnie, ponieważ [Wymagania dotyczącego zgodności: Bez zakłóceń](https://www.w3.org/TR/WCAG20/#cc5) muszą być spełnione.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G4.md %}
- {% include techniki/G60.md %}
- {% include techniki/G170.md %}
- {% include techniki/G171.md %}
- {% include techniki/G180.md %}
- {% include techniki/G186.md %}
- {% include techniki/G198.md %}
- {% include techniki/SCR16.md %} ORAZ {% include techniki/SCR1.md %}
- {% include techniki/SCR33.md %}
- {% include techniki/SCR36.md %}
- {% include techniki/F16.md %}
