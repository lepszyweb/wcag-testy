---
title: 15. Język


sidebar: testy-itc_sidebar
permalink: ICT_15_jezyk
folder: testy-itc
---

## Wymagania dostępności
---------------------
-   [KS WCAG: 3.1.1 Język strony](http://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-doc-lang-id.html) -- Domyślny język naturalny każdej strony internetowej może zostać odczytany przez program komputerowy.
-   [KS WCAG: 3.1.2 Język części](http://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-other-lang-id.html) -- Język naturalny każdej części lub frazy zawartej w treści może zostać odczytany przez program komputerowy, za wyjątkiem nazw własnych, wyrażeń technicznych, słów w nieokreślonym języku oraz słów i fraz, które stanowią część żargonu w bezpośrednio otaczającym je tekście.

## Uzasadnienie metody badania
------------------------------
Domyślny język naturalny (ludzki) dla każdej strony musi być zidentyfikowany programowo. Fragmenty, które używają języka innego niż domyślny, muszą zostać określone programowo.

## Ograniczenia, założenia lub wyjątki
--------------------------------------
-   W przypadku treści internetowych atrybut języka `lang` może być atrybutem wielu znaczników HTML. Jego struktura to `<[znacznik HTML] lang="[podstawowy podznacznik języka\]">`. Podstawowy podznacznik języka jest pierwszym 2 lub 3 znakowym kodem w wartości atrybutu `lang`. Dialekty określone w podznacznikach języka (dodatkowe 2 lub 3 znaki) nie są częścią tego testu.
-   Wyjątek:  Nazwy własne, terminy techniczne, słowa nieokreślonego języka oraz słowa lub frazy, które stały się częścią języka bezpośrednio otaczającego tekstu, nie są objęte językiem części.

## Procedura testu dla KS 3.1.1 Język strony
--------------------------------------------
### Identyfikacja treści
Strony z tekstem (w tym z tekstem alternatywnym).

### Instrukcja testowania
1.  Przeglądając treść strony, zidentyfikuj domyślny naturalny język strony. Domyślnym jest język, w którym prezentowana jest większość treści.
2.  Sprawdź, czy w znaczniku `<html>` strony zdefiniowany jest atrybut `lang`.
3.  Sprawdź, czy wartość atrybutu `lang` odpowiada określonemu domyślnemu naturalnemu językowi strony.
    1.  Podznacznik języka podstawowego jest pierwszym 2 lub 3 znakowym kodem w wartości atrybutu *lang*. (Nie sprawdzajj dodatkowych specyfikacji języka, które mogą występować po podznaczniku języka podstawowego).
    2.  Podznacznik języka podstawowego musi być zgodny z urzędowym rejestrem kodów [IANA Language subtag registry](http://www.iana.org/assignments/language-subtag-registry).

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.1.1  oraz wymaganie podstawowe nr 15 kończy się niepowodzeniem.

## Procedura testu dla KS 3.1.2 Język części
--------------------------------------------
### Identyfikacja treści
Zawartość tekstowa, która różni się od domyślnego naturalnego języka strony, w tym teksty alternatywne dla zawartości nietekstowej.

### Instrukcja testowania
1.  Zidentyfikuj naturalny język treści tekstowej, inny niż domyślny naturalny język strony.
2.  Sprawdź, czy dla każdego elementu HTML zawierającego segment treści w innym języku niż domyślny naturalny język strony, określony został atrybut `lang`. Uwaga: Element bez ustawionego języka dziedziczy atrybut języka od elementów nadrzędnych.
3.  Sprawdź, czy dla segmentów treści w innym języku wartość atrybutu `lang` jest zdefiniowana poprawnie.
    1.  Podznacznik języka podstawowego jest pierwszym 2 lub 3 znakowym kodem w wartości atrybutu `lang`. (Nie sprawdzajj dodatkowych specyfikacji języka, które mogą występować po podznaczniku języka podstawowego).
    2.  Podznacznik języka podstawowego musi być zgodny z urzędowym rejestrem kodów [IANA Language subtag registry](http://www.iana.org/assignments/language-subtag-registry).
### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.1.2  oraz wymaganie podstawowe nr 15 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
----------------------------------------------------------
Brak.

### Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [H57: Używanie atrybutu lang dla elementu html](https://www.w3.org/TR/WCAG20-TECHS/H57.html)
-   [H58: Używanie atrybutu lang do wskazywania zmian w języku naturalnym](https://www.w3.org/TR/WCAG20-TECHS/H58.html)


