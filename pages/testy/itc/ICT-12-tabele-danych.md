---
title: 12. Tabele


sidebar: testy_sidebar
permalink: ICT-12-tabele-danych
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/1-3-1.md %}

## Uzasadnienie metody badania
W przypadku użytkowników technologii wspomagających (AT) tabele danych muszą jawnie kojarzyć dane tabeli z nagłówkami wierszy i kolumn tabeli za pomocą znacznika programowego. Znaczniki tabel ułatwiają także nawigację użytkownikom AT, zapewniając programowe punkty orientacyjne za pomocą nagłówków kolumn i wierszy.

Gdy elementy `<table>` są używane do celów układu, niedozwolone sa elementy struktury tabeli danych, takie jak `<th>`, `<caption>`, lub `summary=` (HTML4).


## Ograniczenia, założenia lub wyjątki
-   **Tabele danych** , w których informacje w komórce wymagają nagłówka wiersza lub kolumny, aby odpowiednio opisać zawartość komórki. Jeśli tabela jest używana do rozmieszczania na stronie komponentów ze względu na estetykę wizualną, wówczas jest uważana za **tabelę układu**.
-   Technikę tę można zastosować w  projektach responsywnych. Te elementy wykorzystują CSS i/lub inne metody stylizacji do prezentacji zawartości w kolumnach lub wierszach. Przekazywana informacja nie opiera się na zrozumiałych relacjach programowych z&nbsp;nagłówkami kolumn lub wierszy. Taka treść nie jest tabelą danych i nie powinna wykorzystywać elementu tabeli, atrybutu ARIA `role="table"` ani powiązanych atrybutów tabeli programowej. Powinna być baddana przy użyciu innych testów podstawowych, takich jak [13. Struktura treści](13_StrukturaTresci) lub ewentualnie [10. Formularze (powiązane instrukcje)](ICT_10_formularze).
-   Wiersze powiązanych danych muszą mieć nagłówek wiersza, aby użytkownicy technologii wspomagających mogli zrozumieć relacje między komórkami danych wiersza. Nie każda tabela wymaga nagłówka wiersza. Na przykład miesiąc kalendarzowy to tabela danych, zwykle z&nbsp;nagłówkami kolumn dniami tygodnia. Daty w rzędach nie są powiązane, więc zazwyczaj nie ma nagłówka wiersza. Gdyby jednak w każdym wierszu znajdowała się komórka wskazująca kolejny tydzień roku, komórka ta służyłaby jako nagłówek wiersza dla dat w&nbsp;tym wierszu.

## Procedura testu dla 1.3.1 Informacje i relacje

### Identyfikacja treści
Wszystkie treści/dane przedstawione wizualnie w tabeli z nagłówkami kolumn i/lub wierszy, w których po linearyzacji treść nie ma znaczącej (sensownej) kolejności.

**Uwaga**: Linearyzacja zawartości tabeli polega na prezentacji dwuwymiarowej treści tabeli w jednowymiarowej kolejności treści w źródle, zaczynając od pierwszej komórki w pierwszym wierszu i kończąc na ostatniej komórce w ostatnim wierszu, od lewej w prawo, od góry do dołu.


### Instrukcja testowania

#### Tabele danych
1.  **Tabela**: Sprawdź, czy każda tabela danych ma programowy kod, aby zidentyfikować ją jako tabelę przy użyciu jednej z następujących technik:
    -   HTML: znacznik `<table>`
    -   ARIA: atrybut `role="table"`
    -   ARIA: atrybut `role="grid"`

    **UWAGA**: zgodnie ze specyfikacją HTML5 elementu `<table>`  oraz powiązanych z nim elementów i&nbsp;atrybutów nie można używać w połączeniu z&nbsp;ARIA `role="table"` oraz powiązanymi rolami i&nbsp;atrybutami. Jeśli tabela łączy te techniki, test kończy się niepowodzeniem. Natomiast atrybut ARIA role="grid" **może  być** używany w&nbsp;elemencie `<table>`.

