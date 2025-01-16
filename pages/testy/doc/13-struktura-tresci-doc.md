---
title: 13. Struktura treści (dokumenty)
last_updated: 16 stycznia 2025

sidebar: testy_sidebar
permalink: 13-struktura-tresci-doc
folder: testy/doc
---


# 13. Struktura treści

## Wymagania dostępności
- {% include ks/2-4-6.md %}
- {% include ks/1-3-1.md %}

## Uzasadnienie metody testowej

-   Widoczne nagłówki muszą być [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable), reprezentować strukturę treści i opisywać treść, która następuje po nagłówkach.
-   Widoczne listy wizualne  muszą być [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable), zgodnie z ich typami (uporządkowane, nieuporządkowane, listy definicji).

## Ograniczenia, założenia lub wyjątki

-   Dokument, w którym znajduje się tylko jeden nagłówek, nie ma struktury na poziomie nagłówków i nie może być testowany pod kątem struktury nagłówków.
-   Dokument może mieć więcej niż jeden nagłówek poziomu 1 lub nie mieć nagłówka poziomu 1.
-   Nagłówek poziomu 1 w dokumencie nie musi być zgodny z tytułem dokumentu.
-   Kolejność poziomów nagłówków nie zawsze może być zgodna z porządkiem liczenia, a mimo to będzie prawidłowa, ponieważ odnosi się do struktury wizualnej/ważkości podanej za pomocą widocznych nagłówków na stronie. Na przykład nagłówek poziomu 2 może być zastosowany dla oznaczenia struktury nawigacyjnej, która poprzedza tytuł nagłówka poziomu 1 w dokumencie. Podobnie, po nagłówku poziomu 1 może następować nagłówek poziomu 3 bez nagłówka poziomu 2 między nimi.
-   Nie wszystkie listy wymagają oznaczania. Na przykład zdania zawierające wykazy rozdzielone przecinkami mogą nie wymagać znaczników list.
-   Test list widocznych wizualnie nie powinien obejmować menu nawigacyjnych. Chociaż listy programowe są często używane do tworzenia menu nawigacyjnych, menu mogą być również tworzone przy użyciu innych technik.

## 13.A Procedura testowa dla nagłówków opisowych
Identyfikator testu podstawowego: _13.A-HeadingDescriptive_

### Identyfikacja treści
<p id="d13aIC">Wizualnie widoczne nagłówki, które oznaczają sekcje treści. Nagłówki są często pisane większą, pogrubioną czcionką, są oddzielone od akapitów dodatkowymi odstępami (choć nie zawsze). Zwróć uwagę na hierarchię i strukturę każdego nagłówka w odniesieniu do innych nagłówków na stronie lub ekranie.</p>

### Instrukcja testowania
1.  Sprawdź, czy każdy nagłówek opisuje temat lub cel następującej po nim treści. [KS 2.4.6]

### Wynik testów
<p id="d13aTR">Jeśli powyższy test zakończy się niepowodzeniem, test podstawowy  <em>13.A-HeadingDescriptive</em> również kończy się niepowodzeniem.</p>

## 13.B Procedura testowa dla programowych nagłówków wizualnych
Identyfikator testu podstawowego: _13.B-VisHeadingProg_

### Identyfikacja treści
<p id="d13bIC">Wizualnie widoczne nagłówki, które oznaczają sekcje treści. Nagłówki są często pisane większą, pogrubioną czcionką, są oddzielone od akapitów dodatkowymi odstępami (choć nie zawsze). Zwróć uwagę na hierarchię i strukturę każdego nagłówka w odniesieniu do innych nagłówków na stronie lub ekranie.</p>

Wizualnie widoczne nagłówki, które oznaczają sekcje treści. Nagłówki są często pisane większą, pogrubioną czcionką, oddzieloną od akapitów dodatkowymi odstępami (choć nie zawsze). Zwróć uwagę na hierarchię i strukturę każdego nagłówka w odniesieniu do innych nagłówków na stronie.

### Instrukcja testowania
1.	Sprawdź, czy wszystkie nagłówki wizualne są określane programowo i czy programowe poziomy nagłówków logicznie pasują do wizualnej prezentacji nagłówka w strukturze nagłówka [KS 1.3.1]:

