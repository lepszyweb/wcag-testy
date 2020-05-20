---
title: 14. Łącza i przyciski


sidebar: testy_sidebar
permalink: ICT-14-lacza-przyciski
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/2-4-4.md %}
- {% include ks/4-1-2.md %}

## Uzasadnienie metody badania
Łącza i przyciski, w tym elementy skryptowe, muszą mieć znaczący tekst (powiązany bezpośrednio lub dostępny w&nbsp;kontekście) opisujący ich cel lub funkcję. Aby powiązany tekst był dostępny dla technologii wspomagających, informacje muszą być 
<a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.okreslony_programowo | strip_html | replace: '*', ''}}">określone programowo</a> (możliwe do odczytania przez program komputerowy)




## Ograniczenia, założenia lub wyjątki
-   [Z Objaśnienia KS 2.4.4](https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-refs.html): Mogą zaistnieć sytuacje, w których cel łącza ma być nieznany lub ukryty. Na przykład, gra może mieć łącza oznaczone tylko jako Drzwi 1, Drzwi nr 2 i Drzwi nr 3. Te teksty łączy byłyby wystarczające, ponieważ celem jest stworzenie napięcia dla wszystkich użytkowników.
-   Ten test obejmuje przyciski. W Technikach wystarczających dla KS 2.4.4 znajduje się technika [FLASH27: Zapewnienie etykiet przycisków opisujących przeznaczenie przycisku](https://www.w3.org/WAI/WCAG21/Techniques/flash/FLASH27).

## Procedura testu dla KS 2.4.4 Cel linku (w kontekście)

### Identyfikacja treści

Wszystkie łącza i przyciski, w tym te, które są elementami skryptowymi i którym przypisano rolę łącza (role="link") lub rolę przycisku (role="button").

### Instrukcja testowania

1.  Sprawdź, czy cel każdego łącza i przycisku można określić na podstawie dowolnej kombinacji tekstu łącza, [dostępnej nazwy, dostępnego opisu](https://www.w3.org/TR/html-aam-1.0/#accessible-name-and-description-computation) lub poprzedzającego bezpośrednio kontekstu strony (ten sam akapit, lista lub komórka tabeli, w której znajduje się łącza lub komórka nagłówka tabeli, z którą jest powiązana komórka zawierająca łącze).

### Wynik testów

Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test 2.4.4, KS 4.1.2 oraz Wymaganie podstawowe nr 14 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
-   W przypadku, gdy łącze / przycisk prowadzi do dokumentu lub aplikacji internetowej, nazwa dokumentu lub aplikacji internetowej wystarcza do opisania celu linku/przycisku (czyli odesłanie do dokumentu lub aplikacji internetowej).

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G91.md %}
- {% include techniki/G53.md %}
- {% include techniki/ARIA7.md %}
- {% include techniki/ARIA8.md %}
- {% include techniki/H77.md %}
- {% include techniki/H79.md %}
- {% include techniki/F89.md %}
