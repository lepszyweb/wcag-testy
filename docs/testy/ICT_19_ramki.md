# 19. Ramki i ramki wbudowane

## Wymagania dostępności
--------------------------
-   [KS WCAG 4.1.2 Nazwa, rola, wartość](https://wcag.lepszyweb.pl/#name-role-value) -- Dla wszystkich komponentów interfejsu użytkownika (włączając w to, ale nie ograniczając jedynie do elementów formularzy, linków oraz komponentów wygenerowanych przez skrypty) nazwa oraz rola (przeznaczenie) mogą być odczytane przez program komputerowy, a stan, właściwości oraz wartości, które mogą być ustawione przez użytkownika, mogą również być ustawione przez program komputerowy; zawiadomienie o zmianach w tych elementach dostępne jest dla programów użytkownika, w tym technologii wspomagających.

## Uzasadnienie metody badania
HTML  obejmuje elementy zwane ramkami i ramkami liniowymi (iframes). Ramki są używane do osadzania na stronie treści ze źródeł zewnętrznych. Na przykład często spotyka się osadzanie ramki z treścią audio lub wideo z innej strony.

O ile użytkownicy widzący mogą rozpoznać strukturę przedstawioną za pomocą ramek i ramek wbudowanych, to użytkownicy czytników ekranu muszą polegać na elementach programowych, które powinny przekazać informację o treści ramek. Celem tych testów jest zbadanie, czy zawartość elementów `<frame>` lub `<iframe>` została w kodzie opisana odpowiednio dla technologii wspomagajacej.   

## Ograniczenia, założenia lub wyjątki
---------------------------------------
- W HTML5 element  `<frame>` jest oznaczony jako przestarzały. Element `<iframe>` jest częścią specyfikacji HTML5. 
Mimo że element `<frame>` jest przestarzały, testerzy mogą spotkać się ze stronami internetowymi lub aplikacjami mobilnymi z przestarzałym kodem, który który choć jest nieaktualny, może i powinien być nadal dostępny.
 
## Procedura testu dla KS 4.1.2 Nazwa, rola, wartość
---------------------------------------------
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

---------------------------------------------
## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [H64: Używanie atrybutu title do tytułowania elementów frame i iframe](http://www.w3.org/TR/WCAG20-TECHS/H64.html)
    
----------------------------------------
[Początek/Wprowadzenie](testy/ICT_00_wprowadzenie.md) | [Poprzedni &gt; Zależność od CSS](testy/ICT_18_zaleznosc-od-css.md) | [Następny &gt; Zgodność z wersją alternatywną](testy/ICT_20_wersje-alternatywne.md)