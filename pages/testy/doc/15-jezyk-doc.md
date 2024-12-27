---
title: 15. Język (dokument)
last_updated: 26 grudnia 2024

sidebar: testy_sidebar
permalink: 15-jezyk-doc
folder: testy/doc
---

## 15. Język

## Wymagania dostępności
- {% include ks/3-1-1.md %}
- {% include ks/3-1-2.md %}

## Uzasadnienie metody testowej
Domyślny naturalny (ludzki) język dla każdej strony musi być określony programowo. Fragmenty, które używają języka innego niż domyślny, muszą być określone programowo.

## Ograniczenia, założenia lub wyjątki
-   Podstawowy język dokumentów jest oparty na ustawieniach preferencji językowych aplikacji. Inne właściwości języka mogą być stosowane do całego dokumentu, określonej zawartości lub sekcji dokumentu. Dialekty określone w podznacznikach języka (dodatkowe 2 lub 3 znaki) nie są częścią tego testu.
-   Wyjątek:  Nazwy własne, terminy techniczne, słowa nieokreślonego języka oraz słowa lub frazy, które stały się częścią języka bezpośrednio otaczającego tekstu, nie są objęte językiem części.

## 15.A Procedura testu języka strony
Identyfikator testu podstawowego: _15.A-LanguageDocument_

### Identyfikacja treści
<p id="d15aIC">Strony z tekstem (w tym z tekstem alternatywnym).</p>

### Instrukcja testowania
1.  Określ domyślny język ludzki dokumentu, przeglądając jego treść. Domyślnym jest język, w którym prezentowana jest większość treści.
2.  Sprawdź, czy wartość właściwości Język odpowiada określonemu domyślnemu naturalnemu językowi dokumentu. [KS 3.1.1]

### Wynik testów
<p id="d15aTR">Jeżeli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _15.A-LanguagePage_ również kończy się niepowodzeniem.</p>


## 15.B Procedura testowa dla języka części
Identyfikator testu podstawowego: _15.B-LanguageParts_

### Identyfikacja treści

<p id="d15bIC">Treść tekstowa, której język różni się od domyślnego naturalnego języka dokumentu, w tym teksty alternatywne dla treści nietekstowych.</p>

### Instrukcja testowania
1.  Zidentyfikuj naturalny język treści tekstowej, inny niż domyślny naturalny język dokumentu.
2.  Sprawdź, czy dla każdego elementu treści w innym języku niż domyślny naturalny język dokumentu, określona została właściwość Język. [KS 3.1.2] 

**Uwaga**: Element bez ustawionego języka dziedziczy swoją właściwość Język z domyślnych ustawień języka dokumentu.

### Wynik testów
<p id="d15bTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy  _15.B-LanguageParts_ również kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
Brak.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/H57.md %}
- {% include techniki/H58.md %}
- {% include techniki/PDF16.md %}
- {% include techniki/PDF19.md %}
