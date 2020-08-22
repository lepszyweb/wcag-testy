---
title: 3. Kolejność fokusu


sidebar: testy_sidebar
permalink: ICT-03-kolejnosc-fokusu
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/2-4-3.md %}  
- {% include ks/3-2-1.md %}  

## Uzasadnienie metody badania
Korzystanie z klawiatury do nawigacji ułatwia kontrolę kolejności ustawiania fokusu.

## Ograniczenia, założenia lub wyjątki
-   Fokus może zostać przeniesiony do kontrolki albo za pomocą klawiatury (np. klawisz Tab), albo myszy (np. kliknięcie pola tekstowego). Przesunięcie myszy nad formantem nie powoduje przeniesienia fokusu, chyba że takie zachowanie zostanie zaimplementowane w skrypcie.
-   Chociaż jest to powszechna i najlepsza praktyka dla niektórych osób, nie jest wymagane ustawianie fokusu w kolejności od lewej do prawej strony, od góry do dołu.
-   Bez wyjątku fokus musi przejść do wszystkich modalnych okien dialogowych i pozostawać w oknie dialogowym, dopóki użytkownik nie zamknie okna.
-   Technologia wspomagająca będzie przetwarzać regiony aria na żywo bez zmiany fokusu. Żywe regiony (dynamiczne), które nie zawierają treści interaktywnych, nie wymagają zmiany fokusu i i nie są uwzględnione w tym teście.
-   W przypadku niektórych typów elementów sterujących kliknięcie elementu sterującego może również aktywować element sterujący (np. przycisk), co z kolei może zainicjować zmianę kontekstu. Elementy sterujące, których wyraźnym celem jest zainicjowanie zmiany kontekstu, nie powodują niepowodzenia tego testu.
-   W tym teście ocenia się KS 3.2.1 Po oznaczeniu fokusem, wyłącznie przy użyciu klawiatury, aby uniknąć niezamierzonego uruchomienia elementów sterujących za pomocą myszy.
-   [Zmiana kontekstu](https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-receive-focus.html#context-changedef) została zdefiniowana na stronie [Objaśnienie KS 3.2.1: Po oznaczeniu fokusem](https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-receive-focus.html) jako: znaczące zmiany treści \[strony internetowej\], które dokonywane bez świadomości użytkownika, mogą go dezorientować, jeżeli nie jest on w stanie oglądać całej strony jednocześnie. Zmiany kontekstu obejmują zmiany::
    1.  W programie użytkownika (przeglądarce, itp.)
    2.  Obszaru operacyjnego
    3.  fokusu
    4.  Treści, która zmienia sens \[strony internetowej\].
-   **Uwaga:** Zmiana treści nie zawsze oznacza zmianę kontekstu. Zmiana w treści, na przykład rozwinięcie drzewa, dynamicznego menu lub zakładki niekoniecznie zmieniają kontekst, dopóki nie zmienią jednego z powyższych (np. fokusu).
-   **Przykład zmiany kontekstu**: Otwarcie nowego okna, przeniesienie fokusu na inny obiekt, przejście na inną stronę internetową (włączając w to także każdą sytuację, kiedy użytkownikowi tylko wydaje się, że przechodzi na inną stronę internetową) lub znaczące przekształcenie wyglądu strony są przykładami zmiany kontekstu.

## Procedura testu dla KS 2.4.3 Kolejność fokusu

### Identyfikacja treści
Komponenty interfejsu dostępne dla klawiatury (np. łącza, pola formularzy, rozwijane menu, treść rozwijana/zwijana treści, widoki drzewa, okienka pop-up/light box, ramki, iframes), które mają znaczącą sekwencję nawigacji.

### Instrukcja testowania
1.  Użyj klawiatury, aby poruszać się po komponentach interfejsu.
    1.  Za pomocą klawiatury aktywuj elementy wyzwalające, które odkrywają schowaną treść (np. menu, okna dialogowe, rozwijana lista drzewa).
        1.  Sprawdź, czy wskaźnik fokusu został przeniesiony na odsłoniętą treść. (Dopuszczalne jest jednokrotne użycie TAB lub użycie klawisza strzałki, aby przesunąć fokus w przód do odsłoniętej zawartości).
        2.  Przesuwaj fokus w odsłoniętej treści.
    2.  Użyj klawiatury, aby zamknąć/ukryć odsłoniętą treść.
        1.  Sprawdź, czy fokus powrócił do elementu wyzwalającego. (Dopuszczalne jest jednokrotne użycie przycisku [Shift+ TAB\] lub użycie klawisza strzałki, aby przesunąć fokus w tył do elementu wyzwalającego.
2.  Sprawdź, czy kolejność ustawiania fokusu zachowuje znaczenie i użyteczność strony.

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
    -   Przeniesienie fokusu na inny komponent interfejsu.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.2.1 oraz wymaganie podstawowe nr 3 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
-   Kolejność tabulacji, która początkowo wydaje się nielogiczna, może nadal spełniać to wymaganie ze względu na logikę biznesową specyficzną dla danej aplikacji.
-   Przydatne może być połączenie tych testów z testami nawigacji klawiatury i widoczności fokusu.
-   Przydatne może być przekazanie testerowi instrukcji na temat tego, czym są „modalne okna dialogowe” i jak powinny się zachowywać.

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G59.md %}
- {% include techniki/H4.md %}
- {% include techniki/G107.md %}
- {% include techniki/F55.md %}
- {% include techniki/SCR26.md %}
- {% include techniki/F85.md %}
