---
title: 21. Limity czasu


sidebar: testy_sidebar
permalink: ICT-21-limity-czasu
folder: testy/itc
---


## Wymagania dostępności
- {% include ks/2-2-1.md %}
- {% include ks/2-2-2.md %}
- {% include ks/1-4-2.md %}

-   [Wymogi zgodności: 5. Brak zakłóceń](https://www.w3.org/TR/WCAG20/#cc5) - Następujące kryteria sukcesu dotyczą całej treści na stronie, włącznie z treścią, która w innych przypadkach nie jest podstawą spełnienia wymogów zgodności, gdyż niezastosowanie poniższych kryteriów mogłoby uniemożliwić jakiekolwiek skorzystanie ze strony: 1.4.2 - Kontrola odtwarzania dźwięku, 2.1.2 - Brak pułapki na klawiaturę, 2.3.1 Trzy błyski lub wartości poniżej progu, 2.2.2: Wstrzymywanie (pauza), zatrzymywanie, ukrywanie.

## Uzasadnienie metody badania
Określić, czy i w jaki sposób użytkownik może modyfikować ograniczenia czasowe, automatyczne odtwarzanie i automatyczną aktualizację.

## Ograniczenia, założenia lub wyjątki
- Ograniczenie czasu z powodów spełniajacych którekolwiek z poniższych kryteriów nie jest uwzględniane w tym teście:
    -   **Wyjątek dotyczący czasu rzeczywistego:** Limit czasowy jest wymaganym komponentem jakiejś czynności w czasie rzeczywistym (np. aukcji) i nie ma możliwości zmiany limitu, lub:
    -   **Wyjątek dotyczący istoty czynności:** Limit czasowy jest istotny i wydłużenie go anulowałoby lub zaburzałoby daną czynność, lub:
    -   **Wyjątek 20 godzin:** Limit czasowy przekracza 20 godzin.
-   Zmiana treści jest uważana za „przedstawianą równolegle z inną treścią”, gdy pojawia się obok innych treści. Na przykład dynamiczna aktualizacja migawek na dole lub z boku strony byłaby uważana za „przedstawianą równolegle”, gdy strona zawiera także wideo z wiadomościami i artykuły tekstowe (oba przykłady treści statycznej). Przycisk umożliwiający użytkownikom wstrzymanie zmiany treści nie będzie uważany za inną treść statyczną.
-   Poruszanie się, przesuwanie, migotanie lub automatyczna aktualizacja treści są uważane za „niezbędne”, jeżeli ich usunięcie zasadniczo zmieniłoby informacje lub funkcjonalność treści, a informacji i funkcjonalności nie można uzyskać w inny sposób, który byłby zgodny z wymogami dostępności.
-   Uwagi do KS 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie:
    -   *Uwaga 1*: Wytyczna 2.3 zawiera więcej informacji na temat treści migoczącej lub zawierającej błyski..
    -   *Uwaga 2*: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi skorzystanie z całej strony, cała zawartość danej strony (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić powyższe kryterium. Więcej informacji: [Wymogi zgodności: 5. Brak zakłóceń](https://www.w3.org/TR/WCAG20/#cc5)
    -   *Uwaga 3*: Treść, która jest aktualizowana okresowo przez aplikację lub przesyłana w sposób ciągły do programu użytkownika, nie musi być przechowywana lub przedstawiana, w czasie pomiędzy wstrzymaniem a wznowieniem prezentacji, ponieważ może to być technicznie nie możliwe, a w wielu przypadkach mogłoby wprowadzać użytkownika w błąd.
    -   *Uwaga 4*: Animacja, która pojawia się w czasie poprzedzającym załadowanie treści, może być uznana za istotną, jeśli wszyscy użytkownicy nie mogą dokonać interakcji w tym czasie oraz jeśli brak wskazania etapu załadowania mógłby wprowadzić użytkownika w błąd lub mogłoby mu się wydawać, że załadowanie treści zostało zawieszone albo przerwane..
-   Uwaga do KS 1.4.2 Kontrola odtwarzania dźwięku:
    -   *Uwaga 1*: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi odczytanie całej strony, wszelkie treści na stronie (bez względu na to, czy spełniają inne kryteria sukcesu, czy nie) muszą spełnić niniejsze kryterium. Więcej informacji: [Wymogi zgodności: 5. Brak zakłóceń](https://www.w3.org/TR/WCAG20/#cc5)

## Procedura testu dla KS 2.2.1 Możliwość dostosowania czasu

### Identyfikacja treści
Wszelkie przypadki ograniczeń czasowych treści (z wyjątkiem wyjątków opisanych powyżej).

### Instrukcja testowania
Dla każdego wystąpienia ograniczonego czasu :
1.  Przed upływem limitu czasu sprawdź, czy spełniono przynajmniej jeden z poniższych warunków:
    -  Użytkownik ma możliwość wyłączenia limitu czasu.
    -  Użytkownik ma możliwość zwiększenia limitu czasu przed jego przekroczeniem o wartość co najmniej dziesięciokrotnie większą od wartości domyślnej.
    -  Użytkownik jest ostrzegany przed upłynięciem limitu czasowego **ORAZ**:
        -   ma przynajmniej 20 sekund na wydłużenie limitu za pomocą prostej czynności (np. „wciśnij klawisz spacji”), **ORAZ**
        -   może wydłużyć limit przynajmniej dziesięciokrotnie.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 2.2.1  oraz Wymaganie podstawowe nr 21 kończy się niepowodzeniem.

## Procedura testu dla KS 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie

### Poruszanie, przesuwanie, migotanie, przewijanie informacji

#### Identyfikacja treści
Wszelkie ruchome, migające lub przewijane informacje, które spełniają WSZYSTKIE z poniższych kryteriów:
-   uruchamiają się automatycznie **ORAZ**
-   trwają dłużej niż 5 sekund, **ORAZ**
-   Są prezentowane równolegle z innymi treściami, **ORAZ**
-   Ich poruszanie, przesuwanie, migotanie nie jest konieczne

#### Instrukcja testowania
1.  Sprawdź, czy istnieje mechanizm umożliwiający użytkownikowi ich wstrzymanie, zatrzymanie lub ukrycie.

### Wynik testów
Jeżeli powyższa próba zakończy się niepowodzeniem, wówczas test KS 2.2.2  oraz Wymaganie podstawowe nr 21 kończy się niepowodzeniem.

### Automatyczna aktualizacja treści

#### Identyfikacja treści
Wszelkie treści, które aktualizują się automatycznie, spełniające WSZYSTKIE poniższe kryteria:
-   aktualizacja uruchamia się automatycznie **ORAZ**
-   są prezentowane równolegle z innymi treściami, **ORAZ**
-   nie są częścią koniecznego działania.

#### Instrukcja testowania
1.  Sprawdź, czy istnieje mechanizm umożliwiający użytkownikowi
    - wstrzymanie, zatrzymanie lub ukrycie **ALBO**
	- kontrolowanie częstotliwości aktualizacji.

#### Wynik testów
Jeżeli powyższa próba zakończy się niepowodzeniem, wówczas test KS 2.2.2, Wymaganie zgodności nr 5 oraz Wymaganie podstawowe nr 21 kończy się niepowodzeniem.

## Procedura testu dla KS 1.4.2 Kontrola odtwarzania dźwięku

### Identyfikacja treści
Elementy strony odtwarzajace dźwięk dłużej niż 3 sekundy.

### Instrukcja testowania
1.  Sprawdź jedną z poniższych możliwości
    1.  na poczatku strony dostępny lub w funkcjach dostępu do platformy dostępny jest mechanizm wstrzymania lub zatrzymania dźwięku, **ALBO**
    2.  na poczatku strony dostępny lub w funkcjach dostępu do platformy dostępny jest mechanizm regulacji głośności niezależny od ogólnego poziomu głośności systemu.

### Wynik testów
Jeżeli powyższa próba zakończy się niepowodzeniem, wówczas test KS  1.4.2, Wymaganie zgodności nr 5: Brak zakłóceń oraz Wymaganie podstawowe nr 21 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego

-   Przypomnij testerom, że w przypadku przekroczenia limitu czasu wskaźnik fokusu powinien powinien się przemieścić  do komunikatu o limicie czasu, aby spełnić kryteria sukcesu dotyczące dostępności klawiatury i kolejności fokusu.
-   W niektórych przypadkach może być konieczne skontaktowanie się z autorami aplikacji w celu wyjaśnienia warunków przekroczenia limitu czasu.
-   Defekty KS 1.4.2 lub 2.2.2 również powodują niespełnienie Wymogu zgodności 5: Brak zakłóceń i powinny być zaznaczone w raporcie z testów, aby wskazać poważny wpływ na dostępność.
-   Przed rozpoczęciem testu przeglądarki muszą być skonfigurowane tak, aby zezwalały na odtwarzanie dźwięku. Wyniki testu mogą zależeć od przeglądarki.

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G198.md %}
- {% include techniki/G180.md %}
- {% include techniki/SCR16.md %} ORAZ {% include techniki/SCR1.md %}
- {% include techniki/G4.md %}
- {% include techniki/SCR33.md %}
- {% include techniki/SCR36.md %}
- {% include techniki/G170.md %}
- {% include techniki/G60.md %}
- {% include techniki/G171.md %}
- {% include techniki/G186.md %}
