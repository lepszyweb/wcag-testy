---
title: 9. Treści powtarzane


sidebar: testy_sidebar
permalink: tz-09-tresci-powtarzane
folder: testy/tz
---


## Cel procedury testowej

Celem tej procedury jest sprawdzenie, czy użytkownikom zapewniono możliwości pomijania bloków treści  powtarzanych na wielu stronach, dzięki czemu można łatwo uzyskać dostęp do głównej treści strony. Celem jest również sprawdzenie, czy treści powtarzane na wielu stronach są na nich umieszczone w spójnej kolejności względnej oraz czy są w sposób spójny identyfikowane.

Spełnianie przez strony internetowe tych trzech kryteriów ma zapewnić, że użytkownicy z ograniczeniami poznawczymi lub wzrokowymi mogą w przewidywalny sposób nawigować po stronie, aby szybko i łatwo docierać do pożądanych treści.

Procedura testowa „Treści powtarzane” obejmuje trzy testy:

- Test 9A: 2.4.1-omijanie-tresci
- Test 9B: 3.2.3-spójna nawigacja
- Test 9C: 3.2.4-spójna identyfikacja

## Omijanie treści powtarzalnych

### Test 9.A: 2.4.1-omijanie-tresci

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.4.1-omijanie-tresci | 9.A   | Istnieje metoda ominięcia tylko za pomocą klawiatury powtarzanych treści. |


### Cel testu 9.A: 2.4.1-omijanie-tresci

Celem testu 2.4.1-omijanie-tresci jest ustalenie, czy na stronie istnieją metody na omijanie treści powtarzanych na wielu stronach oparte tylko na korzystaniu z klawiatury. Takie metody są niezbędne, aby użytkownicy z ograniczeniami ruchowymi lub wzrokowymi, którzy nawigują po stronach tylko za pomocą klawiatury, mogli łatwo przechodzić do głównej treści strony. Aby użytkownik mógł swobodnie omijać powtarzające się bloki treści, nie powinno być wymagane żadne dodatkowe narzędzia, takie jak technologia wspomagająca.     

