---
title: 14. Tabele


sidebar: testy_sidebar
permalink: tz-14-tabele
folder: testy/tz
---

## Cel scenariusza testowego

Celem tego scenariusza testowego jest sprawdzenie, czy struktury tabel i relacje są programowo możliwe do ustalenia, tak aby informacje ważne dla zrozumienia były widoczne dla wszystkich użytkowników, w tym korzystających z technologii wspomagających. Elementy, które mają wspólne cechy, mogą być zorganizowane w tabeli danych, w której związek między komórkami dzielącymi ten sam wiersz lub kolumnę oraz związek każdej komórki z jej nagłówkiem wiersza i / lub kolumny są niezbędne do zrozumienia. Kiedy tak się dzieje, powinno istnieć odpowiednie programowe powiązanie, aby tabela ułatwiła nawigację i zrozumienie relacji między komórkami tabeli dla użytkowników technologii wspomagających. Gdy struktura tabeli jest używana tylko do celów układu, elementy struktury tabeli danych HTML, takie jak nagłówki i atrybuty zasięgu, nie powinny być używane, ponieważ może to powodować zamieszanie dla użytkowników technologii wspomagających.

Scenariusz „Tabele” obejmuje trzy testy:

1.	Test 14.A: 1.3.1-oznakowanie-tabeli
2.	Test 14.B: 1.3.1-powiazanie-nagłowkow-komorek
3.	Test 14.C: 1.3.1-tabela-układu



## Tabele danych

### Test 14.A 1.3.1-identyfikacja-tabeli

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.1-oznakowanie-tabeli | 14.A    | Każda tabela danych ma programowy znacznik, aby zidentyfikować ją jako tabelę. |

### Cel testu 14.A 1.3.1-identyfikacja-tabeli

Celem tego testu jest sprawdzenie, czy każda tabela danych została określona programowo, dzięki czemu technologie wspomagające rozpoznają ją jako tabelę.  
Mówiąc ogólnie, jeśli używana jest tabela danych, należy ją zakodować jako tabelę danych zgodnie ze specyfikacją HTML; nie można po prostu umieścić na stronie obrazu tabeli danych lub użyć stylizacji, aby treść wyglądała jak tabela. 

Tabele danych to struktury, w których treść znajduje się w&nbsp;odpowiednio rozmieszczonych polach nazywanych komórkami. Pola te utworzone są przez poziome i pionowe linie. Miejsca pomiędzy dwiema sąsiednimi pionowymi liniami nazywa się kolumnami, a miejsce pomiędzy dwiema sąsiednimi poziomymi liniami nazywa się wierszami. Komórki tytułujące kolumny lub wiersze nazywa się nagłówkami lub komórkami nagłówków. Wszystkie inne nazywa się komórkami danych.  

Aby treści tabeli mogły być przekazane użytkownikom technologii wspomagających, dane w komórkach wymagają nagłówków kolumn lub wierszy albo kolumn i wierszy, opisujących treść komórek danych. Kolejność odczytu danych w tabeli nie ma sensu bez nagłówków. Dokładne kodowanie tabeli danych zachowuje relację informacji w tabeli, nawet gdy użytkownicy nie widzą tabeli lub format prezentacji został zmieniony.

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-3-1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships).

### Metody i narzędzia testowe 
1.	ANDI: tabele > Analizuj następną tabelę

### Identyfikacja treści

Wszystkie tabele danych (w tym obrazy tabel danych), w których komórki danych, aby je zrozumieć, wymagają nagłówków.

**Uwaga:**

-   Aby pomóc w identyfikacji tabel danych, użyj ANDI::

    1.  Uruchom ANDI: struktury, a następnie wybierz łącze „kolejność czytania”.

    2.  Znaczniki dodane do strony wskazują kolejność, w jakiej technologia wspomagająca odczyta treść

-   Tabele danych to tabele, w których informacje w komórkach wymagają nagłówków wierszy lub kolumn, aby odpowiednio opisać treść komórek. Kolejność odczytywania treści w tabeli danych nie ma sensu bez nagłówków. Zrozumienie treści tabeli nie wymaga jej czytania według kolejności danych. 


