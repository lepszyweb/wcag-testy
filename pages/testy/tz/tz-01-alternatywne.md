---
title: 1. Zgodna wersja alternatywna i brak zakłóceń

sidebar: testy_sidebar
permalink: tz-01-alternatywne
folder: testy/tz
---

Warunki testowe wersji alternatywnych zapewniających zgodność różnią się nieznacznie od pozostałych testów na kilka ważnych sposobów:

- Najpierw przedstawiono warunki testowania wersji alternatywnych zapewniających zgodność, ponieważ identyfikacja dostępnych wersji alternatywnych zapewniających zgodność treści pomaga zdefiniować zakres testowania. Niezgodna treść, która ma wersję alternatywną zapewniającą zgodność, jest testowana pod kątem zakłóceń, a następnie jest wyłączana z testów po tym teście.

-   Mimo że zidentyfikowanie wersji alternatywnych zapewniających zgodność w celu zdefiniowania zakresu testu jest  ważne, nie będzie możliwe ustalenie, czy zapewniono wersję alternatywną zapewniającą zgodność, dopóki nie zakończą się wszystkie inne odpowiednie testy. (Wersja alternatywna zapewniająca zgodność nie może być uznana za taką, dopóki nie przejdzie wszystkich obowiązujących warunków testowych).


-   Wyniki testów dla  wersji alternatywnych zgodnych nie są odpowiadają wzorcowi **prawda=zgodna, nieprawda=niezgodna, nie ma zastosowania**, który jest przestrzegany przez pozostałe testy. Zapewnienie zgodnej alternatywnej wersji nie jest wymagane. Jest raczej akceptowalną metodą dostarczania tych samych informacji i/lub funkcjonalności w sposób dostępny, gdy istnieją inne niezgodne wersje wersje tych treści. Dlatego też status **niezgodna** nie jest odpowiednim wynikiem testu. Jeżeli warunek testowy ma wartość **prawda**, wynikiem testu jest **zgodna**. Jeżeli warunek testowy ma wartość **nieprawda**, alternatywna wersja zgodna nie istnieje, a wynikiem warunku testowego jest **nie ma zastosowania** (**ND**).


## Dostępność wersji alternatywnej

### Identyfikacja treści

Zidentyfikuj inne wersje tej samej treści, tj. treści, które zostały dostarczone na więcej niż jeden sposób, z wyraźnym lub dorozumianym zamiarem, aby jedna lub więcej z tych wersji była osiagana jako dostępna alternatywa.

1.  Zgodne wersje alternatywne mogą być zapewnione dla części strony, całych stron lub całej witryny.
2.  Na istnienie zgodnej wersji alternatywnej mogą wskazywać różne mechanizmy, w tym:

    -   Instrukcje opisujące, jak włączyć dostępność
    -   Treść jest oznaczona jako zgodna wersja alternatywna (wersja dostępna)
    -   Istnieje kilka metod wykonania zadania (np. do wprowadzenia daty służą widżet kalendarza i pole tekstowe)
    -   Miejsce docelowym łącza jest zgodna wersja alternatywna lub wersja dla technologii wspomagających (np. wersja dla czytnika ekranu)
    -   Istnieją preferencje lub ustawienia użytkownika, umożliwiające włączenie ułatwień dostępu
    -   Istnieją elementy sterujące (narzędzia) użytkownika do modyfikowania kolorów i wyglądu tekstu.

3.  Zgodne wersje alternatywne nie muszą się znajdować się w „zakresie zgodności” (zbiorze stron, których dotyczy oświadczenie o zgodności), ani nawet w tej samej witrynie internetowej, o ile są równie łatwo osiągalne, jak wersja niezgodna. W przypadku tej procedury testowej zakres testów jest ograniczony tylko do zgodnych wersji alternatywnych, które są osiągalne na komputerach stacjonarnych. Zgodne wersje alternatywne nie obejmują aplikacji mobilnych, do których dostęp można uzyskać tylko na urządzeniu przenośnym.

