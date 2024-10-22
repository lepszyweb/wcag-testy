---
title: 13. Struktura treści
last_updated: 22 października 2024

sidebar: testy_sidebar
permalink: ICT-13-struktura-tresci
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/2-4-6.md %}
- {% include ks/1-3-1.md %}

## Uzasadnienie metody testowej

-   Widoczne nagłówki muszą być [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable), reprezentować strukturę treści i opisywać treść, która następuje po nagłówkach.
-   Widoczne listy wizualne  muszą być [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable), zgodnie z ich typami (uporządkowane, nieuporządkowane, listy definicji).

## Ograniczenia, założenia lub wyjątki

-   Strona, na której znajduje się tylko jeden nagłówek, nie ma struktury na poziomie nagłówków i nie może być testowana pod kątem struktury nagłówków.
-   Strony mogą mieć więcej niż jeden nagłówek poziomu 1 lub nie mieć nagłówka poziomu 1.
-   Nagłówek poziomu 1 na stronie nie musi być zgodny z tytułem strony.
-   Kolejność poziomów nagłówków nie zawsze może być zgodna z porządkiem liczenia, a mimo to będzie prawidłowa, ponieważ odnosi się do struktury wizualnej/ważkości podanej za pomocą widocznych nagłówków na stronie. Na przykład nagłówek `<h2>` może być zastosowany dla oznaczenia struktury nawigacyjnej poprzedzającej tytuł `<h1>` rozpoczynający główną zawartość na stronie. Podobnie po `<h1>` może następować `<h3>` bez `<h2>` między nimi.
-   [ARIA 1.2](https://www.w3.org/TR/wai-aria-1.2/#heading): Aby mieć pewność, że elementy pełniące rolę nagłówka są zorganizowane w logiczny konspekt, autorzy muszą użyć atrybutu aria-level, aby wskazać właściwy poziom zagnieżdżenia. (Jest to zmiana w stosunku do [ARIA 1.1](https://www.w3.org/TR/wai-aria-1.1/#heading),  gdzie domyślnym był poziom 2.)
-   Nie wszystkie listy wymagają oznaczania. Na przykład zdania zawierające wykazy rozdzielone przecinkami mogą nie wymagać znaczników list ([H48: Użycie ol, ul i dl dla list lub grup łączy](https://www.w3.org/WAI/WCAG22/Techniques/html/H48)).
-   Test list widocznych wizualnie nie powinien obejmować menu nawigacyjnych. Chociaż listy programowe są często używane do tworzenia menu nawigacyjnych, menu mogą być również tworzone przy użyciu innych technik.


## 13.A Procedura testowa dla nagłówków opisowych
Identyfikator testu podstawowego: _13.A-HeadingDescriptive_

### Identyfikacja treści
Wizualnie widoczne nagłówki, które oznaczają sekcje treści. Nagłówki są często pisane większą, pogrubioną czcionką, są oddzielone od akapitów dodatkowymi odstępami (choć nie zawsze). Zwróć uwagę na hierarchię i strukturę każdego nagłówka w odniesieniu do innych nagłówków na stronie lub ekranie.

### Instrukcja testowania
1.  Sprawdź, czy każdy nagłówek opisuje temat lub cel następującej po nim treści. [KS 2.4.6]

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy  _13.A-HeadingDescriptive_ również kończy się niepowodzeniem.

## 13.B Procedura testowa dla programowych nagłówków wizualnych
Identyfikator testu podstawowego: _13.B-VisHeadingProg_

### Identyfikacja treści
Wizualnie widoczne nagłówki, które oznaczają sekcje treści. Nagłówki są często pisane większą, pogrubioną czcionką, są oddzielone od akapitów dodatkowymi odstępami (choć nie zawsze). Zwróć uwagę na hierarchię i strukturę każdego nagłówka w odniesieniu do innych nagłówków na stronie lub ekranie.

### Instrukcja testowania
1.  Sprawdź, czy wszystkie wizualne nagłówki są [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable) i czy programowe poziomy nagłówków logicznie pasują do wizualnej prezentacji nagłówka w strukturze nagłówka:
    -  Ważniejsze działy powinny mieć wyższy priorytet poziomu nagłówka. Na przykład, &lt;h1&gt; jest poziomem wyższym niż &lt;h2&gt;, który jest wyższy niż &lt;h3&gt;.
    -  Nagłówki z jednakowym lub wyższym poziomem rozpoczynają nowe sekcję; nagłówki z niższym poziomem rozpoczynają nowe podsekcje, które są częścią sekcji wyższego poziomu.
    -  HTML lub ARIA programowo określają każdy nagłówek. Gdy używane są oba sposoby znakowania, poziomy nagłówków muszą się zgadzać.
        -   [H42](https://www.w3.org/WAI/WCAG22/Techniques/html/H42): każdy nagłówek może być oznaczony od `<h1>` do `<h6>`.
        -   [ARIA12](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA12): każdy nagłówek może być oznaczony atrybutami role="heading" ”nagłówek” i aria-level="\#\". 
    -  Gdy stosowane są obie techniki, ARIA ma pierwszeństwo, a poziom nagłówka jest wskazywany przez poziom ARIA.
	
### Wynik testów
Jeśli powyższy test zakończy się niepowodzeniem, test podstawowy _13.B-VisHeadingProg_ również  kończy się niepowodzeniem.


## 13.C Procedura testowa dla nagłówków określonych programowo
Identyfikator testu podstawowego: _13.C-ProgHeadingVisual_

### Identyfikacja treści
Nagłówki [określone programowo](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable): od &lt;h1&gt; do &lt;h6&gt; lub za pomocą atrybutu ARIA `role="heading"`.

### Instrukcja testowania
1.  Sprawdź, czy każdy każdy programowo określany nagłówek służy również jako rzeczywisty wizualny nagłówek na stronie. Treść, która nie jest nagłówkiem wizualnym, nie powinna być oznakowana jako nagłówek (na przykład znacznika nagłówka nie należy używać do wyróżniania elementu, który nie jest tytułem dla następującej po nim treści).

### Wynik testów
Jeżeli powyższy testzakończy się niepowodzeniem, wówczas test podstawowy _13.C-ProgHeadingVisual_ kończy się niepowodzeniem.


## 13.D Procedura badawcza dla wykazów widocznych wizualnie
Identyfikator testu podstawowego: _13.D-List_

### Identyfikacja treści
Widoczne wizualnie listy, które są wyświetlane jako grupa elementów, zwykle znajdujących się jeden pod drugim. Wyklucz menu nawigacyjne. Określ typ listy:
-   **Lista nieuporządkowana** nie są numerowane ani literowane. List nieuporządkowanych używa się w przypadkach, gdy kolejność elementów nie jest istotna, ani nie ma konieczności odwoływania się do konkretnych pozycji na liście według liczby/litery.
-   **Lista uporządkowana** numeruje się sekwencyjnie, a jeśli to konieczne, także hierarchicznie (np. 1, 2, 2a, 2ai, itd.). List uporządkowanych używa się tam, gdzie ważna jest kolejność albo konieczne jest odwoływanie się do konkretnych pozycji na liście według liczby/litery.
-   **Lista opisów** (asocjacji, dawniej definicji) (dl) używa się do grupowania dowolnych danych w zestawy nazwa-wartość. Rolę grupy nazwa-wartość mogą spełniać terminy i ich definicje, elementy metadanych i ich wartości oraz dowolne inne grupy danych, na przykład autorzy i tytuły ich książek. Są one powszechne stosowane w słownikach.

**Uwaga**: Ten warunek testowy NIE MA ZASTOSOWANIA, jeśli nie ma żadnych widocznych list.

### Instrukcja testowania
1.  Dla każdej widocznej wizualnej listy:
    -  Sprawdź, czy treść, która ma wygląd listy (z punktorami lub bez), a nie zawiera elementów w uporządkowanej kolejności, została oznaczone jako lista nieuporządkowana objętą znacznikiem `<ul>`, a każdy element na liście jest programowo elementem listy `<li>`. [KS 1.3.1]
    -  Sprawdź, czy treść, które ma wygląd listy numerowanej, została oznaczona jako lista uporządkowana znacznikiem `<ol>`, a każdy element na liście jest programowo elementem listy `<li>`. [KS 1.3.1].
    -  Sprawdź, czy treść, które prezentują grupy elementów powiązanych na zasadzie nazwa-wartość, są oznakowane jako listy opisów znacznikiem `<dl>`, każdy termin jest programowo terminem opisu (znacznik `<dt>`) a każdy opis jest programowo opisem definicji (znacznik `<dd>`. [KS 1.3.1]
**Uwaga**: Każdy termin może mieć więcej niż jeden opis.

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _13.D-List_ również kończy się niepowodzeniem.


##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
- Nie ma testu sprawdzającego, czy listy programowe są listami widocznymi wizualnie.
## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/ARIA12.md %}
- {% include techniki/G115.md %} ORAZ {% include techniki/H49.md %}
- {% include techniki/G117.md %}
- {% include techniki/G130.md %}
- {% include techniki/H42.md %}
- {% include techniki/H48.md %}
- {% include techniki/F43.md %}


