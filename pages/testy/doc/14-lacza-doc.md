---
title: 14. Łącza (dokument)
last_updated: 16 stycznia 2025

sidebar: testy_sidebar
permalink: 14-lacza-doc
folder: testy/doc
---

## Wymagania dostępności
- {% include ks/2-4-4.md %}
- {% include ks/4-1-2.md %}

## Uzasadnienie metody testowej
Łącza i przyciski, w tym elementy skryptowe, muszą mieć znaczący tekst (powiązany bezpośrednio lub znajdujący się w&nbsp;kontekście), który opisuje ich przeznaczenie lub funkcję. Aby powiązany tekst był dostępny dla technologii wspomagających, informacje muszą być możliwe do odczytania przez program komputerowy (możliwe do określenia programowo).

## Ograniczenia, założenia lub wyjątki
-   [Z Objaśnienia KS 2.4.4](https://wcag.irdpl.pl/understanding/cel-lacza-w-kontekscie.html): Mogą wystąpić sytuacje, w których cel łącza ma być nieznany lub ukryty. Na przykład gra może mieć łącza oznaczone tylko jako Drzwi #1, Drzwi #2 i Drzwi #3. Te teksty łączy byłyby wystarczające, ponieważ celem jest stworzenie napięcia dla wszystkich użytkowników.
-   Programowo określony kontekst łącza to dodatkowe informacje, które można programowo określić na podstawie relacji z łączem, połączyć z tekstem łącza i przedstawić użytkownikom w różnych modalnościach
    - **Przykład**: W języku HTML informacje, które można określić programowo na podstawie łącza w języku polskim, obejmują tekst znajdujący się w tym samym akapicie, w tym samym elemencie listy lub komórce tabeli, co łącze, lub w komórce nagłówka tabeli skojarzonej z komórką tabeli zawierającą łącze.
-   Kombinacja dostępnej nazwy elementu i dostępnego opisu jest jego alternatywą tekstową.

## 14.A Procedura testowa dla celu łącza (w kontekście)
Identyfikator testu bazowego: _14.A-LinkPurpose_

### Identyfikacja treści
<p id="d14aIC">Wszystkie łącza, w tym te, które są elementami skryptowymi i działają jak łącza.</p>

### Instrukcja testowania

1. Sprawdź, czy kombinacja [dostępnej nazwy i dostępnego opisu](https://www.w3.org/TR/html-aam-1.0/#accessible-name-and-description-computation) nie jest pusta. [KS 4.1.2]
2.  Sprawdź, czy cel każdego łącza można określić na podstawie dowolnej kombinacji tekstu łącza i programowo określonego połączonego kontekstu [KS 2.4.4]
    - tekstu łącza
	- tekstu, który znajduje się w tym samym akapicie, elemencie listy lub komórce tabeli co łącze,
	- tekstu, który znajduje się w komórce nagłówka tabeli skojarzonej z komórką tabeli zawierającą łącze

### Wynik testów
<p id="d14aTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy  <em>14.A-LinkPurpose</em> również kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
-   W przypadku, gdy łącze prowadzi do dokumentu lub aplikacji internetowej, nazwa dokumentu lub aplikacji internetowej wystarcza do opisania celu łącza (czyli odesłanie do dokumentu lub aplikacji internetowej).

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G53.md %}
- {% include techniki/G91.md %}
- {% include techniki/H77.md %}
- {% include techniki/H79.md %}
- {% include techniki/PDF11.md %}
- {% include techniki/PDF13.md %}
- {% include techniki/F89.md %}
