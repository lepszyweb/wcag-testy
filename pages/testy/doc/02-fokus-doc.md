---
title: 2. Fokus (dokumenty)
last_updated: 15 stycznia 2025

sidebar: testy_sidebar
permalink: 02-fokus-doc
folder: testy/doc
---

## 2. Fokus

## Wymagania dostępności
- {% include ks/2-4-3.md %}  
- {% include ks/2-4-7.md %}
- {% include ks/3-2-1.md %}   

## Uzasadnienie metody testowej
Ręczne nawigowanie po komponentach dokumentu lub sterowanie nimi za pomocą samej klawiatury umożliwi testerowi  rozpoznanie,  kiedy nie ma wizualnego rozróżnienia między elementem z fokusem a resztą dokumentu. Korzystanie z&nbsp; klawiatury do nawigacji ułatwia kontrolę kolejności ustawiania fokusu.

## Ograniczenia, założenia lub wyjątki

-   W porządku tabulacji mogą znajdować się niektóre elementy interfejsu, które zwykle nie są uważane za interaktywne (np. tekst okna z instrukcją wypełniania formularzy). Takie komponenty interfejsu powinny otrzymywać widoczny wskaźnik fokusu, gdy użytkownik nawiguje do nich za pomocą klawiatury.
-   Podczas ręcznego przenoszenia fokusu przez stronę (za pomocą <kbd>Tab</kbd> lub klawiszy strzałek) nie powinna wystąpić utrata widocznego fokusu. Jednak w przypadku wykonania funkcji, która przemieszcza fokus (np. wybór wewnętrznego łącza do elementu strony lub odsłonięcie ukrytej treści), może być konieczne ręczne przesunięcie fokusu za pomocą klawiatury, zanim fokus stanie się ponownie widoczny. Nie jest to uważane za naruszenie.
-   Fokus można przenieść do kontrolki albo za pomocą klawiatury (np. przechodząc do kontrolki za pomocą <kbd>Tab</kbd>) lub myszy (np. klikając pole tekstowe). Przesunięcie wskaźnika myszy na kontrolkę nie powoduje przeniesienia fokusu, chyba że takie zachowanie zostanie zaimplementowane w skrypcie.
-   Chociaż jest to powszechna i najlepsza praktyka, nie jest wymagane ustawianie fokusu w kolejności od lewej do prawej strony, od góry do dołu.
-   Kolejność fokusu obejmuje nawigację do przodu i do tyłu.
-   Bez wyjątku fokus musi zostać przeniesiony do modalnych okien dialogowych i pozostawać w oknie dialogowym, dopóki użytkownik nie zamknie okna.
-   W przypadku niektórych typów kontrolek kliknięcie kontrolki może również uaktywnić kontrolkę (np. przycisk), co z kolei może zainicjować zmianę kontekstu. Kontrolki, które są wyraźnie oznaczone i&nbsp;mają na celu zainicjowanie zmiany kontekstu, nie powodują niepowodzenia tego testu.
-   W tym teście ocenia się KS 3.2.1 Po oznaczeniu fokusem, wyłącznie przy użyciu klawiatury, aby uniknąć niezamierzonego uruchomienia kontrolek za pomocą myszy.
-   [Zmiana kontekstu](https://wcag.irdpl.pl/understanding/po-otrzymaniu-fokusu.html#dfn-zmiana-kontekstu) została zdefiniowana na stronie [Objaśnienie KS 3.2.1: Po otrzymaniu fokusu](https://wcag.irdpl.pl/understanding/po-otrzymaniu-fokusu.html) jako: poważne zmiany w treści, dokonywane bez świadomości użytkowników, które mogą ich dezorientować, gdy nie są w stanie przeglądać całej strony jednocześnie. Zmiany kontekstu obejmują zmiany:
    1.  w programie użytkownika (przeglądarce, itp.)
    2.  obszaru operacyjnego
    3.  fokusu
    4.  treści, która zmienia sens strony internetowej..
-   **Uwaga:** Zmiana treści nie zawsze oznacza zmianę kontekstu. Zmiany treści, takie jak rozwijany konspekt, dynamiczne menu lub zakładki niekoniecznie zmieniają kontekst, dopóki nie zmienią jednego z powyższych (np. fokusu).
-   **Przykłady zmiany kontekstu**: Otwarcie nowego okna, przeniesienie fokusu do innego komponentu, przejście do nowego dokumentu lub okna (w tym wszystkiego, co dla użytkownika wyglądałoby tak, jakby przeniósł się do nowego dokumentu) lub znacząca zmiana układu zawartości strony/ekranu.

## 2.A Procedura testowa widoczności fokusu
Identyfikator testu bazowego: *2.A-FocusVisible*

### Identyfikacja treści

<p id="d2aIC">Komponenty interfejsu dostępne za pomocą klawiatury (np. łącza, pola formularzy, menu rozwijane, pokazywanie/ukrywanie zawartości, widoki drzewa i wyskakujące okienka).</p>

### Instrukcja testowania

<ol id="d2aTI">
    <li id="d2aTI-1">Użyj klawiatury, aby poruszać się po każdym komponencie interfejsu.</li>
    <li id="d2aTI-2">Sprawdź, czy widoczny jest graficzny wskaźnik fokusu, gdy fokus znajduje się na komponencie interfejsu. Wskaźnik fokusu nie może być ograniczony czasowo; dopóki komponent ma fokus klawiatury, wskaźnik fokusu musi pozostać widoczny. [KS 2.4.7]</li>
</ol>

### Wynik testów
<p id="d2aTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test podstawowy  <em>2.A-FocusVisible</em> kończy się niepowodzeniem.</p>


## 2.B Procedura testowa kolejności fokusu
Identyfikator testu podstawowego: *2.B-FocusOrder*

### Identyfikacja treści
<p id="d2bIC">Komponenty dokumentu dostępne dla klawiatury (np. łącza, pola formularzy, menu rozwijane, odsłanianie/ukrywanie treści, widoki drzewa, wyskakujące okienka, itp.), których kolejność w&nbsp;sekwencji nawigacji ma znaczenie dla zachowania sensu i funkcjonalności treści.</p>

### Instrukcja testowania
1.  Użyj klawiatury, aby poruszać się po komponentach dokumentu.
    1.  Za pomocą klawiatury aktywuj kontrolki wyzwalające, które odkrywają schowaną treść (np. menu, okna dialogowe, rozwijana lista drzewa).
        1.  Sprawdź, czy odsłaniana treść, na której można ustawić fokus, jest uwzględniona w kolejności ustawiania fokusu. [KS 2.4.3] 
        2.  Przesuwaj fokus w odsłoniętej treści.
    2.  Użyj klawiatury, aby zamknąć/ukryć odsłoniętą treść.
        1.  Sprawdź, czy fokus powrócił do kontrolki wyzwalającej. (Dopuszczalne jest jednokrotne użycie kombinacji klawiszy <kbd>Shift+ TAB</kbd> lub użycie <kbd>strzałki</kbd>, aby przesunąć wskaźnik fokusu w tył do elementu wyzwalającego. [KS 2.4.3]
2.  Sprawdź, czy kolejność ustawiania fokusu zachowuje znaczenie i użyteczność dokumentu. [KS 2.4.3]

### Wynik testów
<p id="d2bTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test podstawowy <em>2.B-FocusOrder</em> kończy się niepowodzeniem.</p>

## 2.C Procedura testowania Po otrzymaniu fokusu
Identyfikator testu podstawowego: *2.C-OnFocus*

### Identyfikacja treści
<p id="d2cIC">Komponenty dokumentu dostępne dla klawiatury (np. łącza, pola formularzy, menu rozwijane, odsłanianie/ukrywanie treści, widoki drzewa, wyskakujące okienka, itp.).</p>


### Instrukcja testowania
1.  Użyj klawiatury, aby przenosić fokus i przejść w dokumencie przez każdy komponent interaktywny (w tym pola formularzy i listy rozwijane formularzy).
2.  Sprawdź, czy gdy komponent otrzymuje fokus, nie inicjuje to nieoczekiwanej zmiany kontekstu. [SC 3.2.1]
    -   Automatyczne przesłanie formularza, gdy komponent otrzyma fokus.
    -   Uruchomienie okna nowego dokumentu lub przeglądarki, gdy komponent otrzyma fokus.
    -   Przeniesienie fokusu na inny komponent interfejsu.

### Wynik testów
<p id="d2cTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>2.C-OnFocus</em> kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

-   Wyrazistość widocznego fokusu jest subiektywna, a minimalnym poziomem jest domyślne ustawienie  aplikacji (lub platformy systemu operacyjnego) do wskazywania fokusu. Aplikacje mogą również inaczej przedstawiać fokus w określonych sytuacjach.
-   Ten test można przeprowadzić równocześnie z testem [1. Dostęp z klawiatury](testy/01-klawiatura-doc.md).
-   Podczas testowania nie powinny być włączone żadne modyfikacje fokusu w środowisku testowym. Niektóre narzędzia testowe dodają widoczny kontur wokół elementów, które otrzymują fokus. Chociaż narzędzia testujące mogą pomóc testerom w śledzeniu fokusu, żadne wskaźniki dostarczone przez narzędzie testujące nie powinny być używane jako wskaźniki widoczności fokusu potwierdzające spełnienia tego wymagania.
-   Biorąc pod uwagę zmienność sposobu, w jaki aplikacje mogą prezentować fokus w określonych sytuacjach, raporty z testów powinny zawierać szczegółowe informacje o środowisku testowym, w tym o aplikacji i jej wersji.
-   Kolejność tabulacji, która początkowo wydaje się nielogiczna, może nadal spełniać to wymaganie ze względu na logikę biznesową specyficzną dla danej aplikacji.
-   Przydatne może być połączenie tych testów z testami nawigacji klawiatury i widoczności fokusu.
-   Przydatne może być przekazanie testerowi instrukcji na temat tego, czym są „modalne okna dialogowe” i jak powinny się zachowywać.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/F55.md %}
- {% include techniki/F85.md %}
- {% include techniki/G59.md %}
- {% include techniki/G107.md %}
- {% include techniki/G149.md %}
- {% include techniki/G165.md %}
- {% include techniki/G195.md %}
- {% include techniki/SCR26.md %}
- {% include techniki/PDF3.md %}

