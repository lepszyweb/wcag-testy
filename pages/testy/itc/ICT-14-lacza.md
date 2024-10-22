---
title: 14. Łącza
last_updated: 22 października 2024

sidebar: testy_sidebar
permalink: ICT-14-lacza
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/2-4-4.md %}
- {% include ks/4-1-2.md %}

## Opis metody testowej
Łącza, w tym elementy skryptowe, muszą mieć znaczący tekst (powiązany bezpośrednio lub znajdujący się w&nbsp;kontekście), który opisuje ich przeznaczenie lub funkcję. Aby powiązany tekst był dostępny dla technologii wspomagających, informacje muszą być 
<a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.okreslony_programowo | strip_html | replace: '*', ''}}">określone programowo</a> (możliwe do odczytania przez program komputerowy)

## Ograniczenia, założenia lub wyjątki
-   [Z Objaśnienia KS 2.4.4](https://wcag.irdpl.pl/understanding/cel-lacza-w-kontekscie.html): Mogą wystąpić sytuacje, w których cel łącza ma być nieznany lub ukryty. Na przykład gra może mieć łącza oznaczone tylko jako Drzwi #1, Drzwi #2 i Drzwi #3. Te teksty łączy byłyby wystarczające, ponieważ celem jest stworzenie napięcia dla wszystkich użytkowników.
-   Programowo określony kontekst łącza to dodatkowe informacje, które można programowo określić na podstawie relacji z łączem, połączyć z tekstem łącza i przedstawić użytkownikom w różnych modalnościach
    - **Przykład**: W języku HTML informacje, które można określić programowo na podstawie łącza w języku polskim, obejmują tekst znajdujący się w tym samym akapicie, w tym samym elemencie listy lub komórce tabeli, co łącze, lub w komórce nagłówka tabeli skojarzonej z komórką tabeli zawierającą łącze.
-   Połączenie dostępnej nazwy elementu i dostępnego opisu jest jego alternatywą tekstową.

## 14.A Procedura testowa dla celu łącza (w kontekście)
Identyfikator testu bazowego: _14.A-LinkPurpose_

### Identyfikacja treści
Wszystkie łącza, w tym te, które są elementami skryptowymi i mają przypisaną rolę łącza (role="link").

### Instrukcja testowania

1. Sprawdź, czy kombinacja [dostępnej nazwy i dostępnego opisu](https://www.w3.org/TR/html-aam-1.0/#accessible-name-and-description-computation) nie jest pusta. [KS 4.1.2]
2.  Sprawdź, czy cel każdego łącza można określić na podstawie dowolnej kombinacji tekstu łącza i programowo określonego połączonego kontekstu [KS 2.4.4]
    - tekstu, który znajduje się w tym samym akapicie, elemencie listy lub komórce tabeli co łącze,
	- tekstu, który znajduje się w komórce nagłówka tabeli skojarzonej z komórką tabeli zawierającą łącze

### Wynik testów


Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy  _14.A-LinkPurpose_ również kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
-   W przypadku, gdy łącze prowadzi do dokumentu lub aplikacji internetowej, nazwa dokumentu lub aplikacji internetowej wystarcza do opisania celu łącza (czyli odesłanie do dokumentu lub aplikacji internetowej).

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/ARIA7.md %}
- {% include techniki/ARIA8.md %}
- {% include techniki/G53.md %}
- {% include techniki/G91.md %}
- {% include techniki/H77.md %}
- {% include techniki/H79.md %}
- {% include techniki/F89.md %}