-   **WYKLUCZ** treść, która nie wymaga nagłówków wierszy lub kolumn, aby ją zrozumieć:

    -   **tabele układu**, czyli tabele, które służą do rozmieszczania na stronie internetowej treści, które nie mają charakteru danych tabelarycznych, aby uzyskać pewien efekt wizualny bez powiązania informacyjnego między nagłówkami a informacjami w komórkach danych. Treść jest zrozumiała, gdy jest odczytywana w zaznaczonej kolejności.

    -   W przypadku treści prezentowanych wizualnie w tabeli, ale zrozumiałych po odczytaniu w&nbsp;zaznaczonej kolejności czytania, treść nie wymaga struktury tabeli danych. Może się to zdarzyć, gdy do wizualnego przedstawienia informacji zastosowano technikę CSS.

### Zastosowanie

Test 14.A 1.3.1-identyfikacja-tabeli **nie ma zastosowania**, jeśli na stronie nie ma tabel danych. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Uruchom ANDI: tabele.

    1.  Ustal, czy ANDI wykrywa i wyróżnia tabele danych.

        1.  Jeśli moduł tabel nie wyświetla się jako opcja na liście wyboru modułów, to znaczy, że ANDI nie wykrył na stronie żadnej tabeli określonej programowo (co oznacza, że treść prezentowana wizualnie w tabeli nie ma programowego znacznika identyfikującego ją jako tabelę).

        2.  Jeśli moduł ANDI:tabele się wyświetla, użyj przycisku „Analizuj następną tabelę”, aby kolejno podświetlić wykryte tabele na stronie. Jeśli dana tabela nie jest obrysowana przez ANDI i / lub nie jest możliwe przejście do niej za pomocą ANDI, oznacza to, że ANDI nie wykrył tej tabeli programowo (co oznacza, że zawartość prezentowana wizualnie w tej tabeli nie ma programowego znacznika do jej identyfikacji jako tabeli).

2.  Przejrzyj wszystkie tabele danych wykorzystujące `role="presentation"`.

   1.  ANDI wyświetli `role="presentation"` w informacjach o elemencie i / lub w obszarze Alerty dostępności.

   2.  Tabela danych zawierająca `role="presentation"` nie przekaże semantyki tabeli do czytnika ekranu i nie przejdzie tego testu.

3.  Wyjście ANDI wyświetli alert, gdy rola ARIA `role="table"` nie została poprawnie zakodowana.

4.  Użyj przycisków Analizuj poprzednią/następną tabelę w ANDI, aby przejść do każdej z tabel wykrytych na stronie.

### Ocena wyników

Jeśli wszystkie twierdzenia poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.3.1:


1.  Możliwe jest nawigowanie w ANDI:tabele do każdej tabeli danych za pomocą przycisków ANDI Analizuj poprzednią / następną tabelę **oraz**

2.  Tabela danych **nie ma** przypisanej roli ARIA `role="presentation"`, **oraz**

3.  Tabela danych NIE zawiera żadnych alertów tabeli ANDI dotyczących nieprawidłowego użycia atrybutów tabeli ARIA.


3.	ANDI nie zgłasza podczas przeglądania tabel żadnych alertów dotyczących nieprawidłowego użycia atrybutów ARIA `role="table"`.

## Powiązanie komórek danych z nagłówkami

### Test 14.B 1.3.1-powiazanie-komorek-z-naglowkami

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.1-powiazanie-komorek-z-naglowkami | 14.B    | Wszystkie komórki danych są programowo powiązane z odpowiednimi nagłówkami. |

### Cel testu 1.3.1-powiazanie-komorek-z-naglowkami


Celem tego testu jest sprawdzenie, czy wszystkie komórki danych w każdej tabeli danych są programowo powiązane ze wszystkimi odpowiednimi nagłówkami. Dzięki temu technologie wspomagające mogą „zrozumieć” związek komórek danych z nagłówkami wierszy lub kolumn i w pełni przekazać te powiązania użytkownikom. Bez programowego powiązania komórek danych ze wszystkimi odpowiednimi nagłówkami użytkownik technologii wspomagającej może nie być w stanie w pełni zrozumieć treści.

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-3-1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships).

