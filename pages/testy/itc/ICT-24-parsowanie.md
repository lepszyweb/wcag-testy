---
title: 24. Parsowanie


sidebar: testy_sidebar
permalink: ICT-24-parsowanie
folder: testy/itc
---

## Wymogi dostępności
- {% include ks/4-1-1.md %}

## Opis metody testowej
- WCAG 2.2 wycofały KS 4.1.1 Parsowanie, ponieważ nie jest ono już potrzebne, gdyż błędy dostępności w technologiach wspomagających bezpośrednio parsujących HTML już nie istnieją lub są uwzględnione w innych kryteriach.
- Sekcja 508 nie jest bezpośrednio objęta WCAG 2.2, ponieważ odnosi się do WCAG 2.0 Poziom A i AA, Zalecenie W3C, 11 grudnia 2008. KS 4.1.1 Parsowanie nie jest przestarzałe w WCAG 2.0, a kryterium jest wymogiem sekcji 508. Jednak ten test podstawowy będzie zawierał Erratę WCAG 2.0, która stwierdza „To kryterium powinno być uważane za zawsze spełnione dla każdej treści wykorzystującej HTML lub XML”.

<!-- Ten test podstawowy wymaga, aby treść nie zawierała błędów w składni elementów i atrybutów oraz zapewniała prawidłowo zagnieżdżone znaczniki początku/końca, aby uniknąć błędów, które uniemożliwiają programom użytkowników niezawodne przetwarzanie zawartości. Jeśli treści nie można przetworzyć w strukturę danych, wówczas różne programy użytkownika, w tym technologie wspomagające, mogą ją prezentować  odmiennie lub w ogóle nie potrafią jej przetworzyć.-->

## Ograniczenia, założenia lub wyjątki

Z [Erraty do WCAG 2.0](https://www.w3.org/WAI/WCAG20/errata/): Kryterium sukcesu 4.1.1 zostało pierwotnie przyjęte w celu rozwiązania problemów związanych z bezpośrednim analizowaniem HTML przez technologie wspomagające. Od czasu napisania tego kryterium Standard HTML przyjął konkretne wymagania regulujące sposób, w jaki programy użytkownika muszą obsługiwać niekompletne znaczniki, nieprawidłowe zagnieżdżanie elementów, zduplikowane atrybuty i nieunikalne identyfikatory. 

Mimo że standard HTML traktuje niektóre z tych przypadków jako niezgodne dla autorów, uważa się, że „zezwala na te funkcje” do celów tego kryterium sukcesu, ponieważ specyfikacja wymaga, aby programy użytkownika obsługiwały te przypadki w sposób spójny. W praktyce kryterium to samo w sobie nie zapewnia już żadnych korzyści osobom  z niepełnosprawnościami.

Problemy, takie jak brakujące role z powodu nieprawidłowo zagnieżdżonych elementów lub nieprawidłowe stany lub nazwy z powodu zduplikowanego identyfikatora, są objęte innymi kryteriami sukcesu i powinny być zgłaszane w ramach tych kryteriów, a nie jako problemy z 4.1.1.

## Procedura testu dla KS 4.1.1 Parsowanie
Identyfikator testu podstawowego: _24.A-Parsing_
### Identyfikacja treści
Wszystkie strony internetowe

### Instrukcje testowe
1.	Nie są wymagane żadne testy.

### Wynik testów
Test podstawowy _24.A-Parsowanie_ zawsze kończy się pomyślnie.

## Porada: Wskazówki dotyczące usprawniania procesu testów

Brak

## Techniki WCAG 2.2
Chociaż KS 4.1.1 zostało uznane przez WCAG 2.2 za przestarzałe, w celach informacyjnych wymieniono następujące wystarczające techniki:

- {% include techniki/G134.md %}
- {% include techniki/G192.md %}
- {% include techniki/H88.md %}
- {% include techniki/H74.md %} ORAZ {% include techniki/H93.md %} I {% include techniki/H94.md %}
