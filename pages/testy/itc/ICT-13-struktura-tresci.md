---
title: 13. Struktura treści


sidebar: testy_sidebar
permalink: ICT-13-struktura-tresci
folder: testy/itc
---

## Wymagania dostępności
----------------------
-   [KS WCAG: 2.4.6 Nagłówki i etykiety](http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html) -- Nagłówki i etykiety opisują temat lub cel treści.
-   [KS WCAG: 1.3.1 Informacje i relacje](http://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html) -- Informacje, struktura oraz relacje pomiędzy treściami przedstawiane w treści mogą być odczytane przez program komputerowy lub są dostępne w postaci tekstu.

## Uzasadnienie metody badania
------------------------------
-   Widoczne nagłówki muszą być [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable), reprezentować strukturę treści i opisywać treści następujące po nagłówkach.
-   Widoczne listy wizualne  muszą być [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable), zgodnie z ich typami (uporządkowane, nieuporządkowane, listy definicji).

## Ograniczenia, założenia lub wyjątki
--------------------------------------
-   Strona, na której znajduje się tylko jeden nagłówek, nie posiada struktury na poziomie nagłówków i nie może być testowana pod kątem struktury nagłówków.
-   Strony mogą mieć więcej niż jeden nagłówek poziomu 1 lub mogą nie posiadać nagłówka poziomu 1.
-   Nagłówek poziomu 1 nie musi być ściśle taki sam jak tytuł strony.
-   Kolejność poziomów nagłówków nie zawsze może być zgodna z porządkiem liczenia, a mimo to będzie prawidłowa ponieważ odnosi się do struktury wizualnej/ważkości podanej za pomocą widocznych nagłówków na stronie. Na przykład nagłówek &lt;h2&gt; może być zastosowany dla oznaczenia struktury nawigacyjnej poprzedzającej tytuł &lt;h1&gt; rozpoczynający główną zawartość na stronie. Podobnie po &lt;h1&gt; może następować &lt;h3&gt; bez &lt;h2&gt; między nimi.
-   Nie wszystkie listy wymagają znaczników. Na przykład zdania zawierające wykazy rozdzielone przecinkami mogą nie potrzebować znaczników list ([H48: Używanie ol, ul i dl dla list lub grup łączy](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/H48)).

## Procedura testu dla KS 2.4.6 Nagłówki i etykiety
---------------------------------------------------
### Identyfikacja treści
Widoczne nagłówki, które oznaczają sekcje treści. Nagłówki mają często większą, pogrubioną czcionkę, są oddzielone od akapitów dodatkowymi odstępami (choć nie zawsze). Zwróć uwagę na hierarchię i strukturę każdego nagłówka w odniesieniu do innych nagłówków na stronie.

### Instrukcja testowania
1.  Sprawdź, czy każdy nagłówek opisuje temat lub cel następującej po nim treści.


### Wynik testów
Jeżeli powyższa próba zakończy się niepowodzeniem, wówczas test KS 2.4.6 oraz wymaganie podstawowe nr 13 kończy się niepowodzeniem.

## Procedura testu dla KS 1.3.1 Informacje i relacje
----------------------------------------------------
### Teksty wyglądające jak nagłówki

#### Identyfikacja treści
Widoczne nagłówki, które oznaczają sekcje treści. Nagłówki mają często większą, pogrubioną czcionkę, są oddzielone od akapitów dodatkowymi odstępami (choć nie zawsze). Zwróć uwagę na hierarchię i strukturę każdego nagłówka w odniesieniu do innych nagłówków na stronie.

#### Instrukcja testowania
1.  Sprawdź, czy wszystkie wizualne nagłówki są [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable) i czy programowe poziomy nagłówków logicznie pasują do wizualnej prezentacji nagłówka w strukturze nagłówka:
    1.  Ważniejsze nagłówki powinny mieć najwyższy poziom. Na przykład, &lt;h1&gt; jest poziomem wyższym niż &lt;h2&gt;, który jest wyższy niż &lt;h3&gt;.
    2.  Nagłówki z jednakowym lub wyższym poziomem rozpoczynają nowe sekcję; nagłówki z niższym poziomem rozpoczynają nowe podsekcje, które są częścią sekcji o wyższym poziomie.
    3.  HTML lub ARIA programowo identyfikują każdy nagłówek. Gdy używane są oba sposoby znakowania, poziomy nagłówków muszą się zgadzać.
        -   [H42](https://www.w3.org/TR/WCAG20-TECHS/H42.html): każdy nagłówek może być oznaczony od &lt;h1&gt; do &lt;h6&gt;.
        -   [ARIA12](https://www.w3.org/TR/WCAG20-TECHS/ARIA12.html): każdy nagłówek może być oznaczony atrybutami role="heading" ”nagłówek” i aria-level="\#\". Domyślnym poziom nagłówka jest „2”, jeśli nie podano atrybutuaria-level.

#### Wynik testów
Jeżeli powyższa próba zakończy się niepowodzeniem, wówczas test KS 1.3.1 oraz wymaganie podstawowe nr 13 kończy się niepowodzeniem.

### Nagłówki określone programowo

#### Identyfikacja treści
Nagłówki [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable): od &lt;h1&gt; do &lt;h6&gt; lub za pomocą atrybutu ARIA role="heading".

#### Instrukcja testowania
1.  Sprawdź, czy każdy nagłówek zdefiniowany programowo służy również jako rzeczywisty nagłówek na stronie. Treść, która nie jest rzeczywistym nagłówkiem, nie powinna być oznakowana jako nagłówek (na przykład znacznika nagłówka nie należy używać do podkreślania elementu, który nie jest tytułem dla następującej po nim treści).


#### Wynik testów
Jeżeli powyższa próba zakończy się niepowodzeniem, wówczas test KS 1.3.1 oraz wymaganie podstawowe nr 13 kończy się niepowodzeniem.

### Wykazy wyglądające jak listy
Ten warunek testu NIE MA ZASTOSOWANIA, jeśli nie ma żadnych widocznych list.

#### Identyfikacja treści
Widoczne wizualnie listy. Dla każdej listy określ, czy wygląda na uporządkowaną, nieuporządkowaną czy listę asocjacji.
-   **Listy uporządkowane** numeruje się sekwencyjnie, a jeśli to konieczne, także hierarchicznie (np. 1, 2, 2a, 2ai, itd.). List uporządkowanych używa się tam, gdzie ważna jest kolejność albo konieczne jest odwoływanie się do konkretnych pozycji na liście według liczby/litery.
-   **Listy nieuporządkowane** nie są numerowane i używa się ich w przypadkach, gdy kolejność elementtów nie jest istotna, ani nie ma konieczności odwoływania się do konkretnych pozycji na liście według liczby/litery.
-   **List opisów** (asocjacji, dawniej definicji) (dl) używa się do grupowania dowolnych danych w zestawy nazwa-wartość. Rolę grupy nazwa-wartość mogą spełniać terminy i ich definicje, elementy metadanych i ich wartości oraz dowolne inne grupy danych, na przykład autorzy i tytuły ich książek.

*Uwaga*: Programiści mogą używać elementów listy do prezentacji pogrupowanych elementów, takich jak menu i podmenu, usuwając z nich punktownie lub numerację. Takie użycie elementów listy jest dopuszczalne i zgodne z warunkami testu określonymi poniżej.

#### Instrukcja testowania
1.  Dla każdej widocznej listy:
    1.  Sprawdź, czy treści, które mają wygląd listy (z punktorami lub bez), a nie zawierają elementów w uporządkowanej kolejności, zostały oznaczone jako listy nieuporządkowane.
    2.  Sprawdź, czy treści, które mają wygląd listy, zostały oznaczone jako listy uporządkowane.
    3.  Sprawdź, czy treści, które prezentują grupy elementów powiązanych na zasadzie nazwa-wartość sa oznakowane jako listy opisów.


#### Wynik testów
Jeżeli powyższa próba zakończy się niepowodzeniem, wówczas test KS 1.3.1 oraz wymaganie podstawowe nr 13 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
----------------------------------------------------------
## Techniki WCAG 2.1
--------------------
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [ARIA12: Używanie atrybutu role=heading oraz aria-level="\#"do identyfikacji nagłówków](https://www.w3.org/TR/WCAG20-TECHS/ARIA12.html)
-   [H42: Używanie znaczników h1-h6 do identyfikacji nagłówków](https://www.w3.org/TR/WCAG20-TECHS/H42.html)
-   [G130: Zapewnienie opisowych nagłówków](https://www.w3.org/TR/WCAG20-TECHS/G130.html)
-   [G115: Używanie znaczników semantycznych do oznaczania struktury](http://www.w3.org/TR/WCAG20-TECHS/G115.html) AND [H49: Using semantic markup to mark emphasized or special text](http://www.w3.org/TR/WCAG20-TECHS/H49.html)
-   [G117: Używanie tekstu do przekazywania informacji przekazywanych przez zmiany w sposobie prezentacji tekstu](http://www.w3.org/TR/WCAG20-TECHS/G117.html)
-   [H48: Używanie ol, ul i dl dla list lub grup łączy](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/H48)