Jeśli istnieje tylko jedna wersja treści, czyli jeśli nie istnieją wersje alternatywne, wynikiem testu oznaczonych identyfikatorami od 1.A do 1.E jest: **NIE MA ZASTOSOWANIA**.


#### Test 1.A zgodna-wersja-alternatywna

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|---------------------------------------|
| zgodna-wersja-alternatywna | 1.A | Wersja alternatywna zapewniająca zgodność spełnia wszystkie wymagania testowe objęte tą procedurą testową. |

#### Zastosowanie:

Test 1.A zgodna-wersja-alternatywna **nie ma zastosowania**, jeśli istnieje tylko jedna wersja treści.

#### Jak testować:

1.  Włącz dostępność za pomocą ustawień witryny, jeśli istnieją.

2.  Jeśli jedna z wersji została wskazana jako wersja dla celów dostępności, przyjmij, że jest to wersja alternatywna i w tym teście (id 1.A) podaj wyniki testów tylko dla tej wersji.

3.  Po zakończeniu procesu testowania przetestuj zidentyfikowaną wersję „dostępną” pod kątem  wszystkich obowiązujących warunków testowych.

    1.  Może być konieczne przeprowadzenie szeroko zakrojonego badania, zanim zostanie znaleziony wynik dla danego warunku testu. Jeśli ustawienia użytkownika umożliwiają dostęp do całej witryny, cała witryna jest wersją alternatywną i cała witryna musi przejść wszystkie warunki testowe.

    2.  Jeśli w zidentyfikowanej „dostępnej” wersji zostanie stwierdzony defekt, wprowadź **niezdany** dla odpowiedniego ID testu. Nie jest konieczne kontynuowanie testów dla tego testu (ID 1.A) po znalezieniu błędu. Oceń wyniki.

    3.  Jeśli żadna z wersji nie została zidentyfikowana jako „dostępna”, należy przetestować wszystkie wersje, dopóki nie zostanie znaleziona wersja, która spełnia wszystkie obowiązujące warunki testowe.

        1.  Jeśli w danej wersji zostanie stwierdzone niepowodzenie, należy przerwać testowanie tej wersji i przetestować inne wersje.

#### Wyniki oceny

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, , to treść **PRZESZŁA** test; jeśli poniższe twierdzenie jest **FAŁSZYWE**, to ten warunek testowy **NIE MA ZASTOSOWANIA**:

1.	Dostępna jest alternatywna wersja treści, która spełnia wszystkie obowiązujące warunki testowe w tej procedurze testowej.

Jeżeli wynikiem tego warunku testu jest:

-   **ZDANY**, przejdź do (kontynuuj test) 1.B. Dostępna wersja alternatywna (która przeszła ten test 1.A.) będzie określana jako „dostępna wersja” w kolejnych testach.

-   **NIE MA ZASTOSOWANIA**, zaznacz wyniki dla pozostałych warunków testowych zgodnej wersji alternatywnej (1.B - 1.E) jako **NIE MA ZASTOSOWANIA** i kontynuuj testowanie wszystkich wersji z kolejnymi warunkami testowymi. Wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z testu.

##### Uwaga:

-   Zgodne wersje alternatywne mogą być zapewniane dla różnych technologii lub grup użytkowników. Co najmniej jedna wersja musi przejść wszystkie warunki testowe (przejsć pomyślnie wszystkie testy).

-   Pomocne może być przejrzenie dokumentacji produktu w celu uzyskania informacji o wersjach zapewniających zgodność lub włączeniu ułatwień dostępu.

-   Chociaż badanie warunków testowych dla wersji alternatywnej może zostać wstrzymane, gdy zidentyfikowana wersja „dostępna” nie spełnia warunków testowych, konieczne może być dalsze testowanie wersji, aby ukończyć pozostałe testy w tej procedurze testowej. Jeżeli nie ma zgodnej wersji alternatywnej, wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z badania.

