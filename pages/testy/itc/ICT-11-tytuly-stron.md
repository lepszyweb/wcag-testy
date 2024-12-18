---
title: 11. Tytuły stron
last_updated: 22 października 2024

sidebar: testy_sidebar
permalink: ICT-11-tytuly-stron
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/2-4-2.md %}

## Uzasadnienie metody testowej
Element `<title>` definiuje tytuł dokumentu i jest wymagany we wszystkich dokumentach HTML/XHTML. Ten test sprawdza istnienie opisowego tytułu dla strony internetowej.

## Ograniczenia, założenia lub wyjątki
-   Każda strona internetowa musi mieć opisowy tytuł. Ten test jest zawsze obowiązkowy.
-   Element `<title>` w tym teście różni się od atrybutu *title* używanego do dodawania podpowiedzi/dodatkowych informacji o elemencie.
-   Niektóre aplikacje internetowe i inne niż internetowe mogą zawierać treści, które zmieniają się dynamicznie. W takich przypadkach tytuł strony powinien wystarczająco opisywać zmieniony cel aplikacji.
-   [Specyfikacja HTML5](https://www.w3.org/TR/html50/document-metadata.html#the-title-element) stanowi, że dokument HTML powinien mieć tylko jeden element `<title>` ORAZ że element `<title>` powinien być dzieckiem elementu `<head>`. Ale w praktyce wszystkie nowoczesne przeglądarki korygują błędy składniowe związane z lokalizacją i zagnieżdżaniem elementu `<title>`. Oznacza to, że nawet jeśli w kodzie strony zostanie umieszczonych więcej niż jeden element `<title>`, to programy korzystające z Obiektowego Modelu Dokumentu (DOM) umieszczą element `<title>` w prawidłowej lokalizacji i zazwyczaj będą przedstawiać użytkownikowi tylko pierwszy element `<title>` (jeśli jest więcej niż jeden).


## 11.A Procedura testowania tytułów stron
Identyfikator testu podstawowego: _11.A-PageTitled_

### Identyfikacja treści
Znajdź pierwszy znacznik `<title>` odnoszący się do strony.

### Instrukcja testowania

1.  Sprawdź, czy dla strony jest zdefiniowany element &lt;title&gt;.
2.  Sprawdź, czy tytuł strony opisuje treść lub przeznaczenie strony internetowej.
    1.  W przypadku stron w witrynie internetowej sprawdź, czy po tytułach stron można je rozróżniać.
    2.  W przypadku dokumentów lub aplikacji internetowych, do opisania celu wystarcza nazwa dokumentu lub aplikacji internetowej.

### Wynik testów
Jeżeli którakolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test podstawowy _11.A-PageTitled_ kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesów testowych
Brak

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G88.md %}
- {% include techniki/H25.md %}
- {% include techniki/F25.md %}