### Metody i narzędzia testowe 
1.	ANDI: tabele > Analizuj poprzenią / następną tabelę
2.  ANDI: tabele > przyciski Poprzedni / Następny element

### Identyfikacja treści

Wszystkie tabele danych, w których komórki danych, aby je zrozumieć, wymagają nagłówków.

**Uwaga:**

-   Aby pomóc w identyfikacji tabel danych, użyj ANDI::

    1.  Uruchom ANDI: struktury, a następnie wybierz łącze „kolejność czytania”.

    2.  Znaczniki dodane do strony wskazują kolejność, w jakiej technologia wspomagająca odczyta treść

-   Tabele danych to tabele, w których informacje w komórkach wymagają nagłówków wierszy lub kolumn, aby odpowiednio opisać treść komórek. Kolejność odczytywania treści w tabeli danych nie ma sensu bez nagłówków. Zrozumienie treści tabeli nie wymaga jej czytania według kolejności danych. 


-   **WYKLUCZ** treść, która nie wymaga nagłówków wierszy lub kolumn, aby ją zrozumieć:

    -   **tabele układu**, czyli tabele, które służą do rozmieszczania na stronie internetowej treści, które nie mają charakteru danych tabelarycznych, aby uzyskać pewien efekt wizualny bez powiązania informacyjnego między nagłówkami a informacjami w komórkach danych. Treść jest zrozumiała, gdy jest odczytywana w zaznaczonej kolejności.

    -   W przypadku treści prezentowanych wizualnie w tabeli, ale zrozumiałych po odczytaniu w&nbsp;zaznaczonej kolejności czytania, treść nie wymaga struktury tabeli danych. Może się to zdarzyć, gdy do wizualnego przedstawienia informacji zastosowano technikę CSS.

### Zastosowanie

Test  14.B 1.3.1-powiazanie-komorek-z-naglowkami **nie ma zastosowania**, jeśli na stronie nie ma tabel danych. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Użyj przycisków Analizuj następną/poprzednią tabelę, aby przenosić punkt uwagi na każdej tabeli.

2.  Przejdź do każdej komórki danych za pomocą: tabele. Użyj przycisków Poprzedni element / Następny element, aby poruszać się po każdej tabeli, komórka po komórce

3.  Sprawdź dane wyjściowe ANDI dla każdej komórki danych i / lub sprawdź wizualne wyróżnianie tabeli danych, aby ustalić, czy w tabeli określono odpowiednio wszystkie nagłówki dla każdej komórki danych.
 
   1. ANDI wyróżnia wybraną komórkę danych jasnoróżową otoczką. Nagłówki kolumn i wierszy są podświetlone na ciemnoróżowo.
   
   2. Wyjściu ANDI wyświetla również nagłówki. Ostatnim elementem w danych wyjściowych jest treść komórki danych.
   3. Przejrzyj podświetloną treść i wynik ANDI, aby określić, które nagłówki wierszy i kolumn są powiązane z każdą komórką danych w tabeli.


**Uwaga**: W teście należy uwzględnić wszelkie zmiany w tabelach danych, które nastąpią automatycznie lub w wyniku interakcji ze stroną.


### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.3.1:


1.  Tabela danych odpowiednio identyfikuje relacje nagłówka dla każdej komórki danych.

### Uwaga

-   W tym teście należy uwzględnić wszelkie zmiany w tabelach danych, które nastąpią automatycznie lub w wyniku interakcji ze stroną.

## Tabele układu

### Test 14.C 1.3.1-tabele-ukladu

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.1-tabele-ukladu | 14.C    | Tabela układu NIE oznacza tabeli za pomocą roli ARIA 'role="table"' I NIE zawiera struktury nagłówka tabeli ani elementów relacji i / lub powiązanych atrybutów. |

### Cel testu 14.C 1.3.1-tabele-ukladu

Celem tego testu jest sprawdzenie, czy tabele używane tylko do rozmieszczenia treści (układu) nie używają elementów struktury tabeli danych. Jeśli w oznakowaniu tabel układu używa się znaczników strukturalnych (semantycznych), to informacje o strukturze tabeli przekazywane użytkownikom czytników ekranu nie mają żadnej wartości i mogą być rozpraszające lub mylące. 


Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-3-1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships).