#### Test 1.B rownowaznosc-wersji-alternatywnej

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| rownowaznosc-wersji-alternatywnej | 1.B | Zgodna wersja alternatywna zawiera równoważne (takie same) informacje i funkcjonalności.|

#### Zastosowanie:

Test 1.B rownowaznosc-wersji-alternatywnej **nie ma zastosowania**, jeśli istnieje tylko jedna wersja treści (czyli jeśli test 1.A **nie ma zastosowania**).

#### Jak testować:

1.  Kontynuuj test 1.A.

2.  Przejrzyj treść wersji niezgodnej.

3.	Porównaj zgodną wersję alternatywną (która przeszła test 1.A) z wersją niezgodną pod względem równoważności treści (tj. równoważnych informacji i funkcjonalności).


#### Wyniki oceny

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, to treść **PRZESZŁA** test; jeśli poniższe twierdzenie jest **FAŁSZYWE**, to ten warunek testowy **NIE MA ZASTOSOWANIA**:


1.	Zgodna wersja alternatywna (która przeszła test 1.A) zawiera wszystkie te same informacje i funkcjonalności, co treść niezgodna i przedstawione w tym samym języku ludzkim.

Jeżeli wynikiem tego warunku testu jest:

-   **ZDANY**, przejdź do testu 1.C.

-   **NIE MA ZASTOSOWANIA,** oznacz 1.C - 1.E jako **NIE MA ZASTOSOWANIA** i kontynuuj testowanie wszystkich wersji z następnymi warunkami testowymi. Wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z testu.

##### Uwaga:

-   Zgodna wersja alternatywna nie musi być dopasowana „jeden do jednego” do niezgodnej (np. zgodna wersja alternatywna może składać się z większej lub mniejszej liczby stron).

-   Chociaż badanie warunków testowych dla wersji alternatywnej może zostać wstrzymane, gdy zidentyfikowana wersja „dostępna” nie spełnia warunków testowych, konieczne może być dalsze testowanie wersji, aby ukończyć pozostałe testy w tej procedurze testowej. Jeżeli nie ma zgodnej wersji alternatywnej, wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z badania.


### Dostęp do zgodnej wersji alternatywnej

#### Identyfikacja treści

Strona z niezgodną wersją treści, na której istnieje mechanizm, metoda lub ścieżkę dostępu do dostępnej równoważnej wersji treści (która przeszła test 1.B).

Do osiągnięcia zgodnej wersji alternatywnej można zastosować różne metody, w tym:
-   łącze do zgodnej wersji alternatywnej lub wersji przeznaczonej dla technologii wspomagającej (np. wersji dla czytnika ekranu)
-   preferencje lub ustawienia użytkownika umożliwiające dostęp do strony lub całej witryny ze zgodną wersją alternatywną
-   Przełączniki (narzędzia użytkownika) służące do modyfikowania kolorów i wyglądu tekstu strony lub całej witryny
-   Wersja alternatywna zapewniająca zgodność znajduje się na tej samej stronie, co wersja niezgodna.

Jeśli wynikiem testu 1.A lub 1.B jest **NIE MA ZASTOSOWANIA**, to wynikiem testów od 1.C do 1.E jest również **NIE MA ZASTOSOWANIA**.


**Uwaga**: Tylko JEDNA metoda może być użyta do zaoferowania uzytkownikowi zgodnej wersji alternatywnej.

**ALBO** 
-   użytkownik najpierw napotyka treść  niezgodną i musi nawigować do zgodnej wersji alternatywnej wersji (przetestowanej w 1.C) 

**ALBO**

-   wersja niezgodna NIE jest oferowana użytkownikowi najpierw (wówczas przejdź do testu 1.D).

> ALBO test 1.C, jak, ALBO test 1.D musi być ZDANY; nie można zastosować obu równocześnie do tej samej zgodnej wersji alternatywnej (dostępnej i równoważnej).

