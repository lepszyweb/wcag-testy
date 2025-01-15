---
title: 12. Tabele (dokumenty)
last_updated: 16 stycznia 2025

sidebar: testy_sidebar
permalink: 12-tabele-doc
folder: testy/doc
---

# 12. Tabele

## Wymagania dostępności
- {% include ks/1-3-1.md %}
- {% include ks/4-1-2.md %}

## Uzasadnienie metody testowej
W przypadku użytkowników technologii wspomagających tabele danych muszą jawnie kojarzyć dane tabeli z&nbsp;nagłówkami wierszy i kolumn tabeli za pomocą znaczników programowych. Znaczniki tabel ułatwiają także nawigację użytkownikom technologii wspomagających, zapewniając programowe punkty orientacyjne za pomocą nagłówków kolumn i wierszy.

Jeśli elementy tabeli są używane do celów układu, niedozwolone są elementy struktury tabeli danych, takie jak nagłówki kolumn/wierszy, podpisy, podsumowania nie są dozwolone.

## Ograniczenia, założenia lub wyjątki
-   **Tabele danych** to tabele, w których informacje w komórce wymagają nagłówka wiersza lub kolumny, aby odpowiednio opisać zawartość komórki. Jeśli tabela jest używana do rozmieszczania na stronie komponentów ze względu na estetykę wizualną, wówczas jest traktowana jako **tabela układu**.
-   Może się wydawać, że niektóre treści wymagają wizualnej struktury tabeli danych, ale linearyzacja treści ujawnia, że treść jest zrozumiała bez tabeli. 
-   Technikę **tabeli układu** można stosować w  projektach responsywnych. Te elementy używają metod stylizacji do prezentacji treści w kolumnach lub wierszach. Przekazywane informacje nie opierają się na programowych relacjach między nagłówkami kolumn lub wierszy, niezbędnych do ich zrozumienia. Taka treść nie jest tabelą danych i nie powinna i nie powinna mieć programowych atrybutów tabeli danych. Powinna być badana przy użyciu innych testów podstawowych, takich jak [13. Struktura treści](13-struktura-tresci-doc.md) lub ewentualnie [10. Formularze (powiązane instrukcje)](10-formularze-doc.md).
-   Wiersze powiązanych danych muszą mieć nagłówek wiersza, aby użytkownicy technologii wspomagających mogli zrozumieć relacje między komórkami danych wiersza. Nie każda tabela wymaga nagłówka wiersza. Na przykład miesiąc kalendarzowy to tabela danych, zwykle z&nbsp;dniami tygodnia jako nagłówkami kolumn. Daty w wierszach nie są powiązane, więc zazwyczaj nie ma nagłówka wiersza. Gdyby jednak w każdym wierszu znajdowała się komórka wskazująca kolejny tydzień roku, komórka ta służyłaby jako nagłówek wiersza dla dat w&nbsp;tym wierszu.
-   Złożone tabele danych to tabele, które zawierają co najmniej jeden z tych elementów: wiele kolumn nagłówków wierszy, wiele wierszy nagłówków kolumn oraz podzielone lub scalone komórki. Te tabele muszą zawierać formatowanie, które ustanawia programowo określane relacje.

## 12.A Procedura testowania roli tabeli danych
Identyfikator testu podstawowego: _12.A-DataTableRole_

### Identyfikacja treści
Znajdź treść/dane, które są wizualnie przedstawione w tabeli, rozmieszczone w wierszach i kolumnach, w których po linearyzacji treść nie ma znaczącej (sensownej) kolejności.

**Uwaga**: Linearyzacja treści tabeli polega na prezentacji dwuwymiarowej treści tabeli w jednowymiarowej kolejności treści w źródle, zaczynając od pierwszej komórki w pierwszym wierszu i kończąc na ostatniej komórce w ostatnim wierszu, od lewej w prawo, od góry do dołu.


### Instrukcja testowania

<ol id="d12aTI">
    <li id="d12aTI-1">Sprawdź, czy każda tabela danych ma programowo przypisaną rolę tabeli. [SC 4.1.2]</li>
    <li id="d12aTI-2">Sprawdź, czy każda komórka danych ma programowo przypisaną rolę komórki danych. [SC 4.1.2]</li>
    <li id="d12aTI-3">Rozpoznaj wszystkie nagłówki kolumn i wierszy dla każdej komórki danych. Sprawdź, czy każda komórka nagłówka ma programowo przypisaną rolę nagłówka. [SC 4.1.2]</li>
</ol>
	
### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _12.A-DataTableRole_ kończy się niepowodzeniem.


## 12.B Procedura testowania powiązań nagłówków tabeli danych
Identyfikator testu podstawowego: _12.B-DataTableHeaderAssociation_

### Identyfikacja treści
Znajdź w każdej tabeli danej określonej w teście 12.A wszystkie nagłówki kolumn i wierszy dla każdej komórki danych.

### Instrukcje testowe

<ol id="d12bTI">
    <li id="d12bTI-1">Sprawdź, czy wszystkie komórki danych są programowo skojarzone z odpowiednimi nagłówkami. [SC 1.3.1]</li>
</ol>

### Wynik testów
Jeśli powyższy test zakończy się niepowodzeniem, test podstawowy _12.B-DataTableHeaderAssociation_ również kończy się niepowodzeniem.

### Identyfikacja treści
Znajdź treść/dane przedstawione wizualnie w tabeli, która po linearyzacji przedstawia treść w sensownej kolejności.

**Uwaga**: Linearyzacja treści tabeli to prezentacja dwuwymiarowej treści tabeli w&nbsp;jednowymiarowej kolejności treści w&nbsp;źródle, zaczynając od pierwszej komórki w&nbsp;pierwszym wierszu, a&nbsp;kończąc na ostatniej komórce w ostatnim wierszu, od lewej do prawej, od góry do dołu.

### Instrukcje testowe
<ol id="d12cTI">
    <li id="d12cTI-1">Sprawdź, czy tabela służy wyłącznie do celów układu (rozmieszczenia elementów), to znaczy NIE ma elementów nagłówków tabeli danych i powiązanych atrybutów, np. podpisu, określonego zakresu, podsumowania [KS 4.1.2]</li>
</ol>

### Wynik testów
Jeśli powyższy test zakończy się niepowodzeniem, test podstawowy test podstawowy _12.C-LayoutTable_ również kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

- Treści, które są prezentowana tak, aby wyglądały jak tabela, ale nie polegają na powiązaniu komórek z nagłówkami, można najłatwiej rozpoznać przez linearyzację. Innym pomocnym wskaźnikiem może być to, że tabela zawiera tylko nagłówki wierszy albo tylko nagłówki kolumn, ale nie oba.
- Testy podstawowe 12.A i 12.C należy przeprowadzić dla każdej tabeli danych.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/H43.md %}
- {% include techniki/H51.md %}
- {% include techniki/H63.md %}
- {% include techniki/PDF6.md %}
- {% include techniki/PDF20.md %}
- {% include techniki/F46.md %}
- {% include techniki/F49.md %}
