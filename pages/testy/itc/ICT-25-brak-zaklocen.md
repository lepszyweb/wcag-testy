---
title: 25. Brak zakłóceń


sidebar: testy_sidebar
permalink: ICT-25-brak-zaklocen
folder: testy/itc
---


## Wymagania dostępności

-   [WCAG Wymagania zgodności 5: Brak zakłóceń](https://www.w3.org/TR/WCAG20/#cc5) -- Następujące kryteria sukcesu dotyczą całej treści na stronie, włącznie z treścią, która w innych przypadkach nie jest podstawą spełnienia wymogów zgodności, gdyż niezastosowanie poniższych kryteriów mogłoby uniemożliwić jakiekolwiek skorzystanie ze strony:
    -   1.4.2 - Kontrola odtwarzania dźwięku,
    -   2.1.2 - Brak pułapki na klawiaturę,
    -   2.3.1 - Trzy błyski lub wartości poniżej progu
    -   2.2.2 - Wstrzymywanie (pauza), zatrzymywanie, ukrywanie.

## Uzasadnienie metody badania
O wynikach tego testu podstawowego decydują wyniki testów dla KS [1.4.2](ICT-21-limity-czasu.md), 2.1.2, 2.3.1 i 2.2.2

Wyniki testów dla SC 1.4.2 (21.4-AudioControl), 2.1.2 (1.2-NoKeyboadTrap), 2.3.1 (9.1-Flashes) i 2.2.2 (21.2-MovingInfo i 21.3-AutoUpdate) określają wynik tego test podstawowy.


## Ograniczenia, założenia lub wyjątki

Brak.

## Procedura testu dla Wymagania zgodności 5

### Identyfikacja treści
Podstawowe testy dla [1.4.2 oraz 2.2.2](21_LimityCzasu.md), [2.1.2](01_Klawiatura.md), [2.3.1](09_Miganie.md).

### Instrukcja testowania
1.  Sprawdź, czy wszystkie testy zakończyły się powodzeniem (zostły zaliczone).

### Wynik testów
Jeżeli którakolwiek z testów zakończył się niepowodzeniem, wówczas Wymaganie zgodności nr 5 oraz Wymaganaie podstawowe 25 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
-   Wszystkie testy wskazane w tym teście podstawowym muszą się zakończyć pomyślnie, aby cały test został uznany za zaliczony.


### Techniki WCAG 2.1
Nie dotyczy