#### Test 1.C dostep-do-wersji-alternatywnej

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| dostep-do-wersji-alternatywnej | 1.C |  Istnieje mechanizm umożliwiający osiągnięcie zgodnej wersji alternatywnej ze strony niezgodnej.|

#### Zastosowanie:

Test 1.C dostep-do-wersji-alternatywnej **nie ma zastosowania**, jeśli  
- istnieje tylko jedna wersja treści albo 
- test z identyfikatorem 1.A lub 1.B został oceniony jako **NIE MA ZASTOSOWANIA**, albo 
- jeśli użytkownikowi nie została zaoferowana najpierw wersja niezgodna (przejdź do testu 1.D).


#### Jak testować:

1.  Kontynuuj test 1.B.

2.  Zidentyfikuj mechanizm używany do osiągnięcia zgodnej wersji alternatywnej (dostępnej równoważnej, która przeszła test 1.B).

    1.  W razie potrzeby wróć na stronę, na której znajduje się mechanizm umożliwiający wybranie lub włączenie zgodnej wersji alternatywnej.

    2.  Może to być łącze lub funkcja na stronie niezgodnej

    3.  Mogą to być ustawienia użytkownika lub preferencje.

3.  Po zakończeniu tej procedury testowej przetestuj mechanizm pod kątem wszystkich obowiązujących warunków testowych.

#### Wyniki oceny

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, , to treść **PRZESZŁA** test; jeśli poniższe twierdzenie jest **FAŁSZYWE**, to ten warunek testowy **NIE MA ZASTOSOWANIA**:

1.  Mechanizm zastosowany w celu osiągnięcia zzzgodnej wersji alternatywnej (dostępnej równoważnej) spełnia wszystkie obowiązujące warunki testu.

Jeden z warunków testowych - 1.C ALBO 1.D musi być **ZDANY** dla istniejącej zgodnej wersji alternatywnej. Jeżeli wynikiem testu 1.C jest:

-   **ZDANY**, oznacz test 1.D jako **NIE MA ZASTOSOWANIA**, kontynuuj testowanie 1.E.

<!-- -->

-   **NIE MA ZASTOSOWANIA**, gdy:

    -   warunek testowy nie miał zastosowania (bo wersja niezgodna nie była pierwszą oferowaną użytkownikom), kontynuuj testowanie 1.D.

    -   na stronie z wersją niezgodną nie istnieje mechanizm, który umożliwia osiągnięcie zgodnej wersji alternatywnej, oznacz testy 1.D oraz 1.E jako **NIE MA ZASTOSOWANIA** i kontynuuj testowanie wszystkich wersji z następnymi warunkami testowymi.

##### Uwaga:

-   Odpowiednie testy mechanizmów mogą obejmować linki i przyciski, nagłówki, formularze i / lub inne testy.

-   Mechanizm dostępu do zgodnej wersji alternatywnej powinien bezpośrednio lub pośrednio wskazywać, że prowadzi do wersji dostępnej. Na przykład tekst poprzedzający tekst łącza do wersji zgodnej może wprost wskazywać, że łącze prowadzi do zgoodnej wersji alternatywnej. Możliwe jest również „ukrywanie” treści niezgodnych z AT i/lub wykluczenie ich z porzadku tabulacji, ograniczając w ten sposób dostęp tylko do wersji zapewniajacych dostępność dla użytkowników z  niepełnosprawnościami. Takie podejście może jednak nie być możliwe, w zależności od treści.

-   Mechanizm może być wyraźnie podany w treści lub może być oparty na zapewnieniu przez platformę lub przez użytkownika, w tym technologie wspomagające.

-   Mechanizm musi spełniać wszystkie kryteria sukcesu dla deklarowanego poziomu zgodności.

### Identyfikacja treści

Zidentyfikuj wszystkie mechanizmy, metody i ścieżki dostępu do niezgodnych wersji treści.

