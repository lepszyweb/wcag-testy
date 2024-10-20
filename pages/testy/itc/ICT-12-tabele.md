---
title: 12. Tabele


sidebar: testy_sidebar
permalink: ICT-12-tabele
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/1-3-1.md %}
- {% include ks/4-1-2.md %}

## Opis metody testowania
W przypadku użytkowników technologii wspomagających tabele danych muszą jawnie kojarzyć dane tabeli z&nbsp;nagłówkami wierszy i kolumn tabeli za pomocą znaczników programowych. Znaczniki tabel ułatwiają także nawigację użytkownikom technologii wspomagających, zapewniając programowe punkty orientacyjne za pomocą nagłówków kolumn i wierszy.

Jeśli elementy `<table>` są używane do celów układu, niedozwolone sa elementy struktury tabeli danych, takie jak `<th>`, `<caption>` lub `summary`.

## Ograniczenia, założenia lub wyjątki
-   **Tabele danych** to tabele, w których informacje w komórce wymagają nagłówka wiersza lub kolumny, aby odpowiednio opisać zawartość komórki. Jeśli tabela jest używana do rozmieszczania na stronie komponentów ze względu na estetykę wizualną, wówczas jest traktowana jako **tabelę układu**.
-   Może się wydawać, że niektóre treści wymagają wizualnej struktury tabeli danych, ale linearyzacja treści i&nbsp;wyświetlenie kodu ujawnia, że treść jest zrozumiała bez tabeli. 
-   Technikę **tabeli układu** można stosować w  projektach responsywnych. Te elementy wykorzystują CSS i/lub inne metody stylizacji do prezentacji treści w kolumnach lub wierszach. Przekazywane informacje nie opierają się na programowych relacjach między nagłówkami kolumn lub wierszy, niezbędnych do ich zrozumienia. Taka treść nie jest tabelą danych i nie powinna wykorzystywać elementu tabeli, atrybutu ARIA `role="table"` ani powiązanych atrybutów tabeli danych. Powinna być badana przy użyciu innych testów podstawowych, takich jak [13. Struktura treści](13_StrukturaTresci) lub ewentualnie [10. Formularze (powiązane instrukcje)](ICT_10_formularze).
-   Wiersze powiązanych danych muszą mieć nagłówek wiersza, aby użytkownicy technologii wspomagających mogli zrozumieć relacje między komórkami danych wiersza. Nie każda tabela wymaga nagłówka wiersza. Na przykład miesiąc kalendarzowy to tabela danych, zwykle z&nbsp;dniami tygodnia jako nagłówkami kolumn. Daty w wierszach nie są powiązane, więc zazwyczaj nie ma nagłówka wiersza. Gdyby jednak w każdym wierszu znajdowała się komórka wskazująca kolejny tydzień roku, komórka ta służyłaby jako nagłówek wiersza dla dat w&nbsp;tym wierszu.
-   Gdy w instrukcjach testu podstawowego wskazano atrybut ARIA `role`, odnosi się to do pierwszej prawidłowej wartości atrybutu `role` w znaczniku.

## 12.A Procedura testowania roli tabeli danych
Identyfikator testu podstawowego: _12.A-DataTableRole_

### Identyfikacja treści
Znajdź treść/dane, które są wizualnie przedstawione w tabeli, rozmieszczone w wierszach i kolumnach, w których po linearyzacji treść nie ma znaczącej (sensownej) kolejności.

**Uwaga**: Linearyzacja treści tabeli polega na prezentacji dwuwymiarowej treści tabeli w jednowymiarowej kolejności treści w źródle, zaczynając od pierwszej komórki w pierwszym wierszu i kończąc na ostatniej komórce w ostatnim wierszu, od lewej w prawo, od góry do dołu.


### Instrukcja testowania