Wyniki tego testu pozwalają ustalić, czy spełnione jest [kryterium sukcesu 2.4.1 Możliwość pominięcia bloków](https://wcag.lepszyweb.pl/#bypass-blocks).

**Uwaga**: Ten test obejmuje tylko takie metody omijania treści, które opierają się na klawiaturze. Nie uwzględnia innych wystarczających technik WCAG, które do ominięcia powtarzanych treści wymagają innych narzędzi:

- Zapewnienie elementów nagłówka na początku każdej sekcji treści.

- Używanie punktów orientacyjnych ARIA do określania regionów strony.

### Metody i narzędzia testowe 

1.	Klawiatura

2.	ANDI:interaktywne.

3.	ANDI:łącza/przyciski > przycisk „pokaż listę łączy” > łącza pomijające (jeśli istnieją).


### Identyfikacja treści

Ustal, czy istnieje blok lub bloki treści, które są powtarzane na innych stronach witryny.

-   Blokami treści powtarzanych na innych stronach mogą być zestawy łączy nawigacyjnych, nagłówki stron, banery. Mogą to być również zestawy łączy narzędziowych, np. zmiany ustawień, zestawy łączy do serwisów społecznościowych, takich jak Facebook, Twitter, Instagram czy LinkedIn, i inne  

-   Bloki treści nie muszą być dokładnie takie same na wszystkich stronach, aby można je było uznać za powtarzalne; bloki treści można uznać za powtarzające się, jeśli zawierają ten sam typ informacji lub służą temu samemu celowi.

    -  Przykładem jest strona internetowa, która ma zmieniające się reklamy po lewej stronie strony i blok łączy nawigacyjnych u góry każdej strony, które mogą oferować różne opcje zależne od treści strony.

**Uwagi**: 

-  Jeśli między dwoma powtarzającymi się blokami treści istnieje treść, która **nie jest powtarzana**, wówczas każdy blok powtarzanej treści wymaga osobnej funkcji omijania. Nie można takiej złożonej grupy bloków treści uznawać za jeden blok powtarzanej treści.  

-  **WYJATKI**: powtarzane pojedyncze słowa, frazy lub pojedyncze łącza nie są uważane za powtarzające się bloki treści.

-  Ponieważ większość przeglądarek internetowych zapewnia skróty klawiaturowe, które służą do przeniesienia punktu uwagi użytkownika na początek strony lub do paska adresu przeglądarki, udostępnianie metody omijania łączy nawigacyjnych znajdujacych się na dole strony internetowej (zwykle w stopce) może być niepotrzebne.

### Zastosowanie
Test 9A 2.4.1-omijanie-tresci **nie ma zastosowania** na stronach, na których nie ma bloków treści powtarzających się na innych stronach. Jeśli istnieje tylko pojedyncza strona internetowa, która nie jest częścią większej witryny, ten test **nie ma zastosowania**.

### Jak testować

1.  Startując od poczatku strony, użyj standardowych poleceń klawiatury, aby nawigować w przód do powtarzalnych bloków treści. **Uwaga**: Niektóre funkcje omijania mogą być niewidoczne, dopóki nie zostanie na nie przeniesiony fokus klawiatury.

2.  Uruchom ANDI: interaktywne, aby sprawdzić, czy istnieją łącza pomijające, opcje ukrywania, zwijane menu i inne elementy o podobnej funkcjonalności omijania 

    1.  **Uwaga**: Funkcja „porządek tabulacji” w ANDI w module elementy interaktywne, może pomóc w ocenie kolejności, w jakiej funkcje omijania pojawiają się na stronie w stosunku do innych treści.

    2.  Alternatywnie, uruchom ANDI: łącza/przyciski i wybierz przycisk  „pokaż listę łączy”. Ta metoda może ułatwić wyświetlanie łączy pomijający i elementów skryptowych, które mogą nie być łatwo zidentyfikowane wzrokowo lub za pomocą opcji „porządek tabulacji”.


3.  Ustal, czy zapewniono dostępną za pomocą klawiatury metodę pomijania powtarzających się treści (np. łącza pomijajace, skróty klawiaturowe, elementy skryptowe, itp.). **Uwaga**: Ramki mogą posłużyć jako metoda omijania w niekttórych przeglądarkach, a w innych nie. Nie można ich więc uznać za metodę wystarczajacą.  

4.  Użyj standardowych poleceń klawiatury, aby aktywować funkcje omijania.

    1.  Wiele bloków powtarzających się treści może wymagać kilku metod omijania bloków; ominięcie wszystkich bloków powtarzającej się treści może być niemożliwe za pomocą jednej metody.

    2.  Przenoszenie fokusa poza bloki powtarzanej treści może nie zawsze być wyraźnie widoczne, jeśli nie ma elementów, na które można ustawić fokus bezpośrednio po ominiętym bloku.


### Ocena wyników

Jeśli oba poniższe twierdzenia są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 2.4.1:


1.  Istnieje metoda ominięcia powtarzających się treści za pomocą klawiatury **oraz**

2.  Po aktywacji metoda działa, a blok powtarzającej się treści jest pomijany.

**Ważne**: 

- Jeśli bezpośrednio za omijanym blokiem treści nie ma interaktywnego elementu, który odbierałby fokus klawiatury, może nie być oczywiste, że nastąpiło przeniesienie punktu uwagi w inne miejsce strony (np. do treści głównej). Zmniejszenie wysokości okna przeglądarki może sprawić, że przeneisienie fokusa stanie się bardziej oczywiste.

- Każdy blok powtarzających się treści może mieć własną metodę omijania. 

- Żadna treść, która nie jest powtarzalna, nie może być częścią treści, która jest pomijana.

## Spójna nawigacja

### Test 9B: 3.2.3-spojna-nawigacja

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 3.2.3-spojna-nawigacja | 9.B     | Każdy element nawigacyjny występuje w tej samej względnej kolejności w odniesieniu do innych powtarzających się elementów na każdej stronie internetowej, na której się pojawia. |

### Cel testu 9B: 3.2.3-spojna-nawigacja

Celem testu 9B: 3.2.3-spojna-nawigacja jest sprawdzenie, czy na każdej stronie prezentacja i układ  elementów nawigacyjnych jest spójny dla użytkowników, którzy wchodzą w interakcje z powtarzającymi się treściami na zestawie stron internetowych i muszą znaleźć określone informacje lub funkcje więcej niż jeden raz.  Każdy mechanizm nawigacyjny powinien pojawić się w tej samej kolejności względnej na każdej stronie internetowej, na której się pojawia. 

Należy podkreślić, że użycie wyrażenia „ta sama względna kolejność” nie oznacza, że ​​nie można użyć menu podrzędnych lub że nie można użyć bloków dodatkowej nawigacji lub dodatkowych elementów struktury strony. 

Spójna nawigacja jest ważna dla wszystkich, pomaga szybko orientować się na stronach, nawigować po treści, lokalizować określone informacje i rozumieć strukturę strony. Szczególne znaczenie ma dla osób słabowidzących, które korzystają z powiększalników, aby wyświetlać niewielkie części ekranu i muszą dysponować wskazówkami wizualnymi, aby szybko lokalizowac powtarzajacee się treści. 
Prezentowanie powtarzających się treści w tej samej kolejjności jest również ważne dla użytkowników, którzy polegają na swojej pamięci wzrokowej i orientacji przestrzennej, aby lokalizować powtarzające się treści.   

Wyniki tego testu pozwalają ustalić, czy spełnione jest kryterium sukcesu 3.2.3 Spójna nawigacja.
 
Elementy nawigacyjne to wszelkie komponenty, które pomagają użytkownikm lokalizować konkretne informacje lub funkcje na witrynie. Może to być szeroka gama komponentów stosowanych na witrynach i dowolny powtarzalny element na stronie, zarówno elementy interaktywne, jak i nieinteraktywne. Grupowanie elementów również jest &bdquo;komponentem&rdquo; nawigacyjnym. Elementami nawigacyjnymi są między innymi:  

-	Interaktywne elementy, takie jak łącza nawigacyjne, menu, karty, pola wyszukiwania i ikony hiperłączy.

-	Elementy zgrupowane / lokalizacyjne: menu nawigacyjne zawsze po prawej stronie, sekcja reklamowa zawsze po prawej stronie, powtarzający się nagłówek / stopka.

-	Elementy nieinteraktywne: logo zawsze w lewym górnym rogu strony, nagłówek treści strony konsekwentnie umieszczony.


### Metody i narzędzia testowe
1.	Inspekcja wzrokowa.
2.	ANDI: struktury - włączony „porządek odczytu” .


### Identyfikacja treści

Zidentyfikuj wszystkie elementy nawigacyjne, które są powtarzane na innych stronach w witrynie.

**Uwaga:** Elementy nawigacyjne to wszelkie komponenty, które umożliwiają użytkownikowi zlokalizowanie określonych informacji lub funkcji w witrynie. Mogą to być elementy interaktywne lub nieinteraktywne, a grupowanie komponentów może również spełniać tę definicję.

Elementy nawigacyjne nie muszą być dokładnie takie same, aby można je było uznać za powtarzalne; elementy nawigacyjne można uznać za powtarzające się, jeśli zawierają ten sam rodzaj informacji i / lub służą temu samemu celowi. 


### Zastosowanie
Test 9B: 3.2.3-spojna-nawigacja **nie ma zastosowania** na stronach, na których nie ma bloków treści powtarzających się na innych stronach. Jeśli zakresem testowania jest tylko jedna strona internetowa,  która nie jest częścią większej witryny, ten test **nie ma zastosowania**.

### Jak testować

1.  Przejrzyj wiele stron internetowych witryny, aby zidentyfikować komponenty nawigacyjne powtarzające się na wielu stronach. Nie inicjuj zmian treści.

2.  Przejrzyj kolejność elementów nawigacyjnych i porównaj je z kolejnością na innych stronach, na których się pojawiają

    1.  **Uwaga**: Funkcja „porządek tabulacji” w ANDI w module elementy interaktywne, może pomóc w ocenie kolejności, w jakiej elementy pojawiają się na stronie w stosunku do innych treści. Funkcja „kolejność odczytu” również może pomóc w ocenie kolejności komponentów, zarówno interaktywnych, jak i nieinteraktywnych.
	
### Ocena wyników

Jeśli poniższe stwierdzenie jest prawdziwe, treść (strona) **spełnia** wymóg testowy, jest **zgodna** z KS 3.2.3

1. Każdy powtarzany komponent występuje w tej samej względnej kolejności w odniesieniu do innych powtarzanych komponentów na każdej stronie internetowej, na której się pojawia.


Reasumując: ta sama kolejność względna jest zdefiniowana jako ta sama pozycja względem: (1) miejsca położenia na stronie w porównaniu z innymi stronami i (2) do kolejności samych elementów nawigacyjnych.


### Uwaga

- *Ta sama kolejność względna* jest zdefiniowana jako ta sama pozycja w stosunku do pozycji innych elementów. Elementy uznaje się za znajdujące się w tej samej względnej kolejności, nawet jeśli inne elementy zostaną wstawione lub usunięte z pierwotnej kolejności. Na przykład w rozwijanym menu nawigacyjnym może być wstawiony dodatkowy poziom szczegółowości lub do porządku odczytu można wstawić dodatkową sekcję nawigacyjną.

## Spójna identyfikacja

### Test 9C 3.2.4-spojna-identyfikacja

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 3.2.4-spojna-identyfikacja | 9.C     | Dostępne nazwy i opisy komponentów wykonujących tę samą funkcję są spójne (takie same). |


### Cel testu 9C 3.2.4-spojna-identyfikacja

Celem tego testu jest sprawdzenie, czy oznaczenia służące identyfikacji komponentów, które pełnią na stronach tę samą funkcję, jest spójna. Spójna identyfikacja powtarzalnych komponenttów strony sprawia, że korzystanie ze strony jest prostsze i łatwiejsze dla wszystkich. Wspomaga szczególnie osoby z ograniczeniami wzroku i ograniczeniammi funkcji poznawczych. Strategia, z której korzystają osoby korzystające z czytników ekranu podczas przeglądania witryn, polega w dużej mierze na znajomości funkcji, które mogą pojawiać się na różnych stronach. Jeśli identyczne funkcje mają różne nazwy czy etykiety na różnych stronach, korzystanie z witryny jest znacznie trudniejsze. Może to również być mylące i zwiększać obciążenie poznawcze u osób z ograniczeniami poznawczymi.

Wymóg spójności rozciąga się także na alternatywy tekstowe. Jeśli ikony lub inne nietekstowe elementy mają tę samą funkcjonalność, ich alternatywy tekstowe również powinny być spójne.

Dzięki spójnej identyfikacji użytkownicy mogą zastosować swoją wiedzę na temat korzystania z jednej strony na innych stronach witryny, gdy używane są te same komponenty. 

Wyniki tego testu pozwalają ustalić, czy spełnione jest kryterium sukcesu 3.2.4 Spójna identyfikacja.


### Metody i narzędzia testowe
1.	Inspekcja wzrokowa.
2.	ANDI: interaktywne.

### Identyfikacja treści

Zidentyfikuj komponenty, które w zestawie stron internetowych mają tę samą funkcjonalność.

Ta sama funkcjonalność oznacza, że komponenty dają ten sam wynik. Ważne jest, aby zrozumieć, że ten test dotyczy **tylko funkcjonalności**; nie wymaga, aby na przykłąd za każdym razem ten sam obraz miał takie same Wyjście ANDI.

**Uwaga**: Myślenie o identyfikacji treści może być po prostu wyszukaniem wszystkich elementów, które mają tę samą funkcjonalność (wygląd związany z tym elementem nie jest czynnikiem decydującym). Znak „X” może działać jako przycisk usuwania LUB oznaczać, że element został odrzucony. Jeśli ta sama grafika służy wielu funkcjom, może posiadać różne alternatywy tekstowe.  

### Zastosowanie
 
Test 9C: 3.2.4-spojna-identyfikacja **nie ma zastosowania** w przypadkach:

- gdy na stronie nie ma komponentów, które mają taką samą funkcjonalność, jak na innych stronach w zestawie stron internetowych

- gdy tylko jedna strona internetowa, która nie jest częścią większej witryny,

- gdy komponenty pojawiają się tylko na jednej stronie, ale nie na innych stronach. 

**Uwaga**: Ten test ma zastosowanie tylko do tych komponentów, które mają taką samą funkcjonalność w ramach zestawu stron internetowych. Nie dotyczy komponentów, które pojawiają się tylko w obrębie jednej strony i nie pojawiają się na innych stronach. 

### Jak testować

1.  Uruchom ANDI: moduł interakktywne.

2.  Sprawdź Wyjście ANDI dla każdego zidentyfikowanego elementu.


### Ocena wyników

Jeśli poniższe stwierdzenie jest prawdziwe, treść (strona) **SPEŁNIA** wymóg testowy, jest **ZGODNA** z KS 3.2.4:

1.	Komponenty o identycznej funkcjonalności są identyfikowane konsekwentnie.


### Uwaga

-  Spójne alternatywy tekstowe dla elementów interfejsu wykonujących tę samą funkcję nie zawsze są  „identyczne”. Jest to dopuszczalne, jeśli mają one spójny format. Na przykład w przypadku użycia strzałki graficznej na dole strony internetowej, która łączy z następną stroną, alternatywą tekstową może być: „Przejdź do strony 4.” Jednak ten sam obraz strzałki na następnej stronie powinien zawierać informację „Przejdź do strony 5.”
-  Pojedynczy element nietekstowy może służyć do pełnienia różnych funkcji. W takich przypadkach konieczne są różne alternatywy tekstowe i należy je stosować. Przykładami mogą być często spotykane ikony, takie jak fiszki, krzyżyki czy znaki drogowe. Ich funkcje mogą się różnić w zależności od kontekstu strony internetowej. Ikona fiszki (haczyk) może oznaczać „zatwierdzono”, „wypełniono” lub „dołączono”, aby wymienić tylko kilka przypadków. Użycie jako alternatywy tekstowej na wszystkich stronach internetowych jednakowego tekstu typu  „znacznik wyboru” nie pomaga użytkownikom zrozumieć funkcji ikony. Zasadne jest zastosowanie różnych alternatyw tekstowych, gdy ta sama treść nietekstowa pełni wiele funkcji.


## Standardy dostępności

{% include ks/2-4-1.md %}

{% include ks/3-2-3.md %}

{% include ks/3-2-4.md %}

[4. Treść powtarzalna](ICT-04-tresc-powtarzalna)                                                                                                                                                                                                                  