Jeśli wynikiem dla testu 1.A lub dla testu 1.B było **NIE MA ZASTOSOWANIA**, wówczas wynik dla testów od 1.C do 1.E również **NIE MA ZASTOSOWANIA**.  Jeśli wynikiem dla testu 1.C jest **ZDANY**, wówczas wynikiem testu 1.D jest **NIE MA ZASTOSOWANIA**.

### Dostep do wersji niezgodnej

#### Test 1.D dostep-do-wersji-niezgodnej

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| dostep-do-wersji-niezgodnej | 1.D | Dostęp do wersji niezgodnej można uzyskać tylko z wersji zgodnej. |

#### Zastosowanie:
Test 1.D dostep-do-wersji-niezgodnej **nie ma zastosowania**, jeśli 

-   jest tylko jedna wersja treści, LUB

-   Test 1.A lub test 1.B oceniono jako **nie ma zastosowania**, LUB

-   Test 1.C oceniono jako **ZDANY**.

#### Jak testować:

1.  Ustal, w jaki sposób można uzyskać dostęp do niezgodnej wersji treści.

    1.  Do wersji niezgodnej można uzyskać dostęp tylko ze zgodnej wersji alternatywnej.

    2.  Zarówno dostęp do zgodnej wersji alternatywnej, jak i dostęp do wersji niezgodnej można uzyskać z innej strony.

        1.  Czy strona zapewniająca dostęp jest zgodna ze wszystkimi mającymi zastosowanie procedurami testowymi?

        2.  Czy istnieje inny sposób uzyskania dostępu do wersji niezgodnej?

#### Wyniki oceny
Jeśli którekolwiek z poniższych stwierdzeń jest **PRAWDZIWE**, to treść **ZDAŁA** test; jeśli wszystkie twierdzenie są **FAŁSZYWE**, to ten warunek testowy **NIE MA ZASTOSOWANIA**:

1.  Wersję niezgodną można osiągnąć tylko ze zgodnej wersji alternatywnej (która przeszła test 1.B), **ALBO**

2.  Wersja niezgodna jest dostępna tylko ze strony, która:

    1.  spełnia wszystkie pozostałe warunki testowe **ORAZ**

    2.  zapewnia również mechanizm umożliwiający osiągnięcie zgodnej wersji alternatywnej (która przeszła test 1.A oraz test 1.B).

Albo wynikiem testu 1.C, ALBO wynikiem testu 1.D musi być **ZGODNY**, aby istniała zgodna wersja alternatywna. Jeżeli wynikiem tego warunku testowego jest

-   **ZGODNY**, kontynuuj testowanie 1.E.

-   **NIE MA ZASTOSOWANIA** ORAZ zaznaczyłeś 1.C jako **ZGODNY**, kontynuuj testowanie 1.E.

-   **NIE MA ZASTOSOWANIA** ORAZ zaznaczyłeś 1.C jako **NIE MA ZASTOSOWANIA,** oznacz 1.E jako **NIE MA ZASTOSOWANIA** i kontynuuj testowanie wszystkich wersji z następnymi warunkami testowymi.

##### Uwaga:

-   Aby ocena wyników kroku 2 powyżej była **PRAWDA**, zarówno strona, jak i mechanizm muszą przejść wszystkie obowiązujące warunki testu. Po zakończeniu procesu testowania przetestuj stronę i mechanizm pod kątem wszystkich odpowiednich warunków testowych.

### Brak zakłóceń

### Identyfikacja treści

Niezgodne wersje treści, które mają alternatywną wersję zgodną.

Jeśli wynikami testów zarówno dla 1.C jak i 1.D są **NIE MAJĄ ZASTOSOWANIA**,  to wynikiem dla testu 1.E jest również **NIE MA ZASTOSOWANIA**.

#### Test bez-zaklocen

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| bez-zaklocen | 1.E     | Treści w wersjach niezgodnych spełniają wymóg zgodności 5. |

#### Zastosowanie:
Test 1.E bez-zaklocen **nie ma zastosowania**, jeżeli:

