---
title: 15. Treść wstawiana i pozycjonowana za pomocą CSS


sidebar: testy_sidebar
permalink: tz-15-css
folder: testy/tz
---

## Cel scenariusza testowego
Celem tego scenariusza testowego jest sprawdzenie, czy treść, kolejność czytania i znaczenie są nadal zachowywane, jeśli treść wstawiona lub pozycjonowana za pomocą CSS nie będzie widoczna.

Treść wprowadzana za pomocą CSS może być niewidoczna dla niektórych czytników ekranu, więc istotne informacje muszą być prezentowane w równoważny sposób, aby zachować porządek i znaczenie dla użytkowników niewidomych i słabowidzących.


Scenariusz „Treść wstawiana i pozycjonowana za pomocą CSS” obejmuje dwa testy:

W tym temacie są dwie lekcje:
1.	Test 15A 1.3.1-tresci-dodane-przez-css
2.	Test 15.B 1.3.2-zrozumiala-kolejnosc-tresci

## Treść dodana przez CSS 

### Test 15A 1.3.1-tresci-dodane-przez-css

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.1-tresci-dodane-przez-css | 15.A    | Znaczące treści dodane wyłącznie przez CSS są dostępne także w inny sposób. |

### Cel testu 15A 1.3.1-tresci-dodane-przez-css
Celem tego testu jest sprawdzenie, czy znacząca treść wstawiona przy użyciu pseudoelementów CSS ::before i ::after jest również dostępna w inny sposób. Niektóre technologie wspomagające  ignorują CSS. W takich przypadkach użytkownicy mogą nie mieć dostępu do informacji wstawionych za pomocą CSS, chyba że zostaną one również przedstawione na stronie w inny sposób. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-3-1 Informacje i relacje](https://https://wcag.lepszyweb.pl/#info-and-relationships).

### Metody i narzędzia testowe 

1.	ANDI: ukryta treść > content ::before ::after.
2.	Inspekcja wzrokowa treści strony.


### Identyfikacja treści
Wszystkie znaczące treści na stronie dodane za pomocą pseudoelementów CSS ::before i ::after.

Użyj ANDI, aby wykryć wszystkie znaczące treści strony wstawione za pomocą reguł CSS  `content::before` lub `content::after`. Uwzględnij style wbudowane (dodane śródliniowo).

1.	Uruchom ANDI: ukryta treść.
2.  Ustal, czy opcja content ::before ::after jest pokazana.

<!-- -->

1.  Jeśli nie wstawiono żadnej zawartości strony przy użyciu :: przed lub :: po, ANDI nie wyświetli tej opcji.


### Zastosowanie
Test 15A 1.3.1-tresci-dodane-przez-css **nie ma zastosowania**, jeśli na stronie nie ma żadnych znaczących treści wstawionych za pomocą pseudoelementów ::before lub ::after. W takim przypadku oznacz wynik testu jako **ND**. 

**Uwaga**: Treść wstawiona za pomocą ::before lub ::after jest uważana za znaczącą, jeśli po jej ukryciu ta treść znika (np. obrazy, tekst, niestandardowe ikony czcionek) lub znika ważny kontekst dla treści sąsiadujących.

### Jak testować

1.  Launch ANDI: hidden content and select content ::before ::after to reveal all content.Uruchom ANDI: ukryta treść i wybierz prrzycisk content::before ::after, aby wykryć treści wstawione za pomocą CSS.
    1.  Treści wstawione przy użyciu `::before` lub `::after` zostaną oznaczone na czerwono.
	
	**Uwaga**: ANDI pokazuje elementy tylko za pomocą koloru podświetlenia na ekranie; w ANDI nie ma innych danych wyjściowych.

2.  Przejrzyj całą treść wstawioną za pomocą ::before oraz :after i znajdź całą znaczącą treść.

    1.  Jeśli nie ma znaczącej treści, oznacz test 15.A jako **nie ma zastosowania** (**ND**).

    2.  Jeśli istnieje znacząca treść, przejdź do następnego kroku.

3.  Przejrzyj stronę internetową i ustal, czy dla każdego wystąpienia treści CSS dodanej za pomocą ::before lub ::after informacje są przekazywane w inny sposób.

**Uwaga**: Jeśli pseudoelementy CSS :::before i ::after są używane do wstawiania treści znaczących, treść ta musi być również obecna w innym miejscu strony, aby wszyscy użytkownicy czytników ekranu mieli dostęp do tych samych informacji.


### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.3.1:

1.  Wszystkie znaczące treści wstawione przy użyciu `::before` i `::after` mają równoważne informacje przedstawione w inny sposób.

## Pozycjonowanie CSS 

### Test 15.B 1.3.2-zrozumiala-kolejnosc-tresci

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.2-zrozumiala-kolejnosc-tresci | 15.B    | Kolejność odczytywania treści po wyłączeniu arkuszy stylów CSS jest sensowna oraz zachowane jest znaczenie treści (w kontekście). |

Celem tego testu jest sprawdzenie, po wyłączeniu arkuszy stylów CSS kolejność odczytywania treści jest prawidłowa, a znaczenie treści jest zachowane. Kaskadowe arkusze stylów umożliwiają projektantom takie pozycjonowanie elementów strony, że ich porządek, w jakim są wyświetlane na ekranie może być inny niż kolejność elementów w kodzie źródłowym. Natomiast technologie wspomagające, z których korzystają użytkownicy z niepełnosprawnościami prezentują treści w takiej kolejności, w jakiej pojawiają się one w kodzie źródłowym. Kolejność wyświetlania elementów na stronie może być inna niż kolejność w kodzie źródłowym pod warunkiem, że kolejność, w jakiej treści będą odczytywane przez technologie wspomagające będzie logiczna i zrozumiała dla użytkowników oraz nie zmieni znaczenia treści na stronie. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-3-1 Informacje i relacje](https://https://wcag.lepszyweb.pl/#info-and-relationships).

### Metody i narzędzia testowe  
1.	ANDI: Opcje rozszerzone > Linearyzuj stronę (pole wyboru).
2.	Inspekcja wzrokowa.


### Identyfikacja treści
Wszystkie znaczące treści na stronie pozycjonowane za pomocą reguł CSS (w tym wbudowanych).

Użyj ANDI, aby wykryć treści pozycjonowane za pomocą CSS i stylów wbudowanych.

1.	Uruchom ANDI, wybierz kolejno przycisk Opcje rozszerzone, a następnie Linearyzuj stronę, aby usunąć pozycjonowanie CSS z elementów na stronie.

2.  Treść pozycjonowana za pomocą CSS zostanie wyrożniona niebieskim podświetleniem wokół elementów, a elementy te zostaną umieszczone na stronie w tej samej kolejności, w jakiej występują w kodzie źródłowym strony, tj. bez zastosowania pozycjonowania CSS.

### Zastosowanie
Test 15.B 1.3.2-zrozumiala-kolejnosc-tresci **nie ma zastosowania**, jeśli na stronie nie ma treści pozycjonowanych za pomocą CSS (treści, które mają inną kolejność w kodzie źródłowym, niż wynikałaby z układu widocznego na stronie. W takim przypadku oznacz wynik testu jako **ND**.


### Jak testować

1.  Przejrzyj wszystkie wyróżnione, zlinearyzowane treści.
    ANDI oznacza treść pozycjonowaną za pomocą CSS niebieskimi konturami.

2.  Ustal, czy kolejność czytania treści jest nadal zrozumiała po linearyzacji. W razie potrzeby przełącz przycisk linearyzacji, aby wyświetlić pierwotne położenie treści.

**Uwaga**: Kolejność odczytu treści po jej zlinearyzowaniu nie musi być dokładnie taka sama jak przed linearyzacją. Tester powinien sprawdzić, czy kolejność czytania treści jest nadal logiczna i zrozumiała (np. słowa i akapity są prezentowane w kolejności, która nie zmienia znaczenia treści). W wielu przypadkach zmiany pozycji nie wpływają na znaczenie treści. Na przykład zmiana kolejności obszaru treści głównej i obszaru z menu nawigacyjnym nie wpływa na ich znaczenie.

### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.3.2:

1.	Kolejność i znaczenie treści (w kontekście) są zrozumiałe bez pozycjonowania CSS.

### Uwaga

Do rozpoznania kolejności odczytu przed linearyzacją treści można również wykorzystać opcję ANDI: struktury i łącze „porządek odczytu”. Ale włączenie tej opcji nie wyróżnia treści, której położenie na stronie zostało ustalone za pomocą CSS.


## Obowiązujące normy

- {% include ks/1-3-1.md %}
- {% include ks/1-3-2.md %}

- [18. Właściwości zmysłowe](ICT-18-zaleznosc-od-css)
