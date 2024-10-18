---
title: 2. Fokus


sidebar: testy_sidebar
permalink: ICT-02-fokus
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/2-4-3.md %}  
- {% include ks/2-4-7.md %}
- {% include ks/3-2-1.md %}   

## Objaśnienie metody badania
Ręczne nawigowanie lub sterowanie komponentami interfejsu tylko za pomocą samej klawiatury umożliwi testerowi rozpoznanie, kiedy nie ma wizualnego rozróżnienia między elementem z fokusem a resztą dokumentu. Korzystanie z&nbsp; klawiatury do nawigacji ułatwia kontrolę kolejności ustawiania fokusu.

## Ograniczenia, założenia lub wyjątki

-   W porządku tabulacji mogą znajdować się niektóre elementy interfejsu, które zwykle nie są uważane za interaktywne (np. tekst okna z instrukcją wypełniania formularzy). Takie komponenty interfejsu powinny otrzymywać widoczny fokus, gdy użytkownik nawiguje do nich za pomocą klawiatury.
-   Podczas ręcznego przenoszenia fokusu przez stronę (za pomocą <kbd>Tab</kbd> lub klawiszy strzałek) nie powinna wystąpić utrata widocznego fokusu. Jednak po uruchomieniu funkcji, która przemieszcza fokus (np. odsłonięcie wewnętrznego łącza strony lub ukrytej treści), może być konieczne ręczne przesunięcie fokusu za pomocą klawiatury, zanim fokus stanie się ponownie widoczny. Nie jest to uważane za naruszenie.
-   Fokus można przenieść do kontrolki albo za pomocą klawiatury (np. klawiszem Tab), albo myszy (np. kliknięcie pola tekstowego). Przesunięcie wskaźnika myszy nad kontrolkę nie powoduje przeniesienia fokusu, chyba że takie zachowanie zostanie zaimplementowane w skrypcie.
-   Chociaż jest to powszechna i najlepsza praktyka dla niektórych osób, nie jest wymagane ustawianie fokusu w kolejności od lewej do prawej strony, od góry do dołu.
-   Kolejność fokusu dotyczy nawigacji do przodu i do tyłu.
-   Bez wyjątku fokus musi musi zostać przeniesiony do modalnych okien dialogowych i pozostawać w oknie dialogowym, dopóki użytkownik nie zamknie okna.
-   W przypadku niektórych typów kontrolek kliknięcie kontrolki może również uaktywnić kontrolkę (np. przycisk), co z kolei może zainicjować zmianę kontekstu. Kontrolki, które są wyraźnie oznaczone i&nbsp;mają na celu zainicjowanie zmiany kontekstu, nie powodują niepowodzenia tego testu.
-   W tym teście ocenia się KS 3.2.1 Po oznaczeniu fokusem, wyłącznie przy użyciu klawiatury, aby uniknąć niezamierzonego uruchomienia kontrolek za pomocą myszy.
-   Częścią tego testu jest także widoczność fokusu na łączach pomijających.
<!-- 
-   Przełączanie fokusu na odkrywane treści nie jest tutaj testowane. Zobacz [5. Treść zmienna](testy/ICT_05_tresc-zmienna)
-   Technologia wspomagająca będzie przetwarzać regiony aria na żywo bez zmiany fokusu. Żywe regiony (dynamiczne), które nie zawierają treści interaktywnych, nie wymagają zmiany fokusu i nie są uwzględnione w tym teście.
-->
-   [Zmiana kontekstu](https://wcag.irdpl.pl/understanding/po-otrzymaniu-fokusu.html#dfn-zmiana-kontekstu) została zdefiniowana na stronie [Objaśnienie KS 3.2.1: Po otrzymaniu fokusu](https://wcag.irdpl.pl/understanding/po-otrzymaniu-fokusu.html) jako: duże zmiany, dokonywane bez świadomości użytkowników, które mogą ich dezorientować, gdy nie są w stanie przeglądać całej strony jednocześnie. Zmiany kontekstu obejmują zmiany::
    1.  w programie użytkownika (przeglądarce, itp.)
    2.  obszaru operacyjnego
    3.  fokusu
    4.  treści, która zmienia sens strony internetowej..
-   **Uwaga:** Zmiana treści nie zawsze oznacza zmianę kontekstu. Zmiany treści, na przykład rozwinięcie drzewa, dynamicznego menu lub zakładki niekoniecznie zmieniają kontekst, dopóki nie zmienią jednego z powyższych (np. fokusu)..
-   **Przykład zmiany kontekstu**: Otwarcie nowego okna, przeniesienie fokusu na inny obiekt, przejście na inną stronę internetową (włączając w to także każdą sytuację, kiedy użytkownikowi tylko wydaje się, że przechodzi na inną stronę internetową) lub znaczące przekształcenie wyglądu strony są przykładami zmiany kontekstu.

## Procedura testu dla KS 2.4.7 Widoczny fokus
Identyfikator testu bazowego: *2.A-FocusVisible*

### Identyfikacja treści

Komponenty interfejsu dostępne dla klawiatury (np. łącza, pola formularzy, menu rozwijane, odsłanianie/ukrywanie treści, widoki drzewa, wyskakujące okienka).

### Instrukcja testowania
1.  Użyj klawiatury, aby poruszać się po każdym komponencie interfejsu.
2.  Sprawdź, czy widoczny jest graficzny wskaźnik fokusu, gdy fokus znajduje się na komponencie interfejsu. Wskaźnik fokusu nie może być ograniczony czasowo; dopóki komponent ma fokus klawiatury, wskaźnik fokusu musi pozostać widoczny [KS 2.4.7].

### Wynik testów
-   Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test *2.A-FocusVisible* kończy się niepowodzeniem.

## Procedura testu dla KS 2.4.3 Kolejność fokusu
Identyfikator testu bazowego: *2.B-FocusOrder*

### Identyfikacja treści
Komponenty interfejsu dostępne dla klawiatury (np. łącza, pola formularzy, menu rozwijane, odsłanianie/ukrywanie treści, widoki drzewa, wyskakujące okienka, itp.), których kolejność w sekwencji nawigacji ma znaczenie dla zachowania sensu i funkcjonalności treści.


### Instrukcja testowania
1.  Użyj klawiatury, aby poruszać się po komponentach strony.
    1.  Za pomocą klawiatury aktywuj kontrolki wyzwalające, które odkrywają schowaną treść (np. menu, okna dialogowe, rozwijana lista drzewa).
        1.  Sprawdź, czy wskaźnik fokusu można przenieść na odsłoniętą treść. (Dopuszczalne jest jednokrotne użycie TAB lub użycie klawisza strzałki, aby przesunąć fokus w przód do odsłoniętej zawartości).
        2.  Przesuwaj fokus w odsłoniętej treści.
    2.  Użyj klawiatury, aby zamknąć/ukryć odsłoniętą treść.
        1.  Sprawdź, czy fokus powrócił do kontrolki wyzwalającej. (Dopuszczalne jest jednokrotne użycie kombinacji klawiszy <kbd>Shift+ TAB</kbd> lub użycie <kbd>strzałki</kbd>, aby przesunąć fokus w tył do elementu wyzwalającego.
2.  Sprawdź, czy kolejność ustawiania fokusu zachowuje znaczenie i użyteczność strony. [KS 2.4.3]

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test podstawowy *2.B-FocusOrder* kończy się niepowodzeniem.

## Procedura testu dla KS 3.2.1 Po otrzymaniu fokusu
Identyfikator testu podstawowego: *2.C-OnFocus*

### Identyfikacja treści
Komponenty interfejsu dostępne dla klawiatury (np. łącza, pola formularzy, menu rozwijane, odsłanianie/ukrywanie treści, widoki drzewa, wyskakujące okienka, itp.).

### Instrukcja testowania
1.  Użyj klawiatury, aby przenosić fokus i przejść na stronie przez każdy komponent interaktywny (w tym pola formularzy i listy rozwijane formularzy).
2.  Sprawdź, czy gdy komponent otrzymuje fokus, nie inicjuje to nieoczekiwanej zmiany kontekstu. Przykłady zmiany kontekstu obejmują:
    -   Automatyczne przesłanie formularza, gdy komponent otrzyma fokus.
    -   Uruchamienie nowego okna, gdy komponent otrzyma fokus.
    -   Przeniesienie fokusu na inny komponent interfejsu.

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy *2.C-OnFocus* kończy się niepowodzeniem.


##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

-   Wyrazistość widocznego fokusu jest subiektywna, a minimalnym poziomem jest domyślne ustawienie  przeglądarki (lub platformy systemu operacyjnego) do wskazywania fokusu. Aplikacje mogą również inaczej przedstawiać fokus w określonych sytuacjach.
-   Wskaźnik fokusu może przybierać różne formy: obramowania elementu, migającego kursora w polu tekstowym, wizualnej zmiany wyglądu przycisku.
-   Ten test można przeprowadzić równocześnie z testem [1. Dostęp z klawiatury](testy/ICT_01_klawiatura.md).
-   Podczas testowania nie powinny być włączone żadne modyfikacje fokusu w środowisku testowym. Niektóre narzędzia testowe dodają widoczny kontur wokół elementów, które otrzymują fokus. Chociaż narzędzia testujące mogą pomóc testerom w śledzeniu fokusu, żadne wskaźniki dostarczone przez narzędzie testujące nie powinny być używane jako wskaźniki widoczności fokusu potwierdzające spełnienia tego wymagania.
-   Biorąc pod uwagę zmienność sposobu, w jaki przeglądarki mogą prezentować fokus w określonych sytuacjach, raporty z testów powinny zawierać szczegółowe informacje o środowisku testowym, w tym o przeglądarce i jej wersji.
-   Kolejność tabulacji, która początkowo wydaje się nielogiczna, może nadal spełniać to wymaganie ze względu na logikę biznesową specyficzną dla danej aplikacji.
-   Przydatne może być połączenie tych testów z testami nawigacji klawiatury i widoczności fokusu.
-   Przydatne może być przekazanie testerowi instrukcji na temat tego, czym są „modalne okna dialogowe” i jak powinny się zachowywać.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/F55.md %}
- {% include techniki/F85.md %}
- {% include techniki/F78.md %}
- {% include techniki/G59.md %}
- {% include techniki/G107.md %}
- {% include techniki/G149.md %}
- {% include techniki/G165.md %}
- {% include techniki/G195.md %}
- {% include techniki/SCR26.md %}
- {% include techniki/PDF3.md %}
- {% include techniki/C15.md %}
- {% include techniki/SCR31.md %}