1.  **Tabela**: Sprawdź, czy każda tabela danych ma rolę programową `table`, który określa ją jako tabelę danych, zdefiniowaną za pomocą jednej z wymienionych poniżej technik. Jeśli używana jest więcej niż jedna technika, wybierz pierwszą jawnie zdefiniowaną rolę i wykonaj pozostałe testy przy użyciu tego wyboru. [KS 4.1.2]
    -   HTML: znacznik `<table>`, który nie ma jawnie zdefiniowanego atrybutu roli i którego rola może być zmieniona z roli tabeli na inną, np. role="presentation" lub role="none".
    -   ARIA: atrybut `role="table"`
    -   ARIA: atrybut `role="grid"`
    -   ARIA: atrybut `role="treegrid"`
2.  **Komórka danych tabeli**: Sprawdź, czy każda komórka danych używa tylko jednej z&nbsp;następujących metod w&nbsp;celu zdefiniowania jej roli jako komórki danych w&nbsp;wierszu tabeli, w&nbsp;zależności od techniki określonej w&nbsp;pierwszym kroku:
    -   w przypadku znacznika HTML `<table>`: `<td>` dla komórki, która musi znajdować się wewnątrz wiersza `<tr>`.
    -   w przypadku atrybutu ARIA `role="table"`: element komórki danych z&nbsp;atrybutem `role="cell"` musi znajdować się wewnątrz elementu z&nbsp;atrybutem ARIA `role="row"`.
    -   w przypadku atrybutu ARIA `role="grid"` lub ARIA `role="treegrid"`: element komórki danych z&nbsp;atrybutem ARIA `role="gridcell"` musi znajdować się wewnątrz elementu z&nbsp;atrybutem ARIA `role="row"` (jeśli siatka ARIA nie korzysta z&nbsp;rdzennego elementu i&nbsp;struktury `<table>`).
3.  **Komórka nagłówka tabeli**: W przypadku zastosowanej techniki sprawdź, czy każda komórka nagłówka ma programowo przypisaną rolę nagłówka i&nbsp;znajduje się w&nbsp;nadrzędnym elemencie wiersza:
    -   dla elementu HTML `<table>`: nagłówek `<th>` musi znajdować się wewnątrz elementu nadrzędnego wiersza `<tr>`.
    -   dla tabeli utworzonej za pomocą atrybutów ARIA `role="table"`, `role="grid"`, `role="treegrid"`: każdy element z `role="columnheader"` lub `role="rowheader"` musi znajdować się w elemencie nadrzędnym z&nbsp;`role="row"`.

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _12.A-DataTableRole_ kończy się niepowodzeniem.


## 12.B Procedura testowania powiązań nagłówków tabeli danych
Identyfikator testu podstawowego: _12.B-DataTableHeaderAssociation_

### Identyfikacja treści
Znajdź w każdej tabeli danej określonej w teście 12.A wszystkie nagłówki kolumn i wierszy dla każdej komórki danych.

### Instrukcje testowe
1.	**Powiązanie komórki danych z nagłówkiem**: Użyj techniki programowania (HTML lub ARIA) określonej w&nbsp;teście 12.A. Sprawdź, czy każda komórka danych jest programowo skojarzona z jej nagłówkiem (nagłówkami) [KS 1.3.1]:
    -   **Tylko w przypadku prostych tabel HTML utworzonych znacznikiem `<table>`**: z nagłówkami kolumn tylko w pierwszym wierszu, które mają zastosowanie do wszystkich komórek danych w tej samej kolumnie, i nagłówkami wierszy tylko w pierwszej kolumnie, które mają zastosowanie do wszystkich komórek danych w tym samym wierszu; każda komórka nagłówka może być oznaczona `<th>` bez dodatkowych atrybutów.
    -   **w przypadku innych tabel HTML utworzonych znacznikiem `<table>`**: komórka nagłówka może być oznaczona atrybutem `<th scope="[col|row|colgroup|rowgroup]">`, jeśli wszystkie komórki danych, do których odnoszą się nagłówki, znajdują się odpowiednio w tej samej kolumnie, wierszu, grupie kolumn lub grupie wierszy. 
        -   W HTML4 obsługiwane jest `<td scope="[row|col]">`.
        -   W HTML5 `<td scope="[row|col]">` nie jest obsługiwane, więc wszystkie komórki nagłówka muszą być objęte znacznikiem `<th>`.
        -   Atrybut zakresu (`scope`) ma zastosowanie tylko do komórek, które znajdują się po komórkach nagłówka w kolejności odczytu.
    -   **w przypadku innych tabel HTML utworzonych znacznikiem `<table>`**: każda komórka danych `<td>` może być powiązana z komórką nagłówka za pomocą atrybutu `headers` z unikalną wartością identyfikatora `<td headers="[id]">`:
        -   Komórki danych z atrybutem `headers` muszą odwoływać się do identyfikatorów wszystkich odpowiednich komórek nagłówka na potrzeby powiązania programowego.
        -   Identyfikatory, do których odwołuje się atrybut headers dla komórek danych, muszą odnosić się do elementów **w tej samej tabeli** i **w spójnej kolejności**.
    -   **w przypadku innych tabel HTML, która mają OBA atrybuty - `scope` ORAZ `headers` w tej samej tabeli**: komórka danych z odwołaniem do nagłówków zastąpi wszystkie atrybuty `scope` dla tej konkretnej komórki danych. W związku z tym komórki danych z odwołaniem do nagłówków muszą wskazywać identyfikatory wszystkich powiązanych nagłówków.
    -   **W przypadku tabel utworzonych za pomocą atrybutu ARIA `role="table"`, `role="grid"` lub `role="gridtree"`**: każdy element nagłówka kolumny musi mieć `role="columnheader"`, a każdy element nagłówka wiersza musi mieć `role="rowheader"`.

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _12.B-DataTableHeaderAssociation_ również kończy się niepowodzeniem.