1.  Sprawdź, czy wszystkie wizualne nagłówki są [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable) i czy programowe poziomy nagłówków logicznie pasują do wizualnej prezentacji nagłówka w strukturze nagłówka:
    -  Ważniejsze działy powinny mieć wyższy priorytet poziomu nagłówka. Na przykład, nagłówek poziomu 1 jest poziomem wyższym niż nagłówek poziomu 2, który jest wyższy niż nagłówek poziomu 3.
    -  Nagłówki o równym lub wyższym poziomie rozpoczynają nowe sekcję; nagłówki o niższy poziomie rozpoczynają nowe podsekcje, które są częścią sekcji wyższego poziomu.

### Wynik testów

<p id="d13bTR">Jeśli powyższy test zakończy się niepowodzeniem, test podstawowy <em>13.B-VisHeadingProg</em> również  kończy się niepowodzeniem.</p>


## 13.C Procedura testowa dla nagłówków określonych programowo
Identyfikator testu podstawowego: _13.C-ProgHeadingVisual_

### Identyfikacja treści
Programowo określane nagłówki: od nagłówka poziomu 1 do nagłówka poziomu 6.

### Instrukcja testowania
1.  Sprawdź, czy każdy programowo określany nagłówek służy również jako wizualny nagłówek na stronie. Treść, która nie jest nagłówkiem wizualnym, nie powinna być oznakowana jako nagłówek (na przykład znacznika nagłówka nie należy używać do wyróżniania elementu, który nie jest tytułem dla następującej po nim treści). [KS 1.3.1]

### Wynik testów
<p id="d13cTR">Jeżeli powyższy test zakończy się niepowodzeniem, wówczas test podstawowy <em>13.C-ProgHeadingVisual</em> kończy się niepowodzeniem.</p>

## 13.D Procedura testowa dla wykazów widocznych wizualnie
Identyfikator testu podstawowego: _13.D-List_

### Identyfikacja treści
Widoczne wizualnie listy, które są wyświetlane jako grupa elementów, zwykle znajdujących się jeden pod drugim. Wyklucz menu nawigacyjne. Określ typ listy:
-   **Lista nieuporządkowana** nie są numerowane ani literowane. List nieuporządkowanych używa się w przypadkach, gdy kolejność elementów nie jest istotna, ani nie ma konieczności odwoływania się do konkretnych pozycji na liście według liczby/litery.
-   **Lista uporządkowana** jest numerowana lub literowana sekwencyjnie, a jeśli to konieczne, także hierarchicznie (np. 1, 2, 2a, 2ai, itd.). List uporządkowanych używa się tam, gdzie ważna jest kolejność albo konieczne jest odwoływanie się do konkretnych pozycji na liście według liczby/litery.
-   **Lista opisów** (asocjacji, dawniej definicji, <code>dl</code>) używa się do grupowania dowolnych danych w zestawy nazwa-wartość. Rolę grupy nazwa-wartość mogą spełniać terminy i ich definicje, elementy metadanych i ich wartości oraz dowolne inne grupy danych, na przykład autorzy i tytuły ich książek. Są one powszechne stosowane w słownikach.

### Instrukcja testowania
1.  Dla każdej widocznej wizualnej listy:
    -  Sprawdź, czy treść, która ma wygląd listy (z punktorami lub bez), a nie zawiera elementów w uporządkowanej kolejności, jest oznaczona jako lista punktowana. [KS 1.3.1]
    -  Sprawdź, czy treść, które ma wygląd listy numerowanej, jest oznaczona jako lista numerowana lub wielopoziomowa. [KS 1.3.1].


### Wynik testów
<p id="d13dTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>13.D-List</em> również kończy się niepowodzeniem.</p>


##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
- Nie ma testu sprawdzającego, czy listy programowe są listami widocznymi wizualnie.
## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:


- {% include techniki/G115.md %} ORAZ {% include techniki/H49.md %}
- {% include techniki/G117.md %}
- {% include techniki/G130.md %}
- {% include techniki/H42.md %}
- {% include techniki/H48.md %}
- {% include techniki/PDF9.md %}
- {% include techniki/PDF21.md %}
- {% include techniki/F43.md %}
