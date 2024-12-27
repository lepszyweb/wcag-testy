---
title: 18. Znacząca treść i kolejność (dokument)
last_updated: 26 grudnia 2024

sidebar: testy_sidebar
permalink: 18-znaczaca-kolejnosc-doc
folder: testy/doc
---

## 18. Znacząca treść i kolejność

- {% include ks/1-3-1.md %}
- {% include ks/1-3-2.md %}

## Uzasadnienie metody testowej
Treści, które mają znaczenie, muszą być dostępne dla wszystkich użytkowników. Sekwencja treści (w kontekście) musi być logiczna i zachowywać znaczenie treści.

## Ograniczenia, założenia lub wyjątki
-   Znacząca treść zawiera informacje lub kontekst i obejmuje treść nagłówków, stopek, znaków wodnych, elementów strony wzorcowej, artefaktów i elementów przestawnych.
-   W tym teście uwzględniono style znakowe (śródliniowe)
-	Niewidoczna treść (tekst i tło mają ten sam kolor) jest używana do celów dostępności i nie jest uwzględniona w teście 18.A. Jest ona objęta w punkcie 18.B.
-	Programowo oznaczona treść jest wykorzystywana przez technologię wspomagającą. Treść dokumentu, która nie jest dostępna dla technologii wspomagających, może się różnić w zależności od typu dokumentu.

## 18.A Procedura testowa dla treści pozycjonowanych w CSS
Identyfikator testu podstawowego: _18.A-MeaningfulContent_

### Identyfikacja treści
<p id="d18aIC">Znacząca widoczne treść. Nie włączaj znaczących obrazów tła, które są objęte punktem odniesienia 6. Obrazy.</p>

### Instrukcja testowania

1.	Sprawdź, czy cała istotna treść dokumentu jest dostępna lub oznakowana programowo. [SC 1.3.1]

### Wynik testów
Jeśli powyższy test zakończy się niepowodzeniem, test podstawowy _18.A-MeaningfulContent_ również kończy się niepowodzeniem.

### 18.B Procedura testowa dla Znaczącej kolejności

Identyfikator testu podstawowego: _18.B-MeaningfulSequence_

### Identyfikacja treści

<p id="d18bIC">Wszystkie znaczące treści, w tym  treści niewidoczne.</p>


### Instrukcja testowania

<ol id="d18bTI">
    <li id="d18bTI-1">Sprawdź, czy kolejność czytania wszystkich istotnych treści (w kontekście) jest logiczna. [KS 1.3.2]</li>
</ol>

### Wynik testów
Jeśli powyższy test zakończy się niepowodzeniem, test podstawowy _18.B-MeaningfulSequence_ również kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
<p id="d18Advisory">Brak</p>

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G57.md %}
- {% include techniki/PDF3.md %}
- {% include techniki/PDF4.md %}
- {% include techniki/PDF17.md %}
- {% include techniki/F1.md %}
