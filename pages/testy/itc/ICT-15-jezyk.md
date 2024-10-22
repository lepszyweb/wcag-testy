---
title: 15. Język
last_updated: 22 października 2024

sidebar: testy_sidebar
permalink: ICT-15-jezyk
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/3-1-1.md %}
- {% include ks/3-1-2.md %}

## Uzasadnienie metody testowej
Domyślny naturalny (ludzki) język dla każdej strony musi być określony programowo. Fragmenty, które używają języka innego niż domyślny, muszą być określone programowo.

## Ograniczenia, założenia lub wyjątki
-   W przypadku treści internetowych atrybut języka `lang` może być atrybutem wielu znaczników HTML. Jego struktura to `<[znacznik HTML] lang="[podstawowy podznacznik języka\]">`. Podstawowy podznacznik języka jest pierwszym 2- lub 3-znakowym kodem w wartości atrybutu `lang`. Dialekty określone w podznacznikach języka (dodatkowe 2 lub 3 znaki) nie są częścią tego testu.
-   Wyjątek:  Nazwy własne, terminy techniczne, słowa nieokreślonego języka oraz słowa lub frazy, które stały się częścią języka bezpośrednio otaczającego tekstu, nie są objęte językiem części.

## 15.A Procedura testu języka strony
Identyfikator testu podstawowego: _15.A-LanguagePage_

### Identyfikacja treści
Strony z tekstem (w tym z tekstem alternatywnym).

### Instrukcja testowania
1.  Określ domyślny język użytkownika strony, przeglądając treść strony strony. Domyślnym jest język, w którym prezentowana jest większość treści.
2.  Sprawdź, czy w znaczniku `<html>` strony zdefiniowany jest atrybut `lang`. [KS 3.1.1]
3.  Sprawdź, czy wartość atrybutu `lang` odpowiada określonemu domyślnemu naturalnemu językowi strony. [KS 3.1.1]
    1.  Podznacznik języka podstawowego jest pierwszym 2- lub 3-znakowym kodem w wartości atrybutu *lang*. (Nie sprawdzaj dodatkowych specyfikacji języka, które mogą występować po podznaczniku języka podstawowego).
    2.  Podznacznik języka podstawowego musi być zgodny z urzędowym rejestrem kodów [IANA Language subtag registry](http://www.iana.org/assignments/language-subtag-registry).

### Wynik testów
Jeżeli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _15.A-LanguagePage_ również kończy się niepowodzeniem.

## 15.B Procedura testowa dla języka części
Identyfikator testu podstawowego: _15.B-LanguagePart_

### Identyfikacja treści
Treść tekstowa, której język różni się od domyślnego naturalnego języka strony, w tym teksty alternatywne dla treści nietekstowych.

### Instrukcja testowania
1.  Zidentyfikuj naturalny język treści tekstowej, inny niż domyślny naturalny język strony.
2.  Sprawdź, czy dla każdego elementu HTML zawierającego segment treści w innym języku niż domyślny naturalny język strony, określony został atrybut `lang`. [KS 3.1.2] Uwaga: Element bez ustawionego języka dziedziczy atrybut języka od elementów nadrzędnych.
3.  Sprawdź, czy dla segmentów treści w innym języku wartość atrybutu `lang` jest zdefiniowana poprawnie.
    -  Podznacznik języka podstawowego jest pierwszym 2- lub 3-znakowym kodem w wartości atrybutu `lang`. (Nie sprawdzaj dodatkowych specyfikacji języka, które mogą występować po podznaczniku języka podstawowego).
    -  Podznacznik języka podstawowego musi być zgodny z urzędowym rejestrem kodów [IANA Language subtag registry](http://www.iana.org/assignments/language-subtag-registry).

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy  _15.B-LanguagePart_ również kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
Brak.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/H57.md %}
- {% include techniki/H58.md %}
