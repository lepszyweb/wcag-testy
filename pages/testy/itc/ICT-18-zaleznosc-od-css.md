---
title: 18. Zależność od CSS


sidebar: testy_sidebar
permalink: ICT-18-zaleznosc-od-css
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/1-3-2.md %}

## Opis metody testowej
Znaczące informacje dostarczane wyłącznie przez CSS mogą nie być odwzorowane w Obiektowym Modelu Dokumentów (DOM). Informacje równoważne muszą być dostępne bez CSS.

## Ograniczenia, założenia lub wyjątki
-   W tym teście uwzględniono tylko techniki CSS określone jako defekty w WCAG 2.2 poziom A i poziom AA. Mogą istnieć inne techniki CSS, które wpływają na zgodność.
-   W tym teście uwzględniono style śródliniowe.

## 18.A dla procedury testowej dla znaczącego obrazu tła
Obraz tła CSS jest teraz objęty [procedurą testową 6.B dla obrazów z pustymi alternatywnymi tekstami](https://testy.lepszyweb.pl/ICT-06-obrazy#6a-procedura-testowa-dla-obraz%C3%B3w-z-niepust%C4%85-alternatyw%C4%85-tekstow%C4%85).

## 18.18.B Procedura testowa dla treści pozycjonowanych w CSS
Identyfikator testu podstawowego: _18.B-CSSPositionedContent_

### Identyfikacja treści
Znaczące treść pozycjonowana za pomocą CSSS

### Instrukcja testowania

1.	Sprawdź, czy kolejność czytania treści (w kontekście) jest poprawna bez właściwości CSS `position`. [KS 1.3.2]
2.	Sprawdź, czy znaczenie treści (w kontekście) jest zachowane bez właściwości CSS `position`. [KS 1.3.2]

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _18.B-CSSPositionedContent_również kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
-   Testy te nie powinny być wykonywane poprzez wyłączenie wszystkich CSS. Treść nie musi być wpostrzegalna i funkcjonalna przy wyłączonych wszystkich CSS.

## Techniki WCAG 2.1
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G57.md %}
- {% include techniki/F1.md %}
