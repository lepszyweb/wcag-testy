---
title: 1. Zgodna wersja alternatywna i brak zakłóceń

sidebar: testy_sidebar
permalink: tz-01-alternatywne
folder: testy/tz
---


{% include note.html content="Praca nad tłumaczeniem trwa. To jest zgrubna, robocza wersja tłumaczenia." %}


## Cel zestawu testów

Testy z tego zestawu służą ocenie wersji alternatywnych zapewniających zgodność oraz spełniania wymogu [Brak zakłóceń](wcag21#525-brak-zakłóceń), gdy na stronie wykorzystywane są technologie, które nie obsługują dostępności albo użyte są tak, że nie obsługują dostępności.


Treść może być udostępniana w wielu wersjach, pod warunkiem, że jedna z nich jest w pełni zgodna z wymogami dostępności na wybranym poziomie. Zapewnienie wersji alternatywnej zapewniającej zgodność nie jest wymagane przez WCAG. Jest to raczej dopuszczalna metoda zapewnienia tych samych treści i funkcjonalności w sposób spełniający normy dostępności, gdy istnieją inne niezgodne wersje tych treści, czyli wersje niespełniające norm dostępności.

Na stronie internetowej mogą być zastosowane technologie internetowe, które nie obsługują dostępności albo nie są obsługiwane przez dostępność, albo zostały użyte tak, że nie obsługują dostępności. W takich przypadkach można uznać, że spełnione są normy dostępności pod warunkiem, że technologie, które nie obsługują dostępności nie blokują użytkownikom dostępu do reszty strony.       


Gdy strona internetowa zawiera alternatywne wersje treści w celu spełnienia wymagań dostępności, dowiesz się, jak ocenić, czy podana wersja alternatywna jest rzeczywiście dostępna i równoważna. Dowiesz się również, jak oceniać, czy wersje spełniają wymagania WCAG dotyczące dostępu do alternatywnej treści, od wersji niezgodnej do wersji zgodnej i odwrotnie. Zanim alternatywną wersję można uznać za „zgodną wersję alternatywną”, należy ocenić:

Celem tej procedury jest sprawdzenie, czy alternatywna wersja zapewniająca zgodność jest rzeczywiście  dostępna i równoważna oraz zapewnienie alternatywnej wersji zapewniającej zgodność spełnia wymagania WCAG dotyczące dostępu do treści alternatywnej, dostępu z wersji zapewniającej zgodność do wersji niezgodnej i odwrotnie.  

Zanim wersja alternatywna zostanie uznana za „zgodną z wymogami wersji alternatywnej”, należy ocenić, co następuje:

- czy wersja alternatywna jest w pełni dostępna,
- czy wersja alternatywna zawiera równoważne informacje i funkcjonalności,
- czy wszyscy użytkownicy mogą uzyskać dostęp zarówno do wersji zapewniającej zgodność, jak i niespełniającej wymogów zgodności.

Ta procedura testowa różni się od innych procedur w tym procesie testowym. Wykonując audyt zgodności, musisz najpierw ustalić, czy istnieje alternatywna wersja treści zapewniająca zgodność, a następnie ustalić, czy spełnia ona wszystkie wymagania „zgodnej wersji alternatywnej”. 

Wynik tej oceny określa zakres audytu.

Jeśli istnieje wersja alternatywna zapewniająca zgodność, to ta wersja zastępuje w zakresie testowania wersję niezgodną, a wersja niezgodna nie jest uwzględniana w raporcie z audytu.

Innymi słowy, audytowi podlega wersja alternatywna zapewniająca zgodność, a nie wersja niezgodna, nawet jeśli wersja niezgodna jest „podstawową” wersją strony czy witryny.

Podobnie jak w przypadku innych procedur testowych podczas oceny wyników, ustala się, że treść **spełnia** wymagania zgodności, jeśli warunek testowy lub warunki testowe są **prawdą**. 

Wykonywanie niektórych testów w tej procedurze zależy od tego, czy wynik poprzedniego testu został oceniony jako **spełnia** wymagania zgodności bądź został oznaczony jako **nie ma zastosowania**. 

Kolejna różnica dotyczy zastosowania oceny **nie spełnia**. Ponieważ zapewnienie wersji alternatywnej zapewniającej zgodność nie jest wymagane, to w ocenie wyniku testów 1.A - 1.D wersji alternatywnej nie można zastosować oceny **nie spełnia** warunków testowych. Jeśli twierdzenie definiujące warunek testowych nie są **prawdziwe**, to w odniesieniu do wersji mającej zapewnić zgodność stosuje się ocenę **nie ma zastosowania**.

-   Wyniki testów dla  wersji alternatywnych zgodnych nie są odpowiadają wzorcowi **prawda=zgodna, nieprawda=niezgodna, nie ma zastosowania**, który jest przestrzegany przez pozostałe testy. Zapewnienie zgodnej alternatywnej wersji nie jest wymagane. Jest raczej akceptowalną metodą dostarczania tych samych informacji i/lub funkcjonalności w sposób dostępny, gdy istnieją inne niezgodne wersje tych treści. Dlatego też status **niezgodna** nie jest odpowiednim wynikiem testu. Jeżeli warunek testowy ma wartość **prawda**, wynikiem testu jest **zgodna**. Jeżeli warunek testowy ma wartość **nieprawda**, alternatywna wersja zgodna nie istnieje, a wynikiem warunku testowego jest **nie ma zastosowania** (**ND**).

- Wyniki testów wersji alternatywnych zapewniających zgodność nie odpowiadają wzorcowi stosowanemu w pozostałych procedurach testowych, według którego jeżeli twierdzenia definiujące warunek testowy są **prawdą**, to treść **spełnia** wymagania (jest **zgodna**), jeżeli są **nieprawdą**, to treść **nie spełnia** wymagania (jest **niezgodna**). Ponieważ zapewnienie wersji alternatywnej zapewniającej zgodność nie jest wymagane, to jeśli w odniesieniu do wersji alternatywnej, która ma zapewnić zgodność, ocenia się, że twierdzenie definiujące warunek testowy jest **nieprawdą**, to uznaje się, że nie istnieje wersja alternatywna (oceniana wersja nie jest wersją alternatywną, bo nie spełnia wymagania) i w związku z tym ustala się wynik warunku testowego, że **nie ma zastosowania** 

Jeżeli wszystkie wymagania, które mają zastosowanie, nie zostaną spełnione w żadnej wersji alternatywnej, wersja alternatywna nie może być uznana za zgodną z wymaganiami, ponieważ musi być zgodna **ze wszystkimi** wymaganiami. W takim przypadku tester przestaje wykonywać testy wersji, która miała być alternatywną i obejmuje zakresem testowania wszystkie wersje treści. Przechodzi do następnego testu i rejestruje wyniki dla wszystkich wersji treści i dla wszystkich warunków testowych. Dlatego ważne jest, aby w momencie rozpoczęcia testów określić, czy istnieje deklarowana zgodna wersja alternatywna, aby do zakresu testów włączyć tylko odpowiednią treść,

Gdy zostanie znaleziona zgodna wersja alternatywna, niezgodne wersje treści można pominąć w zakresie testowania. Jednak przed całkowitym wykluczeniem niezgodnej wersji treści należy ocenić spełnienie pewnej ograniczonej liczby wymagań, aby się upewnić, że niezgodna treść nie zakłóca możliwości dostępu użytkownika do treści.

Wymagania dotyczące braku zakłóceń mają zastosowanie do wszystkich treści na stronie internetowej, w tym treści, które mają zgodną alternatywną wersję, ponieważ ich niespełnienie może zakłócać jakiekolwiek korzystanie ze strony.

Procedura testów zgodności wersji alternatywnej i braku zakłóceń jest pierwszą procedurą testową w procesie Trusted Tester, ponieważ jest niezbędna do określenia zakresu testów. 

Testy (warunki testowe) wersji alternatywnych zapewniających zgodność różnią się nieznacznie od pozostałych testów na kilka istotnych sposobów:

- Najpierw przedstawiono warunki testowania wersji alternatywnych zapewniających zgodność, ponieważ identyfikacja dostępnych wersji alternatywnych zapewniających zgodność treści pomaga ustalić zakres testowania. Niezgodna treść, która ma wersję alternatywną zapewniającą zgodność, jest testowana pod kątem zakłóceń, a następnie jest wyłączana z testów po tym teście.

-  Mimo że zidentyfikowanie wersji alternatywnych zapewniających zgodność w celu zdefiniowania zakresu testu jest ważne, ustalenie, czy zapewniono wersję alternatywną zapewniającą zgodność nie będzie możliwe, dopóki nie zakończą się wszystkie inne odpowiednie testy. (Wersja alternatywna zapewniająca zgodność nie może być uznana za taką, dopóki nie przejdzie wszystkich wymaganych testów).

Procedura testowa „Zgodna wersja alternatywna i brak zakłóceń” obejmuje pięć testów:

1.	Test 1.A Wersja-alt-zgodna 
2.  Test 1.B Wersja-alt-rownowazna
3.  Test 1.C Dostep-z-wersji-niezgodnej
4.  Test 1.D Dostep-do-wersji-niezgodnej
5.  Test 1.E Bez-zaklocen

## Dostępność wersji alternatywnej

### Test 1.A Wersja-alt-zgodna

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|---------------------------------------|
| Wersja-alt-zgodna | 1.A | Wersja alternatywna zapewniająca zgodność spełnia wszystkie wymagania testowe objęte tą procedurą testową. |

### Cel testu

Zapewnianie wielu wersji tej samej treści nie jest wymagane. Jeśli istnieje tylko jedna wersja treści i jest ona zgodna z wymogami Sekcji 508, wówczas inne wersje nie są konieczne.

Gdy treść nie spełnia wymogów dostępności, twórcy mogą zapewnić alternatywną wersję treści zapewniającą zgodność. Ale alternatywna wersja zapewniająca zgodność musi przejść wszystkie obowiązujące testy, aby można ją uznać za wersję alternatywną spełniającą wymogi dostępności. 

Aby być „zgodną wersją alternatywną”, zgodnie z definicją WCAG, należy spełnić wiele wymagań. Ten test jest tylko jednym z nich. 

Wersje alternatywne zapewniające zgodność mogą być prezentowane na wiele sposobów, na przykład za pomocą przełącznika strony do trybu dostępności, łącza prowadzącego do zgodnej wersji alternatywnej, łączy umożliwiających użytkownikom dostosowanie preferencji na stronie internetowej. 

Wyniki tego testu służą do ustalenia, czy spełnione są [wymagania WCAG dotyczące zgodności](wcag21#52-wymogi-dotyczące-zgodności)

### Metody i narzędzia testowe 
1.	Wszystkie narzędzia stosownie do wymaganych testów.


### Identyfikacja treści

Inne wersje tej samej treści, tj. treści, które zostały dostarczone na więcej niż jeden sposób, z wyraźnym lub dorozumianym zamiarem, aby jedna lub więcej z tych wersji była osiągana jako dostępna alternatywa.

**Uwaga**: Pomocne może być przejrzenie dokumentacji produktu w celu uzyskania informacji o dostępnych wersjach lub włączeniu ułatwień dostępu.

1.  Zgodne wersje alternatywne mogą być zapewnione dla części strony, całych stron lub całej witryny.
2.  Na istnienie zgodnej wersji alternatywnej mogą wskazywać różne mechanizmy, w tym:

    -   Instrukcje opisujące, jak włączyć dostępność
    -   Treść jest oznaczona jako zgodna wersja alternatywna (wersja dostępna)
    -   Istnieje kilka metod wykonania zadania (np. do wprowadzenia daty służą widżet kalendarza i pole tekstowe)
    -   Miejsce docelowym łącza jest zgodna wersja alternatywna lub wersja dla technologii wspomagających (np. wersja dla czytnika ekranu)
    -   Istnieją preferencje lub ustawienia użytkownika, umożliwiające włączenie ułatwień dostępu
    -   Istnieją elementy sterujące (narzędzia) użytkownika do modyfikowania kolorów i wyglądu tekstu.

3.	Zgodne wersje alternatywne nie muszą się znajdować się w „zakresie zgodności” (zbiorze stron, których dotyczy oświadczenie o zgodności), ani nawet w tej samej witrynie internetowej, o ile są równie łatwo osiągalne, jak wersja niezgodna. Na przykład alternatywna wersja może znajdować się w innej domenie niż testowana witryna. W przypadku tej procedury testowej zakres testów jest ograniczony tylko do zgodnych wersji alternatywnych, które są osiągalne na komputerach stacjonarnych. Zgodne wersje alternatywne nie obejmują aplikacji mobilnych, do których dostęp można uzyskać tylko na urządzeniu przenośnym.

### Zastosowanie:
Test 1.A Wersja-alt-zgodna **nie ma zastosowania**, jeśli istnieje tylko jedna wersja treści.

### Jak testować:

1.  Włącz dostępność za pomocą ustawień witryny, jeśli istnieją.

2.  Jeśli jedna z wersji została wskazana jako wersja dla celów dostępności, przyjmij, że jest to wersja alternatywna i w tym teście (id 1.A) podaj wyniki testów tylko dla tej wersji.

3.  Po zakończeniu procesu testowania przetestuj zidentyfikowaną wersję „dostępną” pod kątem  wszystkich obowiązujących warunków testowych.

    1. Przed ustaleniem wyniku może być konieczne przeprowadzenie szeroko zakrojonego badania, zanim zostanie znaleziony wynik dla danego warunku testu. Jeśli ustawienia użytkownika umożliwiają dostęp do całej witryny, cała witryna jest wersją alternatywną i cała witryna musi przejść wszystkie warunki testowe.

    2.  Jeśli w zidentyfikowanej „dostępnej” wersji zostanie stwierdzony defekt, wprowadź **nie spełnia** dla odpowiedniego ID testu. Nie jest konieczne kontynuowanie testów dla tego testu (ID 1.A) po znalezieniu błędu. Oceń wyniki.

    3.  Jeśli żadna z wersji nie została zidentyfikowana jako „dostępna”, należy przetestować wszystkie wersje, dopóki nie zostanie znaleziona wersja, która spełnia wszystkie obowiązujące warunki testowe.

        1.  Jeśli w danej wersji zostanie stwierdzone niepowodzenie, należy przerwać testowanie tej wersji i przetestować inne wersje.

       Aby ustalić, które warunki testowe mają zastosowanie, powinieneś przejrzeć treść tego, co uważa się za „wersję alternatywną”. W tym teście oceniana jest tylko treść dostępna w więcej niż jednej wersji. Przetestuj wersję alternatywną oznaczoną jako zgodną. Na przykład:
          - Jeśli istnieje film bez napisów i inny plik tego samego wideo, ale z napisami, to istnieje  wersja alternatywna. Twoim „zakresem testowania” jest tylko plik wideo z napisami. Reszta treści strony, jeśli taka istnieje, nie podlega testowaniu (nie jest objęta testem).
         - Jeśli dostępne są elementy sterujące dla użytkownika, takie jak regulacja kontrastu kolorów, dostępna jest wersja alternatywna. Włącz ustawienia kontrastu kolorów, a zakres testowania to tylko funkcja dopasowania kontrastu i cała treść, na którą miały wpływ te ustawienia.

### Ocena wyników
Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymagania zgodności, jeśli twierdzenie poniżej jest **fałszywe**, ten warunek testowy **nie ma zastosowania**.

1.	Istnieje alternatywna wersja treści, która spełnia wszystkie obowiązujące warunki testowe w tym procesie testowym.

Jeżeli wynikiem tego warunku testu jest:

-   **spełnia** wymagania, przejdź do testu 1.B. Wersja alternatywna, która przeszła ten test (1.A.) będzie określana w kolejnych testach jako „dostępna wersja”.

-   **nie ma zastosowania**, oznacz wyniki dla pozostałych testów (1.B - 1.E) tej wersji jako **nie ma zastosowania** i kontynuuj testowanie wszystkich wersji z kolejnymi warunkami testowymi. Wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z testu.

##### Uwaga:

-   Zgodne wersje alternatywne mogą być zapewniane dla różnych technologii lub grup użytkowników. Co najmniej jedna wersja musi przejść wszystkie warunki testowe (przejść pomyślnie wszystkie testy).

-   Pomocne może być przejrzenie dokumentacji produktu w celu uzyskania informacji o wersjach zapewniających zgodność lub włączeniu ułatwień dostępu.

-   Chociaż badanie warunków testowych dla wersji alternatywnej może zostać wstrzymane, gdy wersja określona jako „dostępna” nie spełnia warunków testowych, konieczne może być dalsze testowanie wersji, aby ukończyć pozostałe testy w tym procesie testowym. Jeżeli nie ma zgodnej wersji alternatywnej, wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z badania.

## Równoważność zgodnej wersji alternatywnej

### Test 1.B Wersja-alt-rownowazna

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| Wersja-alt-rownowazna | 1.B | Zgodna wersja alternatywna zawiera równoważne (takie same) informacje i funkcjonalności.|

### Cel testu
Celem tego testu jest sprawdzenie, czy dostępna wersja alternatywna (wersja, która przeszła test 1.A) zapewnia te same informacje i funkcje w tym samym języku naturalnym co treść niezgodna, oraz czy informacje są aktualne. 

Dostępna (zgodna) wersja alternatywna musi zapewniać użytkownikom treść równoważną treści wersji niezgodnej. 

Wyniki tego testu służą do ustalenia, czy spełnione są wymagania alternatywnej wersji WCAG .

Wyniki tego testu służą do ustalenia, czy spełnione są [wymagania WCAG dotyczące zgodności](wcag21#52-wymogi-dotyczące-zgodności)

### Metody i narzędzia testowe 
1.	Wszystkie narzędzia stosownie do wymaganych testów.


### Identyfikacja treści
Dostepna wersja alternatywna, która przeszła pomyślnie test 1.A. 


### Zastosowanie

Test 1.B Wersja-alt-rownowazna **nie ma zastosowania**, jeśli istnieje tylko jedna wersja treści (czyli jeśli test 1.A **nie ma zastosowania**).

### Jak testować

1.  Kontynuuj test 1.A.

2.  Przejrzyj treść wersji niezgodnej.

3.	Porównaj dostępną wersję alternatywną (która przeszła test 1.A) z wersją niezgodną pod kątem równoważności treści (tj. równoważnych informacji i funkcjonalności).

**Uwaga**: 

- Dostępna wersja musi być tak samo aktualna, jak wersja niezgodna, aby mogła zostać uznana za równoważną.

- Sprawdź, czy informacje w dostępnej wersji są w tym samym języku naturalnym co treść niezgodna (np. oryginalna treść jest w języku polskim, więc dostępna wersja również musi być w języku polskim).

### Ocena wyników
Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymagania zgodności, jeśli twierdzenie poniżej jest **fałszywe**, ten warunek testowy **nie ma zastosowania**.

1.	Dostępna (zgodna) wersja alternatywna (która przeszła test 1.A) zawiera wszystkie te same informacje i funkcjonalności, co treść niezgodna i przedstawione w tym samym języku ludzkim.

Jeżeli wynikiem tego warunku testu jest:

-   **spełnia** wymagania, przejdź do testu 1.C. 

-   **nie ma zastosowania**, oznacz wyniki dla pozostałych testów (1.C - 1.E) tej wersji jako **nie ma zastosowania** i kontynuuj testowanie wszystkich wersji z kolejnymi warunkami testowymi. Wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z testu.

### Uwaga

-   Dostępna (zgodna) wersja alternatywna nie musi być dopasowana „jeden do jednego” do oryginału (do wersji niezgodnej), np. zgodna wersja alternatywna może składać się z większej lub mniejszej liczby stron.

-   Chociaż testowanie wersji alternatywnej może zostać wstrzymane, gdy wersja „dostępna” nie spełnia warunków testowych, konieczne może być dalsze jej testowanie, aby ukończyć pozostałe testy w tym procesie testowym. Jeżeli nie ma dostępnej (zgodnej) wersji alternatywnej, wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z badania.


## Dostęp do zgodnej wersji alternatywnej

### Test 1.C Dostep-do-wersji-zgodnej

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| Dostep-do-wersji-zgodnej | 1.C |  Istnieje mechanizm umożliwiający osiągnięcie zgodnej wersji alternatywnej ze strony niezgodnej.|

### Cel testu

Zarówno ten test, jak i następny wymaga ustalenia, w jaki sposób można uzyskać dostęp do równoważnej dostępnej wersji (która przeszła pomyślnie test 1.B) i podjęcia decyzji, czy testy 1.C lub 1.D mają zastosowanie. 

Jeśli użytkownik najpierw napotka niezgodną wersję treści, a następnie musi przejść do dostępnej równoważnej wersji, przetestuj *1.C Dostep-do-wersji-zgodnej*. Jeśli użytkownik nie zobaczy najpierw niezgodnej treści , przetestuj *1.D Dostep-do-wersji-niezgodnej*.

Tylko jeden z tych testów, 1.C lub 1D może być przeprowadzony, oba nie mogą dotyczyć tej samej dostępnej równoważnej wersji.
 
Jeżeli test 1.C **nie ma zastosowania** do treści, o której mowa, tester musi przeprowadzić test 1.D. Możliwe jest, że wiele dostępnych równoważnych wersji **różnych** treści jest prezentowanych na różne sposoby (więc zarówno test 1.C, jak i 1.D mogą mieć zastosowanie, gdy oceniane są **różne** dostępne równoważne treści).


Na przykład tester może testować stronę internetową, która tylko na jednej stronie ma przycisk przełączania, który włączyć ustawienia dostępności dla formularzy. Ponieważ użytkownik otrzymuje najpierw wersję niezgodną z wymaganiami, zostanie ona przetestowana dla 1.C Dostep-do-wersji-zgodnej. W innym miejscu witryny znajduje się strona internetowa z dwoma łączami, które prowadzą użytkowników do „łącza do dostępnej wersja tabeli” lub „łącza do niezgodnego wykresu”. Ponieważ użytkownikowi nie została przedstawiona najpierw treść zgodna, tester wykona  najpierw test 1.D Dostep-do-wersji-niezgodnej. 
 
W danym momencie można użyć tylko **jednej** metody prezentacji każdej dostępnej równoważnej wersji, która podlega ocenie. Albo warunek testowy 1.C, albo 1.D musi być oceniony jako **spełniony** dla każdej dostępnej równoważnej wersji, aby można ją uznać za zgodną wersją alternatywną i kontynuować testowanie w 1.E.

Ten test obejmuje sprawdzenie metody, mechanizmu lub ścieżki użytkownika, które umożliwiają dostęp za pośrednictwem strony do dostępnej (zgodnej) wersji alternatywnej z wersji niezgodnej. Mechanizm zastosowany w celu uzyskania dostępu do dostępnej wersji alternatywnej musi być zgodny ze wszystkimi wymaganiami testu. Mechanizm może mieć różną postać, między innymi przycisku, łącza, klawiszy skrótów, równoczesnej prezentacji alternatywnej treści na tej samej stronie.   


Wyniki tego testu służą do ustalenia, czy spełnione są [wymagania WCAG dotyczące zgodności](wcag21#52-wymogi-dotyczące-zgodności)

### Metody i narzędzia testowe 
1.	Wszystkie narzędzia stosownie do wymaganych testów.


### Identyfikacja treści
Strona z niezgodną wersją treści, na której istnieje mechanizm, metoda lub ścieżka dostępu do dostępnej równoważnej wersji treści (która przeszła test 1.B).

Do osiągnięcia zgodnej wersji alternatywnej można zastosować różne metody, w tym:
-   łącze do zgodnej wersji alternatywnej lub wersji przeznaczonej dla technologii wspomagającej (np. wersji dla czytnika ekranu)
-   preferencje lub ustawienia użytkownika umożliwiające dostęp do strony lub całej witryny ze zgodną wersją alternatywną
-   Przełączniki (narzędzia użytkownika) służące do modyfikowania kolorów i wyglądu tekstu strony lub całej witryny
-   Wersja alternatywna zapewniająca zgodność znajduje się na tej samej stronie, co wersja niezgodna.

### Zastosowanie

Test 1.C Dostep-do-wersji-zgodnej **nie ma zastosowania**, jeśli  
- istnieje tylko jedna wersja treści albo 
- test z identyfikatorem 1.A lub 1.B został oceniony jako **NIE MA ZASTOSOWANIA**, albo 
- jeśli użytkownik nie spotyka się najpierw z wersją niezgodną (wtedy przejdź do testu 1.D).

**Wskazówka**: Zadaj sobie pytanie, czy punktem wyjścia jest niezgodna treść lub strona z niezgodną treścią?
•	Jeśli tak, wykonaj ten test (1.C).
•	Jeśli nie, oznacz 1.C jako **nie ma zastosowania** i wykonaj test 1.D.

**Uwaga**: Tylko **jedna** metoda może być użyta do zaoferowania użytkownikowi zgodnej wersji alternatywnej: 
   - **albo** użytkownik najpierw napotyka treść  niezgodną i musi nawigować do zgodnej wersji alternatywnej wersji (testowanej w 1.C) 
   - **albo** użytkownik **nie spotyka się** najpierw z wersją niezgodną  (wówczas przejdź do testu 1.D).

**Albo tylko** wynik testu 1.C, **albo tylko** wynik testu 1.D musi być oceniony jako **spełniony**; nie można zastosować obu testów równocześnie do tej samej zgodnej wersji alternatywnej (dostępnej i równoważnej).


### Jak testować:

1.  Kontynuuj test 1.B.

2.  Zidentyfikuj mechanizm używany do osiągnięcia zgodnej wersji alternatywnej (dostępnej równoważnej, która przeszła test 1.B).

    1.  W razie potrzeby wróć na stronę, na której znajduje się mechanizm umożliwiający wybranie lub włączenie zgodnej wersji alternatywnej.

    2.  Może to być łącze lub funkcja na stronie niezgodnej

    3.  Mogą to być ustawienia użytkownika lub preferencje.

3.  Po zakończeniu tego procesu testowego przetestuj mechanizm pod kątem wszystkich obowiązujących warunków testowych.


### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymagania zgodności, jeśli twierdzenie poniżej jest **fałszywe**, ten warunek testowy **nie ma zastosowania**.

1.  Mechanizm zastosowany w celu osiągnięcia zgodnej wersji alternatywnej (dostępnej równoważnej) spełnia wszystkie obowiązujące warunki testu.

Jeżeli wynikiem tego warunku testu jest:

-   **spełnia** oznacz test 1.D jako **nie ma zastosowania** i przejdź do testu 1.E 

-   **nie ma zastosowania**, ponieważ 

   - wersja niezgodna nie była pierwszą oferowaną użytkownikom, przejdź do testu 1.D.
   - na stronie z wersją niezgodną nie istnieje mechanizm, który umożliwia osiągnięcie zgodnej wersji alternatywnej, oznacz testy 1.D oraz 1.E jako **nie ma zastosowania** i&nbsp;kontynuuj testowanie wszystkich wersji z kolejnymi warunkami testowymi. 
   
Wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z testu.


### Uwaga:

-   Testy odpowiednich mechanizmów mogą obejmować łacza i przyciski, nagłówki, formularze  lub inne testy.

-   Mechanizm dostępu do zgodnej wersji alternatywnej powinien bezpośrednio lub pośrednio wskazywać, że prowadzi do wersji dostępnej. Na przykład tekst poprzedzający tekst łącza do wersji zgodnej może wprost wskazywać, że łącze prowadzi do zgodnej wersji alternatywnej. Możliwe jest również „ukrywanie” treści niezgodnych z technologiami wspomagającymi i  wykluczenie ich z porządku tabulacji, ograniczając w ten sposób dostęp tylko do wersji zapewniających dostępność dla użytkowników z  niepełnosprawnościami. Takie podejście może jednak nie być możliwe, w zależności od treści.

-   Mechanizm może być wyraźnie podany w treści lub może być oparty na zapewnieniu przez platformę lub przez użytkownika, w tym technologie wspomagające.

-   Mechanizm musi spełniać wszystkie kryteria sukcesu dla deklarowanego poziomu zgodności.

### Dostep do wersji niezgodnej

### Test 1.D Dostep-do-wersji-niezgodnej

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| Dostep-do-wersji-niezgodnej | 1.D | Dostęp do wersji niezgodnej można uzyskać tylko z wersji zgodnej. |

### Cel testu 
Ten test, podobnie jak poprzedni, wymaga najpierw zrozumienia, w jaki sposób można uzyskać dostęp do równoważnej dostępnej wersji, a następnie podjęcia decyzji o zastosowaniu testu 1.C lub 1.D. Jeśli test 1.C **nie miał zastosowania**, ponieważ użytkownik nie zaczyna od strony z wersją niezgodną, wykonaj test 1.D. Testów 1.C i 1.D nie można zastosować jednocześnie do tej samej dostępnej wersji równoważnej. (Mogą one mieć zastosowanie do dwóch różnych dostępnych równoważnych wersji o różnej zawartości lub funkcjonalności).

Celem tego testu jest ustalenie, czy do niezgodnej wersji treści można dotrzeć tylko z treści zgodnej (z wersji zgodnej do wersji niezgodnej lub ze strony internetowej zawierającej mechanizm do osiągnięcia zarówno zgodnej, jak i niezgodnej wersji treści), dzięki czemu użytkownicy, którzy chcą przejść do zgodnych treści, mogą to zrobić bez napotkania jakichkolwiek barier dostępności. 

Wyniki tego testu służą do ustalenia, czy spełnione są [wymagania WCAG dotyczące zgodności](wcag21#52-wymogi-dotyczące-zgodności)

### Metody i narzędzia testowe 
1.	Inspekcja ręczna.
2.	Wszystkie narzędzia stosownie do wymaganych testów.


### Identyfikacja treści

Wszystkie mechanizmy, metody i ścieżki dostępu do niezgodnych wersji treści.

Jeśli wynikiem dla testu 1.A lub dla testu 1.B było **nie ma zastosowania**, wówczas wynik dla testów od 1.C do 1.E również **nie ma zastosowania**.  Jeśli wynikiem dla testu 1.C jest **spełnione**, wówczas wynikiem testu 1.D jest **nie ma zastosowania**.

**Wskazówka**: Aby upewnić się, że stosujesz właściwy test, dokładnie sprawdź punkt początkowy, aby uzyskać dostęp do wersji niezgodnej. Zapytaj siebie:

Czy zacząłem od wersji niezgodnej lub strony zawierającej wersję niezgodną?

-	Jeśli tak, wróć i przetestuj to pod 1.C.
-	Jeśli nie, sprawdź 1.D.

W testach w świecie rzeczywistym częściej spotyka się scenariusz, który byłby testowany w wersji 1.C, gdzie domyślnie dostępna jest wersja niezgodna. „Mechanizm” jest szeroko definiowany jako proces lub technika służąca do osiągnięcia rezultatu i może być wyraźnie podany w treści, albo może być zapewniony przez platformę lub przez programy użytkowników, w tym przez technologie wspomagające. Na przykład, użytkownik korzystający wyłącznie z klawiatury może polegać na systemie operacyjnym i funkcji przeglądarki przy korzystaniu z klawiatury. Użytkownik korzystający z czytnika ekranowego prawdopodobnie polegałby na dodatkowych funkcjach, które oferuje jego czytnik ekranowy do poruszania się po treści strony internetowej.


### Zastosowanie:
Test 1.D Dostep-do-wersji-niezgodnej **nie ma zastosowania**, jeśli 

-   jest tylko jedna wersja treści **lub**
-   test 1.A lub test 1.B oceniono jako **nie ma zastosowania**, **lub**
-   test 1.C oceniono jako **spełniony**.

### Jak testować

1.  Ustal, w jaki sposób można uzyskać dostęp do niezgodnej wersji treści.

    1.  Do wersji niezgodnej można uzyskać dostęp tylko ze zgodnej wersji alternatywnej ( dostępnej równoważnej wersji).

    2.  Zarówno dostęp do zgodnej wersji alternatywnej, jak i dostęp do wersji niezgodnej można uzyskać z innej strony.

        1.  Czy strona zapewniająca dostęp jest zgodna ze wszystkimi mającymi zastosowanie procedurami testowymi?

        2.  Czy istnieje inny sposób uzyskania dostępu do wersji niezgodnej?

### Ocena wyników
Jeśli którekolwiek z twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymagania zgodności, jeśli twierdzenie poniżej jest **fałszywe**, ten warunek testowy **nie ma zastosowania**.

1.  Wersję niezgodną można osiągnąć tylko ze zgodnej wersji alternatywnej (z dostępnej równoważnej wersji, która przeszła test 1.B) **albo**

2.  Wersja niezgodna jest dostępna tylko ze strony, która:

    1.  spełnia wszystkie pozostałe warunki testu **oraz**

    2.  zapewnia również mechanizm umożliwiający osiągnięcie zgodnej wersji alternatywnej (dostępnej równoważnej wersji, która przeszła test 1.A oraz test 1.B).


**Albo** wynikiem testu 1.C, **albo**  wynikiem testu 1.D musi być **spełnia wymagania**, aby istniała zgodna wersja alternatywna. Jeżeli wynikiem tego testu jest


-   **spełnia**, przejdź do testu 1.E

-   **nie ma zastosowania** oraz test 1.C został oznaczony **spełnia**, przejdź do testu 1.E

-   **nie ma zastosowania** oraz test 1.C został oznaczony **nie ma zastosowania** i&nbsp;kontynuuj testowanie wszystkich wersji z kolejnymi warunkami testowymi.

### Uwaga

-   Jeśli ocena wyników kroku 2 powyżej była **prawdą**, zarówno strona, jak i mechanizm muszą przejść wszystkie obowiązujące warunki testu. Po zakończeniu procesu testowania przetestuj stronę i mechanizm pod kątem wszystkich odpowiednich warunków testowych.

## Brak zakłóceń

### Test 1.E Bez-zaklocen

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| Bez-zaklocen | 1.E     | Treści w wersjach niezgodnych spełniają wymóg zgodności 5. |

### Cel testu

Celem tego testu jest sprawdzenie, czy niezgodna treść, która ma zgodną alternatywną wersję, nie zakłóca ani nie blokuje możliwości interakcji użytkownika z treścią zgodną. 
Wykonując pięć konkretnych testów niezgodnych treści, sprawdzisz, czy strona internetowa:
-	Umożliwia użytkownikom wstrzymywanie, zatrzymywanie lub kontrolowanie głośności odtwarzanej automatycznie treści audio **oraz**
-	Umożliwia użytkownikom wstrzymywanie, zatrzymywanie lub ukrywanie ruchomych, migających lub przewijanych treści **oraz**
-	Umożliwia użytkownikom zatrzymywanie, wstrzymywanie, ukrywanie lub kontrolowanie częstotliwości automatycznie aktualizowanych treści **oraz**
-	Nie ma zawartości błyskającej **oraz**
-	Nie ma pułapki na klawiaturę.

Wyniki tego testu służą do ustalenia, czy spełnione są [wymagania WCAG  5.2.5 Brak zakłóceń](wcag21#525-brak-zakłóceń)

### Metody i narzędzia testowe 
1.	Wszystkie narzędzia stosownie do wymaganych testów.

### Identyfikacja treści

Niezgodne wersje treści, które mają alternatywną wersję zgodną.

### Zastosowanie
Test 1.E Bez-zaklocen **nie ma zastosowania**, jeżeli:

-  jest tylko jedna wersja treści, **lub**

-  testy 1.C i 1.D oceniono jako  **nie ma zastosowania**.

### Jak testować:

1.  Niezgodna treść, która ma zgodną alternatywną wersję, musi zostać przetestowana przed wyłączeniem treści z pozostałej części testowania.
    
	1. Przejdź do treści niezgodnej

2.  Jeśli to konieczne lub ma zastosowanie, wyłącz funkcje ułatwień dostępu w ustawieniach witryny lub preferencjach.

3.  Po zakończeniu tego procesu testowego **wykonaj tylko** następujące testy niezgodnej wersji treści:

    1.  Test 2.A - 1.4.2-sterowanie-dzwiekiem

    2.  Test 2.B - 2.2.2-tresci-ruchome

    3.  Test 2.C - 2.2.2-automatyczna-aktualizacja

    4.  Test 3.A - 2.3.1-migotanie

    5.  Test 4.C - 2.1.2-bez-pułapki-na-klawiaturę

4.  Oznacz odpowiedni identyfikator testu, jeżeli którykolwiek z powyższych testów daje wynik **niespełnione** lub **nie testowano** (dla testu 3.A).

### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymagania zgodności, jeśli twierdzenie poniżej jest **fałszywe**, ten warunek testowy **nie ma zastosowania** 

1.  Wyniki dla każdego z poniższych testów to **spełnia** lub **nie ma zastosowania** w&nbsp;przypadku niezgodnych wersji treści (**nie testowano** dla testu 3.A).

    1.  Test 2.A - 1.4.2-sterowanie-dzwiekiem

    2.  Test 2.B - 2.2.2-tresci-ruchome

    3.  Test 2.C - 2.2.2-automatyczna-aktualizacja

    4.  Test 3.A - 2.3.1-migotanie

    5.  Test 4.C - 2.1.2-bez-pułapki-na-klawiaturę

**Uwaga:** Po wykonaniu tego testu na niezgodnej wersji treści, która ma zgodną wersję alternatywną, pomiń testowanie niezgodnej treści w pozostałej części testowania.

## Obowiązujące normy

[Wersja alternatywna zapewniająca zgodność](http://www.fdc.org.pl/wcag2/index.html#conforming-alternate-versiondef) nie jest wymogiem. Wymóg zgodności \#1 pozwala na włączenie do zakresu zgodności stron niezgodnych z wymaganiami, o ile mają one „zgodną wersję alternatywną”. Gwarantuje to, że wszystkie informacje i wszystkie funkcje, które znajdują się na stronach objętych zakresem zgodności, są dostępne na stronach internetowych zgodnych z wymogami.

[20. Zgodność z wersją alternatywną](ICT-20-wersje-alternatywne)

[Wymóg zgodności WCAG 5.2.5 Brak zakłóceń](https://www.w3.org/TR/WCAG20/#conformance-reqs): Następujące kryteria sukcesu dotyczą wszystkich treści na stronie, włącznie z treściami, które w innych przypadkach nie są podstawą spełnienia wymogów zgodności, ponieważ niezastosowanie poniższych kryteriów mogłoby uniemożliwiać korzystanie ze strony:
- 1.4.2 Kontrola odtwarzania dźwięku
- 2.1.2 Brak pułapki na klawiaturę,
- 2.3.1 Trzy błyski lub wartości poniżej progu, oraz
- 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie.

[25. Brak zakłóceń](ICT-25-brak-zaklocen)