> Na przykład, autor, który zastosuje rolę siatki w jakimś elemencie tabeli HTML, nie musi stosować atrybutu ARIA `role="row"`, ani `role="gridcell"` do elementów potomnych HTML `<tr>` i `<td>`, ponieważ oprogramowanie użytkownika automatycznie dokona odpowiedniego przekładu. Gdy autor ponownie chce wykorzystać rdzenny element tabeli i potrzebuje elementu `gridcell` do rozciągnięcia wielu wierszy lub kolumn, POWINIEN zastosować odpowiednie atrybuty języka hosta (HTML) zamiast właściwości WAI-ARIA `aria-rowspan`  lub `aria-colspan` (z [Accessible Rich Internet Applications (WAI-ARIA) 1.1](https://www.w3.org/TR/wai-aria-1.1/grid-0)).

2.  Sprawdź, czy do elementu `<table>` NIE jest przypisany atrybut ARIA `role="presentation"`.
3.  **Komórki danych tabeli**: Sprawdź, czy każda komórka danych używa tylko jednej z&nbsp;następujących metod w celu zdefiniowania jej jako komórki danych w&nbsp;wierszu tabeli, w&nbsp;zależności od techniki określonej w&nbsp;pierwszym kroku:
    -   w przypadku znacznika HTML `<table>`: `<td>` dla komórki, która musi znajdować się wewnątrz wiersza `<tr>`.
    -   w przypadku atrybutu ARIA `role="table"`: atrybut ARIA `role="cell"` opisujący element, który musi znajdować się wewnątrz elementu z&nbsp;atrybutem ARIA `role="row"`.
    -   w przypadku atrybutu ARIA `role="grid"`: atrybut ARIA `role="gridcell"`, opisujący element, który musi znajdować się wewnątrz elementu z&nbsp;atrybutem ARIA `role="row"` (jeśli siatka ARIA nie korzysta z&nbsp;natywnego elementu i struktury `<table>`).
4.  **Komórki nagłówków i powiązane komórki danych**: Zidentyfikuj wszystkie nagłówki kolumn i&nbsp;wierszy dla każdej komórki danych. Sprawdź, czy wszystkie komórki danych są programowo powiązane z&nbsp;odpowiednimi nagłówkami, za pomocą jednej z&nbsp;poniższych technik::
    -   w przypadku prostych tabel HTML znacznik `<table>` ze wszystkimi nagłówkami w&nbsp;pierwszym wierszu LUB kolumnie, każda komórka nagłówkowa musi być oznaczona znacznikiem `<th>` bez dodatkowych atrybutów.
    -   w przypadku innych tabel HTML utworzonych znacznikiem `<table>`, komórki nagłówka można oznaczyć za pomocą `<th scope="xxx">`, jeśli wszystkie komórki danych następujące po nagłówku są powiązane wprost z nagłówkiem. HTML4 obsługuje `<td scope>` (nie jest więc konieczny znacznik `<th>`. W HTML5 `<td scope>` nie jest obsługiwane, więc wszystkie komórki nagłówka muszą mieć `<th>`. Dopuszczalne wartości dla atrybutu `scope` to `col` &vert; `row` &vert; `colgroup` &vert; `rowgroup`.  Zakres (*scope*) dotyczy tylko komórek, które występują po komórkach nagłówka(ów) w kolejności odczytu.
    -   w przypadku innych tabel HTML utworzonych znacznikiem `<table>`, komórki danych można powiązać z komórką nagłówka, włączając unikalną wartość identyfikatora `<td headers="xxx">`.
        -   Komórki danych muszą odwoływać się do identyfikatora (identyfikatorów) wszystkich odpowiednich komórek nagłówka za pomocą atrybutu `headers`, aby nagłówki wierszy i kolumn były poprawnie powiązane.
        -   Kolejność identyfikatorów nagłówków przywoływanych w atrybucie musi być konsekwentna i mieć znaczącą sekwencję.
    -   w przypadku innych tabel HTML utworzonych znacznikiem `<table>`,  które używają ZARÓWNO `<th scope=>`, JAK I odnoszą się do identyfikatorów nagłówków za pomocą atrybutów `<td headers=>` w tej samej tabeli, odniesienie do każdej komórka danych z headers= zastąpi wszystkie atrybuty `scope=` dla powiązanych nagłówków tabeli dla ta konkretnej komórki danych. W&nbsp;związku z&nbsp;tym komórki danych z odwołaniem `headers=` muszą wskazywać wszystkie odpowiednie nagłówki, niezależnie i&nbsp;od atrybutów `scope=` w&nbsp;powiązanych nagłówkach.
    -   w przypadku tabel utworzonych za pomocą atrybutu ARIA `role="table"`: każdy nagłówek kolumny musi mieć atrybut `role="columnheader"` ORAZ każdy nagłówek wiersza musi mieć `role="rowheader"`.
    -   w przypadku tabel utworzonych za pomocą atrybutu ARIA `role="grid"`: każdy nagłówek kolumny musi mieć atrybut `role="columnheader"` ORAZ każdy nagłówek wiersza musi mieć `role="rowheader"` (jeśli siatka ARIA nie korzysta z&nbsp;natywnego elementu i&nbsp;struktury `<table>`).

#### Tabele układu
1.  Sprawdź, czy tabele służą wyłącznie do celów układu (rozmieszczenia elementów):
    1.  Upewnij się, że tabela układu nie została zdefiniowana za pomoca atrybutu ARIA role="table" oraz atrybutów ARIA dotyczących tabeli
    2.  Upewnij się, że jeśli tabela ma atrybut `role="presentation"`, to nie zawiera komórek nagłówkowych i innych elementów struktury wskazujących relacje, ani powiązanych atrybutów (np. `<th>`, summary= (HTML4), `<caption>`, `scope=`, lub `headers=`).
    3.  Upewnij się, że w siatce ARIA (gdzie siatka danych jest identyfikowana za pomocą atrybutu `role="grid"`) NIE określono nagłówków kolumn za pomoca atrybutu ARIA `role="columnheader"`, ani nagłówków wierszy za pomocą atrybutu ARIA `role="rowheader"`.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.3.1 oraz wymaganie podstawowe nr 12 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego

Treści, które są prezentowana za pomocą CSS, aby wyglądały jak tabela, ale nie polegają na powiązaniu komórek z nagłówkami, można najłatwiej zidentyfikować przez linearyzację. Innym pomocnym wskaźnikiem może być to, że tabela zawiera tylko nagłówki wierszy albo tylko nagłówki kolumn.


## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/H43.md %}
- {% include techniki/H51.md %}
- {% include techniki/H63.md %}
- {% include techniki/F49.md %}
- {% include techniki/F46.md %}
