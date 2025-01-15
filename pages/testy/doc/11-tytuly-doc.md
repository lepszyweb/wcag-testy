---
title: 11. Tytuły dokumentów (dokumenty)
last_updated: 16 stycznia 2025

sidebar: testy_sidebar
permalink: 11-tytuly-doc
folder: testy/doc
---


## Wymagania dostępności
- {% include ks/2-4-2.md %}

## Uzasadnienie metody testowej
Właściwość Tytuł definiuje tytuł dokumentu i jest wymagana we wszystkich dokumentach. Ten test sprawdza istnienie opisowego tytułu dokumentu.

## Ograniczenia, założenia lub wyjątki
-   Każdy dokument musi mieć opisowy tytuł. Ten test jest zawsze obowiązkowy.
-	Test ten ma zastosowanie do wszystkich dokumentów w zbiorze dokumentów (np. portfolio PDF).


## 11.A Procedura testowania tytułów stron
Identyfikator testu podstawowego: _11.A-PageTitled_

### Identyfikacja treści
<p id="d11aIC">Właściwość Tytuł dokumentu.</p>

### Instrukcja testowania

1.  Sprawdź, czy właściwość Tytuł dokumentu jest zdefiniowana dla tego dokumentu. [KS 2.4.2]
2.  Sprawdź, czy tytuł dokumentu opisuje jego treść lub przeznaczenie. [KS 2.4.2]

### Wynik testów
<p id="d11aTR">Jeżeli którakolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test podstawowy <em>11.A-PageTitled</em> kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesów testowych
Brak

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G88.md %}
- {% include techniki/H25.md %}
- {% include techniki/PDF18.md %}
- {% include techniki/F25.md %}
