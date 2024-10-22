---
title: 23. Wiele dróg
last_updated: 22 października 2024

sidebar: testy_sidebar
permalink: ICT-23-wiele-drog
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/2-4-5.md %}

## Uzasadnienie metody testowej
Ten test podstawowy wymaga ręcznego sprawdzenia kilku różnych technik służących lokalizacji strony w zestawie stron.

## Ograniczenia, założenia lub wyjątki

-   Wyjątki: strony internetowe, które są wynikiem lub krokiem w procesie, nie są uwzględniane w tym teście.

## 23.A Procedura testu dla powiązanych stron internetowych
Identyfikator testu podstawowego: _23.A-MultipleWays_

### Identyfikacja treści
Strony internetowe w zestawie powiązanych stron (witrynie).

### Instrukcja testowania
1.  Sprawdź, czy strona zapewnia dwa lub więcej sposobów znalezienia i dotarcia do żądanej strony w witrynie, na przykład za pomocą takich technik, jak:
    -   mapa witryny
    -   wyszukiwarka
    -   spis treści
    -   menu nawigacyjne lub menu rozwijane
    -   drzewa nawigacyjne
    -   łącza między stronami (poprzednia - następna)

### Wynik testów
Jeśli powyższy test zakończy się niepowodzeniem, test podstawowy _23.A-MultipleWays_ również kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
-   Oprócz wymienionych technik lokalizowania strony internetowej w witrynie internetowej mogą istnieć inne sposoby.


## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G63.md %}
- {% include techniki/G64.md %}
- {% include techniki/G125.md %}
- {% include techniki/G126.md %}
- {% include techniki/G161.md %}
- {% include techniki/G185.md %}