### Metody i narzędzia testowe 
1.	ANDI: tabele > Analizuj poprzenią / następną tabelę


### Identyfikacja treści

Tabele określone programowo, w których struktura tabeli jest używana wyłącznie do celów układu.

**WYKLUCZ** tabele danych.

**Uwaga:**

-   Aby znaleźć na stronie tabele określone programowo, użyj ANDI: tabele (jak w poprzednim teście).

    1.  Jeśli modułu ANDI:tabele nie ma na liście opcji ANDI, wówczas na stronie nie ma określonej programowo.

-   Aby znaleźć tabele układu:

    1.  Uruchom ANDI:struktury, a następnie wybierz łącze „porządek czytania”.

    2.  Wskaźniki dodane do strony wskazują kolejność, w jakiej technologia wspomagająca odczyta treść.

- Treść znajdująca się w tabeli układu nie wymaga nagłówków wierszy lub kolumn do zrozumienia. Treść ta powinna być sensowna, gdy jest czytana w kolejności czytania określonej przez ANDI.


### Zastosowanie

Test  14.C 1.3.1-tabele-ukladu **nie ma zastosowania**, jeśli na stronie nie ma tabel układu. W takim przypadku oznacz wynik testu jako **ND**.


### Jak testować

1.  Kontynuuj test 14.A.

    1.  Jeśli moduł ANDI: tabele nie wyświetla się jako opcja na liście wyboru modułów, to znaczy, że ANDI nie wykrył na stronie tabeli określonej programowo, czyli że nie ma na stronie treści, która ma programowe znaczniki określające treść jako tabelę.

    2.  Jeśli moduł ANDI: tabele wyświetla się, użyj przycisku „Analizuj następną tabelę”, aby kolejno podświetlić wykryte tabele na stronie. Jeśli jakaś tabela nie zostanie wyróżniona przez ANDI lub przejście do niej za pomocą ANDI jest niemożliwe, oznacza to, że ANDI nie wykrył jej programowo  (co oznacza, że treść prezentowana wizualnie jako tabela nie jest określona programowo, czyli nie posiada znakowania opisującego ją jako tabelę).

2.  Sprawdź daną wyjściową „Element” w ANDI, aby ustalić, czy układ używa `role="table"`.

    **Uwaga**: szukasz „Element: `role="table"`, a nie „Element: `<table>`”. (Atrybut ARIA `role=table"` służy do definiowania tabeli danych. Tego atrybutu nigdy nie należy używać w tabeli układu.) 

3.  Sprawdź dane wyjściowe ANDI i wszelkie powiązane alerty, aby ustalić, czy `<table>` zawiera elementy i atrybuty struktury nagłówka (np. `<th>` lub `scope="row"`).

    1.  Jeśli tabela ma przypisany atrybut ARIA `role="presentation"` (lub `role="none"`) i jeśli w tabeli oznakowano(określono programowo) także nagłówki (np. używając `<th>`, `scope="row"`, `scope="col"`,) ANDI zapewni odpowiedni alert; zignoruj ten alert w tabeli układu. Tabela zawierająca `role="presentation"` (lub `role="none"`) nie przekaże semantyki tabeli do czytnika ekranu. Dlatego, jeśli tabela jest rzeczywiście tabelą układu, semantykę struktury tabeli (np. `<th>`, `scope="row"`) można zignorować.

### Ocena wyników

Jeśli którekolwiek twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.3.1:

1.  ANDI nie wykrył tabeli układu **lub**

2.  element `<table>` ma atrybut `role="presentation"` lub `role="none"`, **lub**

3.  Oba twierdzenia poniżej są **prawdą**:

    1.  Tabela nie używa atrybutu `role="table"` lub jakiegokolwiek powiązanego z rolą tabeli atrybutu (np., `role="row"`, `role="columnheader"`) **oraz**

    2.  Tabela nie używa żadnego elementu ani atrybutu, określającego strukturę danych tabeli i powiązania między komórkami i nagłówkami (np. `<th>`, `scope="row"`)

## Obowiązujące normy

- {% include ks/1-3-1.md %}
- {% include ks/1-3-2.md %}
- {% include ks/4-1-2.md %}
- [12. Tabele danych](ICT-12-tabele-danych)