## 12.C Procedura testowania tabel układu
Identyfikator testu bazowego: _12.C-LayoutTable_

### Identyfikacja treści
Znajdź treść/dane przedstawione wizualnie w tabeli, która po linearyzacji przedstawia treść w sensownej kolejności.

**Uwaga**: Linearyzacja treści tabeli to prezentacja dwuwymiarowej treści tabeli w&nbsp;jednowymiarowej kolejności treści w&nbsp;źródle, zaczynając od pierwszej komórki w&nbsp;pierwszym wierszu, a&nbsp;kończąc na ostatniej komórce w ostatnim wierszu, od lewej do prawej, od góry do dołu.

### Instrukcje testowe
1.  Sprawdź, czy tabela służy wyłącznie do celów układu (rozmieszczenia elementów):
    -  **Nie** wyznacza tabeli układu za pomocą atrybutu `role="table"` i powiązanych atrybutów tabeli ARIA.
    - **Nie ma** elementów nagłówka tabeli HTML i/lub powiązanych atrybutów (np. `<th>`, `summary`, `<caption>`, `scope` i/lub `headers`), **chyba** że spełniony jest co najmniej jeden z poniższych warunków:
        - element HTML `<table>` ma atrybut `role="prezentation"`
        - element HTML `<table>` ma atrybut `role="none"`
    - **Nie ma** żadnych elementów z `role="columnheader"` lub `role="rowheader"`. Ponieważ te role są jawne, zastosowanie `role="presentation"` lub `role="none"` do elementu nadrzędnego nie zostanie odziedziczone (zgodnie z [Presentational Roles Conflict Resolution](https://www.w3.org/TR/wai-aria-1.3/#conflict_resolution_presentation_none), „Jeśli dozwolony element podrzędny ma jawną rolę nieprezentacyjną, programy użytkownika MUSZĄ zignorować odziedziczoną rolę prezentacyjną i uwidocznić element z jego jawną rolą”.) 

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _12.C-LayoutTable_ również kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

- Treści, które są prezentowana za pomocą CSS, aby wyglądały jak tabela, ale nie polegają na powiązaniu komórek z nagłówkami, można najłatwiej rozpoznać przez linearyzację. Innym pomocnym wskaźnikiem może być to, że tabela zawiera tylko nagłówki wierszy albo tylko nagłówki kolumn, ale nie oba.
- Testy podstawowe 12.A i 12.C należy przeprowadzić dla każdej tabeli danych.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/H43.md %}
- {% include techniki/H51.md %}
- {% include techniki/H63.md %}
- {% include techniki/F46.md %}
- {% include techniki/F49.md %}