-  jest tylko jedna wersja treści, **lub**

-  Testy 1.C i 1.D oceniono jako  **nie ma zastosowania**.

#### Jak testować:

1.  Niezgodna treść, która ma zgodną alternatywną wersję, musi zostać przetestowana przed pominięciem treści z pozostałej części testowania.

2.  Jeśli to konieczne i / lub dotyczy, wyłącz funkcje ułatwień dostępu w ustawieniach witryny lub preferencjach.

3.  Po zakończeniu tego procesu testowego WYKONAJ TYLKO następujące testy niezgodnej wersji treści:

    1.  test 2.A (1.4.2-sterowanie-dzwiekiem) Test 2.A (Sterowanie dźwiękiem 1.4.2)

    2.  test 2.B (2.2.2-migajace-ruchome-przewijane) Test 2.B (2.2.2-miganie-ruch-przewijanie)

    3.  test 2.C (2.2.2-automatyczna-aktualizacja) Test 2.C (Automatyczna aktualizacja 2.2.2)

    4.  test 3.A (2.3.1-błyskanie) Test 3.A (błyskanie 2.3.1)

    5.  test 4.C (2.1.2-bez-pulapki-na-klawiature) Test 4.C (2.1.2-bez pułapki na klawiaturę)

4.  Oznacz odpowiedni identyfikator testu, jeżeli którykolwiek z powyższych testów daje wynik **NIEZDANY** lub **NIE MA ZASTOSOWANIA** (dla testu 3.A).

#### Wyniki oceny

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, to treść **PRZESZŁA** test; jeśli poniższe twierdzenie jest **FAŁSZYWE**, to ten warunek testowy **NIE MA ZASTOSOWANIA**:

1.  Wyniki dla każdego z poniższych testów to ZDANY lub NIE MA ZASTOSOWANIA w przypadku niezgodnych wersji treści.

    1.  Test 2.A (1.4.2-sterowanie-dzwiekiem)

    2.  Test 2.B (2.2.2-migajace-ruchome-przewijane)

    3.  Test 2.C (2.2.2-automatyczna-aktualizacja)

    4.  Test 3.A (2.3.1-błyskanie)

    5.  Test 4.C (2.1.2-bez-pulapki-na-klawiature)

**Uwaga:** Po wykonaniu tego testu na niezgodnej wersji treści, która ma zgodną wersję alternatywną, pomiń testowanie niezgodnej treści w pozostałej części testowania.

### Zastosowane standardy

[Wersja alternatywna zapewniająca zgodność](http://www.fdc.org.pl/wcag2/index.html#conforming-alternate-versiondef) nie jest wymogiem. Wymóg zgodności \#1 pozwala na włączenie do zakresu zgodności stron niezgodnych z wymaganiami, o ile mają one „zgodną wersję alternatywną”. Gwarantuje to, że wszystkie informacje i wszystkie funkcje, które znajdują się na stronach objętych zakresem zgodności, są dostępne na stronach internetowych zgodnych z wymogami.

[20. Zgodność z wersją alternatywną](ICT-20-wersje-alternatywne)

[Wymóg zgodności WCAG 5. Brak zakłóceń](https://www.w3.org/TR/WCAG20/#conformance-reqs): Poniższe kryteria sukcesu dotyczą całej treści na stronie, włącznie z treścią, która w innych przypadkach nie jest podstawą spełnienia wymogów zgodności, gdyż niezastosowanie poniższych kryteriów mogłoby uniemożliwić jakiekolwiek skorzystanie ze strony:
- 1.4.2 Kontrola odtwarzania dźwięku
- 2.1.2 - Brak pułapki na klawiaturę,
- 2.3.1 - Trzy błyski lub wartości poniżej progu, oraz
- 2.2.2 - Wstrzymywanie (pauza), zatrzymywanie, ukrywanie.

[25. Brak zakłóceń](ICT-25-brak-zaklocen)