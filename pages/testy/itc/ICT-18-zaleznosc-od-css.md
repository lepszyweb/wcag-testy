---
title: 18. Zależność od CSS


sidebar: testy_sidebar
permalink: ICT-18-zaleznosc-od-css
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/1-1-1.md %}
- {% include ks/1-3-1.md %}
- {% include ks/1-3-2.md %}
- {% include ks/4-1-2.md %}

## Uzasadnienie metody badania
Znaczące informacje dostarczane wyłącznie przez CSS mogą nie być odwzorowane w Obiektowym MOdelu Dokumentów (DOM). Informacje równoważne muszą być dostępne bez CSS.

## Ograniczenia, założenia lub wyjątki
-   W tym teście uwzględniono tylko techniki CSS określone jako defekty w WCAG 2.0 poziom A i poziom AA. Mogą istnieć inne techniki CSS, które wpływają na zgodność.
-   W tym teście uwzględniono style śródliniowe.

## Procedura testu dla KS 1.1.1 Treść nietekstowa oraz 4.1.2 Nazwa, rola, wartość

### Identyfikacja treści
Znaczące obrazy tła renderowane przez CSS

### Instrukcja testowania
1.  Sprawdź, czy znaczący obraz CSS zawiera równoważny tekstowy opis alternatywny:
    1.  dodany za pomocą atrybutu ARIA `role="img"` i niepustej wartości atrybutu `aria-label` ORAZ
    2.  wartości atrybutu `aria-label` zapewnia te same informacje, co znaczący obraz tła

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.1.1, KS 4.1.2  oraz wymaganie podstawowe nr 18 kończy się niepowodzeniem.

## Procedura testu dla KS 1.3.1 Informacje i relacje

### Identyfikacja treści
Znacząca treść strony wstawiana przez CSS przy użyciu `::before` lub `::after`.

### Instrukcja testowania
1.  W przypadku treści znaczących dostarczanych za pośrednictwem CSS sprawdź, czy dostępne są równoważne informacje bez zawartości CSS.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.3.1  oraz wymaganie podstawowe nr 18 kończy się niepowodzeniem.

## Procedura testu dla KS 1.3.2 Zrozumiała kolejność

### Identyfikacja treści
Treść pozycjonowana za pomocą CSS::

### Instrukcja testowania
1.  Sprawdź, czy kolejność czytania treści (w kontekście) jest poprawna bez właściwości CSS `position`.
2.  Sprawdź, czy znaczenie treści (w kontekście) jest zachowane bez właściwości position CSS `position`.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.3.2 oraz wymaganie podstawowe nr 18 kończy się niepowodzeniem.

## Procedura testu dla KS 4.1.2 Nazwa, rola, wartość

Zobacz: [5. Treść zmienna](ICT_05_tresc-zmienna).

##  Wskazówki dotyczące usprawniania procesu testowego

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G57.md %}
- {% include techniki/F3.md %}
- {% include techniki/F87.md %}
- {% include techniki/F1.md %}
