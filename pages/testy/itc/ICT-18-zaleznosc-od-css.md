---
title: 18. Zależność od CSS


sidebar: testy_sidebar
permalink: ICT-18-zaleznosc-od-css
folder: testy/itc
---



## Wymagania dostępności
---------------------
-   [KS WCAG 1.1.1 Treść nietekstowa](https://wcag.lepszyweb.pl/#non-text-content) -- Wszelkie treści nietekstowe przedstawione użytkownikowi posiadają swoją tekstową alternatywę, która pełni tę samą funkcję, za wyjątkiem sytuacji opisanych poniżej.
    -   **Cele dekoracyjne, formatowanie, treść niewidoczna:** Jeśli treść nietekstowa pełni jedynie funkcję dekoracyjną, używana jest do formatowania wizualnego lub też nie jest przedstawiana użytkownikowi, powinna być wdrożona w sposób umożliwiający technologiom wspomagającym jej zignorowanie.
-   [KS WCAG 1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships) -- Informacje, struktura oraz relacje pomiędzy treściami przedstawiane w treści mogą być odczytane przez program komputerowy lub są dostępne w postaci tekstu.
-   [KS WCAG 1.3.2 Zrozumiała kolejność](https://wcag.lepszyweb.pl/#meaningful-sequence) -- Jeśli kolejność, w jakiej przedstawiona jest treść, ma znaczenie dla zrozumienia treści — kolejność taka musi być możliwa do odczytania przez program komputerowy.
-   [WCAG2 SC 4.1.2 Nazwa, rola, wartość](https://wcag.lepszyweb.pl/#name-role-value) -- Dla wszystkich komponentów interfejsu użytkownika (włączając w to, ale nie ograniczając jedynie do elementów formularzy, linków oraz komponentów wygenerowanych przez skrypty) nazwa oraz rola (przeznaczenie) mogą być odczytane przez program komputerowy, a stan, właściwości oraz wartości, które mogą być ustawione przez użytkownika, mogą również być ustawione przez program komputerowy; zawiadomienie o zmianach w tych elementach dostępne jest dla programów użytkownika, w tym technologii wspomagających.

## Uzasadnienie metody badania
------------------------------
Znaczące informacje dostarczane wyłącznie przez CSS mogą nie być odwzorowane w Obiektowym MOdelu Dokumentów (DOM). Informacje równoważne muszą być dostępne bez CSS.


## Ograniczenia, założenia lub wyjątki
---------------------------------------
-   W tym teście uwzględniono tylko techniki CSS określone jako defekty w WCAG 2.0 poziom A i poziom AA. Mogą istnieć inne techniki CSS, które wpływają na zgodność.
-   W tym teście uwzględniono style śródliniowe.

## Procedura testu dla KS 1.1.1 Treść nietekstowa oraz 4.1.2 Nazwa, rola, wartość
------------------------------------------------------------------------

### Identyfikacja treści
Znaczące obrazy tła renderowane przez CSS

### Instrukcja testowania
1.  Sprawdź, czy znaczący obraz CSS zawiera równoważny tekstowy opis alternatywny:
    1.  dodany za pomocą atrybutu ARIA `role="img"` i niepustej wartości atrybutu `aria-label` ORAZ
    2.  wartości atrybutu `aria-label` zapewnia te same informacje, co znaczący obraz tła

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.1.1, KS 4.1.2  oraz wymaganie podstawowe nr 18 kończy się niepowodzeniem.

## Procedura testu dla KS 1.3.1 Informacje i relacje
---------------------------------------------------

### Identyfikacja treści
Znacząca treść strony wstawiana przez CSS przy użyciu `::before` lub `::after`.

### Instrukcja testowania
1.  W przypadku treści znaczących dostarczanych za pośrednictwem CSS sprawdź, czy dostępne są równoważne informacje bez zawartości CSS.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.3.1  oraz wymaganie podstawowe nr 18 kończy się niepowodzeniem.

## Procedura testu dla KS 1.3.2 Zrozumiała kolejność
---------------------------------------------------

### Identyfikacja treści
Treść pozycjonowana za pomocą CSS::

### Instrukcja testowania
1.  Sprawdź, czy kolejność czytania treści (w kontekście) jest poprawna bez właściwości CSS `position`.
2.  Sprawdź, czy znaczenie treści (w kontekście) jest zachowane bez właściwości position CSS `position`.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.3.2 oraz wymaganie podstawowe nr 18 kończy się niepowodzeniem.

## Procedura testu dla KS 4.1.2 Nazwa, rola, wartość
-----------------------------------------------
Zobacz: [5. Treść zmienna.md](testy/ICT_05_tresc-zmienna.md).

##  Wskazówki dotyczące usprawniania procesu testowego
---------------------------------------------
## Techniki WCAG 2.1
---------------------
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [G57: Porządkowanie zawartości w znaczącej kolejności](https://www.w3.org/TR/WCAG20-TECHS/G57.html)
-   [F3: Niespełnienie kryterium sukcesu 1.1.1 z powodu użycia CSS do osadzania obrazów, które przekazują ważne informacje](https://www.w3.org/TR/WCAG20-TECHS/F3.html)
-   [F87: Niespełnienie kryterium sukcesu 1.3.1 z powodu wstawiania nieprzywijających się treści za pomocą pseudoelementów :before oraz :after i własności 'content' w CSS](https://www.w3.org/TR/WCAG20-TECHS/F87.html)
-   [F1: Niespełnienie kryterium sukcesu 1.3.2 z powodu zmiany znaczenia treści poprzez umieszczenie informacji w CSS](https://www.w3.org/TR/WCAG20-TECHS/F1.html)
