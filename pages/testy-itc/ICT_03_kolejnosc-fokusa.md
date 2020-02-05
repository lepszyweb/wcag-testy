---
title: 3. Kolejność fokusa


sidebar: testy-itc_sidebar
permalink: ICT_03_kolejnosc-fokusa
folder: testy-itc
---

## Wymagania dostępności
-   [KS WCAG: 2.4.3 Kolejność fokusa](https://wcag.lepszyweb.pl/#focus-order) -- Jeśli strona internetowa może być nawigowana sekwencyjnie, a kolejność nawigacji wpływa na zrozumienie lub funkcjonalność strony, komponenty przyjmujące fokus zachowują kolejność, dzięki której zachowany jest sens i funkcjonalność treści.
-   [KS WCAG: 3.2.1 Po oznaczeniu fokusem](https://wcag.lepszyweb.pl/#on-focus) -- Jeśli jakikolwiek komponent jest oznaczony fokusem, nie powoduje to zmiany kontekstu.

## Uzasadnienie metody badania
Korzystanie z klawiatury do nawigacji ułatwia kontrolę kolejności ustawiania fokusa.

## Ograniczenia, założenia lub wyjątki
-   Fokus może zostać przeniesiony do kontrolki albo za pomocą klawiatury (np. klawisz Tab), albo myszy (np. kliknięcie pola tekstowego). Przesunięcie myszy nad formantem nie powoduje przeniesienia fokusa, chyba że takie zachowanie zostanie zaimplementowane w skrypcie.
-   Chociaż jest to powszechna i najlepsza praktyka dla niektórych osób, nie jest wymagane ustawianie fokusa w kolejności od lewej do prawej strony, od góry do dołu.
-   Bez wyjątku fokus musi przejść do wszystkich modalnych okien dialogowych i pozostawać w oknie dialogowym, dopóki użytkownik nie zamknie okna.
-   Technologia wspomagająca będzie przetwarzać regiony aria na żywo bez zmiany fokusa. Żywe regiony (dynamiczne), które nie zawierają treści interaktywnych, nie wymagają zmiany fokusa i i nie są uwzględnione w tym teście.
-   W przypadku niektórych typów elementów sterujących kliknięcie elementu sterującego może również aktywować element sterujący (np. przycisk), co z kolei może zainicjować zmianę kontekstu. Elementy sterujące, których wyraźnym celem jest zainicjowanie zmiany kontekstu, nie powodują niepowodzenia tego testu.
-   W tym teście ocenia się KS 3.2.1 Po oznaczeniu fokusem, wyłącznie przy użyciu klawiatury, aby uniknąć niezamierzonego uruchomienia elementów sterujących za pomocą myszy.
-   [Zmiana kontekstu](https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-receive-focus.html#context-changedef) została zdefiniowana na stronie [Objaśnienie KS 3.2.1: Po oznaczeniu fokusem](https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-receive-focus.html) jako: znaczące zmiany treści \[strony internetowej\], które dokonywane bez świadomości użytkownika, mogą go dezorientować, jeżeli nie jest on w stanie oglądać całej strony jednocześnie. Zmiany kontekstu obejmują zmiany::
    1.  W programie użytkownika (przeglądarce, itp.)
    2.  Obszaru operacyjnego
    3.  Fokusa
    4.  Treści, która zmienia sens \[strony internetowej\].
-   **Uwaga:** Zmiana treści nie zawsze oznacza zmianę kontekstu. Zmiana w treści, na przykład rozwinięcie drzewa, dynamicznego menu lub zakładki niekoniecznie zmieniają kontekst, dopóki nie zmienią jednego z powyższych (np. fokusa).
-   **Przykład zmiany kontekstu**: Otwarcie nowego okna, przeniesienie fokusa na inny obiekt, przejście na inną stronę internetową (włączając w to także każdą sytuację, kiedy użytkownikowi tylko wydaje się, że przechodzi na inną stronę internetową) lub znaczące przekształcenie wyglądu strony są przykładami zmiany kontekstu.

## Procedura testu dla KS 2.4.3 Kolejność fokusa

### Identyfikacja treści
Komponenty interfejsu dostępne dla klawiatury (np. łącza, pola formularzy, rozwijane menu, treść rozwijana/zwijana treści, widoki drzewa, okienka pop-up/light box, ramki, iframes), które mają znaczącą sekwencję nawigacji.

### Instrukcja testowania
1.  Użyj klawiatury, aby poruszać się po komponentach interfejsu.
    1.  Za pomocą klawiatury aktywuj elementy wyzwalające, które odkrywają schowaną treść (np. menu, okna dialogowe, rozwijana lista drzewa).
        1.  Sprawdź, czy wskaźnik fokusa został przeniesiony na odsłoniętą treść. (Dopuszczalne jest jednokrotne użycie TAB lub użycie klawisza strzałki, aby przesunąć fokus w przód do odsłoniętej zawartości).
        2.  Przesuwaj fokus w odsłoniętej treści.
    2.  Użyj klawiatury, aby zamknąć/ukryć odsłoniętą treść.
        1.  Sprawdź, czy fokus powrócił do elementu wyzwalającego. (Dopuszczalne jest jednokrotne użycie przycisku [Shift+ TAB\] lub użycie klawisza strzałki, aby przesunąć fokus w tył do elementu wyzwalającego.
2.  Sprawdź, czy kolejność ustawiania fokusa zachowuje znaczenie i użyteczność strony.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 2.4.3 oraz wymaganie podstawowe nr 3 kończy się niepowodzeniem.

## Procedura testu dla KS 3.2.1 Po oznaczeniu fokusem

### Identyfikacja treści
Komponenty interfejsu dostępne dla klawiatury (np. łącza, pola formularzy, rozwijane menu, treść rozwijana/zwijana treści, widoki drzewa, okienka pop-up/light box, ramki, iframes).

### Instrukcja testowania
1.  Użyj klawiatury, aby przenieść fokus i przejść przez każdy komponent interaktywnego interfejsu (w tym listy rozwijane formularzy i pola formularzy).
2.  Sprawdź, czy gdy komponent otrzymuje fokus, nie powoduje to nieoczekiwanej zmiany kontekstu. Przykłady zmiany kontekstu obejmują:
    -   Automatyczne przesłanie formularza, gdy komponent otrzyma fokus.
    -   Uruchamienie nowego okna, gdy komponent otrzyma fokus.
    -   Przeniesienie fokusa na inny komponent interfejsu.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.2.1 oraz wymaganie podstawowe nr 3 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
-   Kolejność tabulacji, która początkowo wydaje się nielogiczna, może nadal spełniać to wymaganie ze względu na logikę biznesową specyficzną dla danej aplikacji.
-   Przydatne może być połączenie tych testów z testami nawigacji klawiatury i widoczności fokusa.
-   Przydatne może być przekazanie testerowi instrukcji na temat tego, czym są „modalne okna dialogowe” i jak powinny się zachowywać.

## Techniki WCAG 2.1
-   Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
    -   [G59: Umieszczanie elementów interaktywnych w kolejności podążającej za sekwencjami i relacjami w obrębie treści](http://www.w3.org/TR/WCAG20-TECHS/G59.html)
    -   [H4: Tworzenie logicznej kolejności tabulacji poprzez łącza, formanty formularzy i obiekty](http://www.w3.org/TR/WCAG20-TECHS/H4.html)
    -   [G107: Używanie raczej &bdquo;aktywuj&bdquo; niż &bdquo;focus&bdquo; jako polecenia uruchamiającego zmiany kontekstu](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/G107)
    -   [F55: Niespełnienie kryterium sukcesu 2.1.1, 2.4.7 i 3.2.1 z powodu użycia skryptu do usunięcia wskaźnika fokusa po otrzymaniu fokusa](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/F55)
    -   [SCR26: Wstawianie dynamicznej zawartości do modelu obiektów dokumentu bezpośrednio po elemencie wyzwalającym](https://www.w3.org/TR/WCAG20-TECHS/SCR26.html)
    -   [F85: Niespełnienie kryterium sukcesu 2.4.3 z powodu używania okien dialogowych lub menu, które nie sąsiadują z ich kontrolą wyzwalania w kolejności sekwencyjnej nawigacji](https://www.w3.org/TR/WCAG20-TECHS/F85.html)


