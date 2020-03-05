---
title: 19. Ramki i ramki wbudowane


sidebar: testy_sidebar
permalink: ICT-19-ramki
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/4-1-2.md %}

## Uzasadnienie metody badania
HTML  obejmuje elementy zwane ramkami i ramkami liniowymi (iframes). Ramki są używane do osadzania na stronie treści ze źródeł zewnętrznych. Na przykład często spotyka się osadzanie ramki z treścią audio lub wideo z innej strony.

O ile użytkownicy widzący mogą rozpoznać strukturę przedstawioną za pomocą ramek i ramek wbudowanych, to użytkownicy czytników ekranu muszą polegać na elementach programowych, które powinny przekazać informację o treści ramek. Celem tych testów jest zbadanie, czy zawartość elementów `<frame>` lub `<iframe>` została w kodzie opisana odpowiednio dla technologii wspomagajacej.   

## Ograniczenia, założenia lub wyjątki
- W HTML5 element  `<frame>` jest oznaczony jako przestarzały. Element `<iframe>` jest częścią specyfikacji HTML5.
Mimo że element `<frame>` jest przestarzały, testerzy mogą spotkać się ze stronami internetowymi lub aplikacjami mobilnymi z przestarzałym kodem, który który choć jest nieaktualny, może i powinien być nadal dostępny.

## Procedura testu dla KS 4.1.2 Nazwa, rola, wartość

### Ramki - `Frame`

#### Identyfikacja treści
Wszystkie ramki (`frame`).

#### Instrukcja testowania
1.  Sprawdź, czy każde element `<frame` ma atrybut `title` odpowiednio opisujący zawartość ramki


### Wynik testów
Jeżeli powyższa próba zakończy się niepowodzeniem, wówczas test KS 4.1.2 oraz wymaganie podstawowe nr 19 kończy się niepowodzeniem.

### Ramki wbudowane - `iFrame`

#### Identyfikacja treści
Wszystkie ramki wbudowanne (`iFrames`).

#### Instrukcja testowania
1.  Sprawdź, czy kombinacja [dostępnej nazwy i opisu](https://www.w3.org/TR/html-aam-1.0/#iframe-element) odpowiednio opisuje zawartość ramki wbudowanej.

### Wynik testów
Jeżeli powyższa próba zakończy się niepowodzeniem, wówczas test KS 4.1.2 oraz wymaganie podstawowe nr 19 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/H64.md %}
