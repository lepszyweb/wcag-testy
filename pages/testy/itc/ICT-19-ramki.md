---
title: 19. Ramki i ramki wbudowane


sidebar: testy_sidebar
permalink: ICT-19-ramki
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/4-1-2.md %}

## Opis metody testowej
HTML  obejmuje elementy zwane ramkami i ramkami liniowymi (`iframe`, inaczej liniowa, łączona, pływająca, lokalna, wbudowana). Ramki są używane do osadzania na stronie treści ze źródeł zewnętrznych. Na przykład często spotyka się osadzanie ramki z treścią audio lub wideo z innej strony.

O ile użytkownicy widzący mogą rozpoznać strukturę prezentowaną za przez ramki i i elementy `iframe`, to użytkownicy czytników ekranu muszą polegać na elementach programowych, które powinny przekazać informację o treści ramek. Ta procedura testowa służy ocenie, czy treść elementów `<frame>` lub `<iframe>` została w kodzie przedstawiona odpowiednio dla technologii wspomagającej.   

## Ograniczenia, założenia lub wyjątki
-   W HTML5 element  `<frame>` jest oznaczony jako przestarzały. Element `<iframe>` jest częścią specyfikacji HTML5. Mimo że element `<frame>` jest przestarzały, testerzy mogą nadal spotykać strony internetowe lub aplikacje mobilne z przestarzałym kodem, który choć jest nieaktualny, może i powinien być nadal dostępny.
-   Połączenie dostępnej nazwy i dostępnego opisu elementu `<iframe>` jest jego alternatywą tekstową.
-   Czwarta zasada użycia ARIA mówi: "nie używaj `role="presentation"` lub `aria-hidden="true"` na elemencie, na który można przenieść fokus. Użycie któregokolwiek z nich na elemencie, na którym można się skupić, spowoduje, że niektórzy użytkownicy skupią się na „niczym”.
-   Piąta zasada użycia ARIA mówi: „wszystkie elementy interaktywne muszą mieć dostępną nazwę”.

## 19.A Procedura testowa dla ramek
Identyfikator testu podstawowego: _19.A-FrameTitle_

### Identyfikacja treści
Wszystkie ramki (`frame`).

### Instrukcja testowania
1.  Sprawdź, czy każdy element `<frame` ma atrybut `title`, który nie jest pusty. [KS 4.1.2]
2.	Sprawdź, czy atrybut `title` wystarczająco dokładnie opisuje treść ramki. [SC 4.1.2]

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _19.A-FrameTitle_ również kończy się niepowodzeniem.

## 19.B Procedura testowa dla iFrame
Identyfikator testu podstawowego: _19.B-iFrameName_

### Identyfikacja treści
Wszystkie ramki iFrame w kolejności fokusu klawiatury

### Instrukcja testowania
1.	Sprawdź, czy kombinacja [dostępnej nazwy i opisu](https://www.w3.org/TR/html-aam-1.0/#iframe-element) każdego elementu iframe nie jest pusta. [KS 4.1.2]
2.	Sprawdź, czy niepusta kombinacja dostępnej nazwy i dostępnego opisu każdego elementu iframe przedstawia wystraczająco dokładnie jego treść. [KS 4.1.2]
3.	Sprawdź, czy rola ARIA nie jest "prezentation". [KS 4.1.2].1.2]
4.	Sprawdź, czy rola ARIA nie jest "none". [KS 4.1.2]
5.	Sprawdź, czy stan aria-hidden nie jest "true". [KS 4.1.2]

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _19.B-iFrameName_ również kończy się niepowodzeniem.


##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
brak

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:
- {% include techniki/H64.md %}
