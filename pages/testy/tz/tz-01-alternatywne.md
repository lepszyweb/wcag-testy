---
title: 1. Zgodna wersja alternatywna i brak zakłóceń

sidebar: testy_sidebar
permalink: tz-01-alternatywne
folder: testy/tz
---


{% include note.html content="Praca nad tłumaczeniem trwa. To jest zgrubna, robocza wersja tłumaczenia." %}


## Cel zestawu testów

Testy z tego zestawu służą ocenie wersji alternatywnych zapewniających zgodność oraz spełniania wymogu [Brak zakłóceń](wcag21#525-brak-zakłóceń), gdy na stronie wykorzystywane są technologie, które nie obsługują dostępności albo użyte są tak, że nie obsługują dostępności.

Można udostępniać wiele wersji treści, o ile jedna z nich jest w pełni zgodna na wybranym poziomie. Zapewnienie wersji alternatywnej zapewniającej zgodność nie jest wymagane przez WCAG. Jest to raczej dopuszczalna metoda zapewnienia samych informacji i funkcji w przystępny sposób, gdy istnieją inne niezgodne wersje tych treści, czyli wersje niespełniające norm dostępności.

Na stronie internetowej mogą być zastosowane technologie internetowe, które nie obsługują dostępności albo nie są obsługiwane przez dostępność, albo zostały użyte tak, że nie obsługują dostępności. W takich przypadkach można uznać, że spełnione są normy dostępności pod warunkiem, że technologie, które nie obsługują dostępności nie blokują użytkownikom dostępu do reszty strony.       

Celem tej procedury jest sprawdzenie, w przypadku gdy witryna internetowa zawiera alternatywne wersje treści w&nbsp;celu spełnienia wymagań dostępności, 

- czy podana zgodna wersja alternatywna jest rzeczywiście dostępna i równoważna
- czy wersje spełniają wymagania WCAG dotyczące dotarcia do alternatywnej treści, z wersji niezgodnej do wersji zgodnej. 

Zanim alternatywną wersję można uznać za „zgodną wersję alternatywną”, należy ocenić:
- czy wersja alternatywna jest w pełni dostępna,
- czy wersja alternatywna zapewnia równoważne informacje i funkcje,
- czy wszyscy użytkownicy mogą dotrzeć zarówno do zgodnej wersji alternatywnej, jak i do wersji niezgodnej, niespełniającej wymogów zgodności.

Ta procedura testowa różni się od innych procedur w tym procesie testowym. Wykonując audyt zgodności, musisz najpierw ustalić, czy istnieje alternatywna wersja treści zapewniająca zgodność i ustalić, czy spełnia ona wszystkie wymagania „zgodnej wersji alternatywnej”. 

To określi zakres twojego audytu. 

Jeśli istnieje zgodna wersja alternatywna, to ta wersja zasadniczo zastępuje wersję niezgodną w zakresie testowania, a wersja niezgodna nie jest uwzględniona w raporcie z testu.

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
4.  Test 1.D Bez-zaklocen

## Dostępność wersji alternatywnej

### Test 1.A Wersja-alt-zgodna

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|---------------------------------------|
| Wersja-alt-zgodna | 1.A | Wersja alternatywna zapewniająca zgodność spełnia wszystkie wymagania testowe objęte tą procedurą testową. |

### Cel testu

Zapewnianie wielu wersji tej samej treści nie jest wymagane. Jeśli istnieje tylko jedna wersja treści i jest ona zgodna z wymogami WCAG, wówczas inne wersje nie są konieczne.

Gdy treść nie spełnia wymogów dostępności, twórcy te same informacje i funkcje w dostępny sposób. Ale alternatywna wersja treści musi przejść wszystkie obowiązujące testy, aby można ją uznać „zgodną wersję alternatywną”. 

Aby być „zgodną wersją alternatywną” zgodnie z definicją WCAG, należy spełnić wiele wymagań; ten test jest tylko jednym z nich. 

Alternatywne wersje mogą być prezentowane na wiele sposobów, na przykład za pomocą  przełącznika strony do trybu dostępności, łącza prowadzącego do zgodnej wersji alternatywnej, łączy umożliwiających użytkownikom dostosowanie preferencji na stronie internetowej.

Wyniki tego testu służą do ustalenia, czy spełnione są [wymagania WCAG dotyczące zgodności](wcag21#52-wymogi-dotyczące-zgodności).

### Metody i narzędzia testowe 
1.	Wszystkie narzędzia stosownie do wymaganych testów.


### Identyfikacja treści

Zidentyfikuj inne wersje tej samej treści, tj. treści, które zostały dostarczone na więcej niż jeden sposób, z wyraźnym lub dorozumianym zamiarem, aby jedna lub więcej z tych wersji była osiągana jako dostępna alternatywa.

**Uwaga**: Pomocne może być przejrzenie dokumentacji produktu w celu uzyskania informacji o dostępnych wersjach lub włączeniu funkcji dostępności.

1.  Zgodne wersje alternatywne mogą być zapewnione dla części strony, całych stron lub całej witryny.
2.  Na istnienie zgodnej wersji alternatywnej mogą wskazywać różne mechanizmy, w tym:

    -   Instrukcje opisujące, jak włączyć dostępność
    -   Treść jest oznaczona jako zgodna wersja alternatywna (wersja dostępna)
    -   Istnieje kilka metod wykonania zadania (np. do wprowadzenia daty służą widżet kalendarza i pole tekstowe)
    -   Miejscem docelowym łącza jest zgodna wersja alternatywna lub wersja dla technologii wspomagających (np. wersja dla czytnika ekranu)
    -   Istnieją preferencje lub ustawienia użytkownika, umożliwiające włączenie ułatwień dostępu
    -   Istnieją elementy sterujące (narzędzia) użytkownika do modyfikowania kolorów i wyglądu tekstu.

3.	Zgodne wersje alternatywne nie muszą się znajdować się w zakresie zgodności (zbiorze stron, których dotyczy oświadczenie o zgodności), ani nawet w tej samej witrynie internetowej, o ile są równie łatwo osiągalne, jak wersja niezgodna. Na przykład alternatywna wersja może znajdować się w innej domenie niż testowana witryna. W przypadku tego procesu testowego zakres testów jest ograniczony tylko do alternatyw, które są osiągalne na komputerach stacjonarnych. Alternatywne wersje nie obejmują aplikacji mobilnych, do których dostęp można uzyskać tylko na urządzeniu przenośnym.

### Zastosowanie:
Test 1.A Wersja-alt-zgodna **nie ma zastosowania**, jeśli istnieje tylko jedna wersja treści.

### Jak testować:

1.	Włącz funkcje dostępności (jeśli to konieczne), wybierz wersję treści oznaczoną jako zgodna wersja alternatywna i przejdź do niej.
2.	Po zakończeniu tego procesu testowego przetestuj oznaczoną zgodną wersję alternatywną pod kątem wszystkich obowiązujących warunków testowych. Zapisz wyniki dla każdego obowiązującego testu.
    1. Jeśli nie zostaną znalezione żadne błędy, może to być zgodna wersja alternatywna.
    2. Jeśli zostanie znaleziony błąd, oznaczona wersja nie jest zgodną wersją alternatywną.
	3. Jeśli istnieją jeszcze inne wersje alternatywne oznaczone jako zgodne, przetestuj je, dopóki nie zostanie znaleziona wersja, która spełnia wszystkie obowiązujące warunki testowe.

### Ocena wyników
Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymagania zgodności, jeśli twierdzenie poniżej jest **fałszywe**, ten warunek testowy **nie ma zastosowania**.

1. Wersja treści oznaczona jako zgodna wersja alternatywna treści (wersja dostępna) spełnia wszystkie obowiązkowe warunki testowe w tym procesie testowym.

**Uwaga:** Zgodne wersje alternatywne mogą być zapewniane dla różnych środowisk technologicznych lub grup użytkowników. W takim przypadku co najmniej jedna wersja musi spełnić wszystkie warunki testowe (przejść pomyślnie wszystkie testy obowiązkowe w tym procesie testowym)


Jeżeli wynikiem tego warunku testu jest:

-   **spełnia** wymagania, przejdź do testu 1.B. Wersja alternatywna, która przeszła ten test (1.A.) będzie określana w kolejnych testach jako „dostępna wersja”.

-   **nie ma zastosowania**, oznacz wyniki dla pozostałych testów (1.B - 1.E) tej wersji jako **nie ma zastosowania** i kontynuuj testowanie wszystkich wersji z kolejnymi warunkami testowymi. Wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z testu.


##### Uwaga:

-   Pomocne może być przejrzenie dokumentacji produktu w celu uzyskania informacji o wersjach zapewniających zgodność lub włączeniu ułatwień dostępu.

-   Chociaż badanie warunków testowych dla wersji alternatywnej może zostać wstrzymane, gdy wersja określona jako „zgodna” nie spełnia warunków testowych, konieczne może być dalsze testowanie wersji, aby ukończyć pozostałe testy w tym procesie testowym. Jeżeli nie ma zgodnej wersji alternatywnej, wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z badania.

## Równoważność zgodnej wersji alternatywnej

### Test 1.B Wersja-alt-rownowazna

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| Wersja-alt-rownowazna | 1.B | Zgodna wersja alternatywna zawiera równoważne (takie same) informacje i funkcje.|

### Cel testu
Celem tego testu jest sprawdzenie, czy dostępna wersja alternatywna (wersja, która przeszła test 1.A) zapewnia te same informacje i funkcje w tym samym języku naturalnym co treść niezgodna oraz czy informacje są aktualne. 

Innymi słowy, celem jest potwierdzenie, że użytkownicy zgodnej wersji alternatywnej mają podane równoważne i aktualne informacje. 

Wyniki tego testu służą do ustalenia, czy spełnione są [wymagania WCAG dotyczące zgodności](wcag21#52-wymogi-dotyczące-zgodności)

### Metody i narzędzia testowe 
1.	Wszystkie narzędzia stosownie do wymaganych testów.


### Identyfikacja treści
Zgodna wersja alternatywna, która przeszła pomyślnie test 1.A. 


### Zastosowanie

Test 1.B Wersja-alt-rownowazna **nie ma zastosowania**, jeśli istnieje tylko jedna wersja treści (czyli jeśli test 1.A **nie ma zastosowania**).

### Jak testować

1.  Kontynuuj test 1.A.

2.  Przejrzyj treść wersji niezgodnej.

3.	Porównaj zgodną wersję alternatywną (tę, która przeszła test 1.A) z wersją niezgodną pod kątem równoważności treści (tj. równoważnych informacji i funkcji).

**Uwaga**: 

- Dostępna wersja musi być tak samo aktualna, jak wersja niezgodna, aby mogła zostać uznana za równoważną.

- Sprawdź, czy informacje w dostępnej wersji są w tym samym języku naturalnym co treść niezgodna (np. oryginalna treść jest w języku polskim, więc dostępna wersja również musi być w języku polskim).

### Ocena wyników
Jeśli twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymagania zgodności, jeśli twierdzenie poniżej jest **fałszywe**, ten warunek testowy **nie ma zastosowania**.

1. Zgodna wersja alternatywna (która przeszła test 1.A) zawiera wszystkie te same informacje i funkcje, co treść niezgodna
2. Treści zgodnej wersji alternatywnej są aktualne.
3. Treści zgodnej wersji alternatywnej są przedstawione w tym samym języku ludzkim.

Jeżeli wynikiem testu tego warunku jest:

-   **spełnia** wymagania, przejdź do testu 1.C. 

-   **nie ma zastosowania**, oznacz wyniki dla pozostałych testów (1.C - 1.E) tej wersji jako **nie ma zastosowania** i kontynuuj testowanie wszystkich wersji z kolejnymi warunkami testowymi. Wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z testu.

### Uwaga

-   Dostępna (zgodna) wersja alternatywna nie musi być dopasowana „jeden do jednego” do oryginału (do wersji niezgodnej), np. zgodna wersja alternatywna może składać się z większej lub mniejszej liczby stron.

-   Chociaż testowanie wersji alternatywnej może zostać wstrzymane, gdy wersja zgodna nie spełnia warunków testowych, konieczne może być dalsze jej testowanie, aby ukończyć pozostałe testy w tym procesie testowym. Jeżeli nie ma dostępnej (zgodnej) wersji alternatywnej, wszystkie wersje treści powinny zostać przetestowane i uwzględnione w raporcie z badania.


## Dostęp do zgodnej wersji alternatywnej

### Test 1.C Dostep-do-wersji-zgodnej

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| Dostep-do-wersji-zgodnej | 1.C |  Istnieje mechanizm umożliwiający osiągnięcie zgodnej wersji alternatywnej ze strony niezgodnej.|

### Cel testu

Zarówno ten test, jak i następny wymaga ustalenia, w jaki sposób można uzyskać dostęp do równoważnej dostępnej wersji (która przeszła pomyślnie test 1.B) i podjęcia decyzji, czy testy 1.C lub 1.D mają zastosowanie. 

### Identyfikacja treści
1. Strona z niezgodną wersją treści, na której wskazano, że istnieje zgodna wersja alternatywna i zapewniono mechanizm, za pomocą którego można dotrzeć do tej zgodnej wersji alternatywnej.

2.  Na stronie z niezgodną wersją treści zidentyfikuj mechanizm używany do osiągnięcia zgodnej wersji alternatywnej (dostępnej równoważnej, która przeszła test 1.B).

    -   Może to być łącze do zgodnej wersji alternatywnej lub zgodnej wersji  alternatywnej przeznaczonej dla technologii wspomagającej (np. wersji dla czytnika ekranu).

    -   Może to być widżet z ustawieniami preferencji użytkownika włączający funkcje dostępności dla strony lub całej witryny.

    -   Mogą to być  przełączniki (narzędzia użytkownika) służące do modyfikowania kolorów i wyglądu tekstu na stronie lub w całej witrynie.
	
<!-- -

Do osiągnięcia zgodnej wersji alternatywnej można zastosować różne metody (mechanizmy), w tym::
-   łącze do zgodnej wersji alternatywnej lub wersji przeznaczonej dla technologii wspomagającej (np. wersji dla czytnika ekranu)
-   preferencje lub ustawienia użytkownika włączające funkcje dostępności dla strony lub całej witryny
-   Przełączniki (narzędzia użytkownika) służące do modyfikowania kolorów i wyglądu tekstu na stronie lub w całej witrynie
-   Wersja alternatywna zapewniająca zgodność znajduje się na tej samej stronie, co wersja niezgodna.
   Przechodzenie do zidentyfikowanej dostępnej wersji zawartości na stronie -->


### Jak testować:

1.	Wykonaj testy od 2 do 20 dla mechanizmu używanego do osiągnięcia  zgodnej wersji alternatywnej.

Uwaga: W praktyce rzadko kiedy trzeba przeprowadzać wszystkie 18 testów. Zazwyczaj większość testów nie będzie miała zastosowania. Na przykład, jeśli mechanizmem dostępu będzie łącze internetowe, to konieczne mogą być testy badające spełnienie KS 1.1.1 Treść nietekstowa, 1.4.1 Użycie koloru, 1.4.3 Kontrast minimalny, 1.4.5 Obrazy tekstu, 2.4.4 Cel łącza (w kontekście), 2.5.5 Etykieta w nazwie.  


### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** ten warunek testowy, jeśli twierdzenie poniżej jest **fałszywe**, ten testowanie tego warunku kończy się wynikiem **niezaliczony**.


1. Mechanizm zastosowany w celu osiągnięcia zgodnej wersji alternatywnej spełnia wszystkie obowiązujące warunki testowe.


**Uwagi:**
-   Testy odpowiednich mechanizmów mogą obejmować łącza i przyciski, nagłówki, formularze lub inne testy.
-   Mechanizm dostępu do wersji zgodnej powinien bezpośrednio lub pośrednio wskazywać, że prowadzi on do wersji zgodnej. Na przykład tekst poprzedzający łącze do wersji z funkcjami dostępności może bezpośrednio informować, że łącze prowadzi do wersji z funkcjami dostępności. Możliwe jest również „ukrywanie” treści niezgodnych z technologiami wspomagającymi i  wykluczenie ich z porządku tabulacji, ograniczając w ten sposób dostęp tylko do wersji zgodnej zapewniającej dostępność użytkownikom z niepełnosprawnościami. Takie podejście może jednak nie być możliwe, w zależności od treści.
-   Mechanizm ten może być wyraźnie wskazany w treści lub może być zapewniony przez platformę lub przez programy użytkownika, w tym technologie wspomagające.
-   Mechanizm musi spełniać wszystkie kryteria sukcesu dla deklarowanego poziomu zgodności.

Wyniki tego testu służą do ustalenia, czy spełnione są [wymagania WCAG dotyczące zgodności](https://www.w3.org/Translations/WCAG21-pl/#conformance-reqs)


## Brak zakłóceń

### Test 1.D Bez-zaklocen

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|--------------------------------------------|
| Bez-zaklocen | 1.D     | Treści w wersjach niezgodnych spełniają wymóg zgodności 5. |

### Cel testu

Celem tego testu jest sprawdzenie, czy niezgodna treść, która ma zgodną wersję alternatywną, nie zakłóca ani nie blokuje możliwości interakcji użytkownika z treścią zgodną. 

Wykonując pięć konkretnych testów niezgodnych treści, sprawdzisz, czy strona internetowa:
1.	Umożliwia użytkownikom wstrzymywanie, zatrzymywanie lub kontrolowanie głośności odtwarzanej automatycznie treści audio **oraz**
2.	Umożliwia użytkownikom wstrzymywanie, zatrzymywanie lub ukrywanie ruchomych, migających lub przewijanych treści **oraz**
3.	Umożliwia użytkownikom zatrzymywanie, wstrzymywanie, ukrywanie lub kontrolowanie częstotliwości automatycznie aktualizowanych treści **oraz**
4.	Nie ma zawartości błyskającej **oraz**
5.	Nie ma pułapki na klawiaturę.

Wyniki tego testu służą do ustalenia, czy spełnione są [wymagania WCAG  5.2.5 Brak zakłóceń](https://www.w3.org/Translations/WCAG21-pl/#cc5)


### Metody i narzędzia testowe 
1.	Wszystkie narzędzia stosownie do wymaganych testów.

### Identyfikacja treści

Niezgodne wersje treści, które mają alternatywną wersję zgodną.

### Zastosowanie
Test 1.D Bez-zaklocen **nie ma zastosowania**, jeżeli test 1.A oceniono jako  **nie ma zastosowania**.

### Jak testować:

1.  Niezgodna treść, która ma zgodną alternatywną wersję, musi zostać przetestowana przed jej wyłączeniem z pozostałej części testowania.
    
	1. Przejdź do treści niezgodnej

2.  Jeśli to konieczne lub ma zastosowanie, wyłącz funkcje dostępności w ustawieniach witryny lub preferencjach.

3.  **Wykonaj tylko** następujące testy na niezgodnych wersjach treści:

    1.  Test 2.A - 1.4.2-sterowanie-dzwiekiem

    2.  Test 2.B - 2.2.2-tresci-ruchome

    3.  Test 2.C - 2.2.2-automatyczna-aktualizacja

    4.  Test 3.A - 2.3.1-migotanie

    5.  Test 4.C - 2.1.2-bez-pułapki-na-klawiaturę

4.  Wprowadź wyniki testów do odpowiednich identyfikatorów testów wymienionych powyżej

5.  Nie wykonuj żadnych dalszych testów na niezgodnych wersjach treści.

### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, to test kończy się wynikiem **ZALICZONY**, jeśli twierdzenie poniżej jest **fałszywe**, to test kończy się wynikiem **NIEZALICZONY**. 

1.  Wyniki każdego z poniższych testów to **ZALICZONY** lub **nie ma zastosowania** wszystkich wersji niezgodnych z wymaganiami.

    1.  Test 2.A - 1.4.2-sterowanie-dzwiekiem

    2.  Test 2.B - 2.2.2-tresci-ruchome

    3.  Test 2.C - 2.2.2-automatyczna-aktualizacja

    4.  Test 3.A - 2.3.1-migotanie

    5.  Test 4.C - 2.1.2-bez-pułapki-na-klawiaturę

**Uwaga:** Po wykonaniu tego testu na niezgodnej wersji treści, która ma zgodną wersję alternatywną, pomiń testowanie niezgodnej treści w pozostałej części testowania.


## Obowiązujące normy

[Wersja alternatywna zapewniająca zgodność](https://www.w3.org/Translations/WCAG21-pl/#conformance-reqs) nie jest wymogiem. Wymóg zgodności \#1 pozwala na włączenie do zakresu zgodności stron niezgodnych z wymaganiami, o ile mają one „zgodną wersję alternatywną”. Gwarantuje to, że wszystkie informacje i wszystkie funkcje, które znajdują się na stronach objętych zakresem zgodności, są dostępne na stronach internetowych zgodnych z wymogami.

[20. Zgodność z wersją alternatywną](ICT-20-wersje-alternatywne)

[Wymóg zgodności WCAG 5.2.5 Brak zakłóceń](https://www.w3.org/Translations/WCAG21-pl/#cc5): Następujące kryteria sukcesu dotyczą wszystkich treści na stronie, włącznie z treściami, które w innych przypadkach nie są podstawą spełnienia wymogów zgodności, ponieważ niezastosowanie poniższych kryteriów mogłoby uniemożliwiać korzystanie ze strony:
- 1.4.2 Kontrola odtwarzania dźwięku
- 2.1.2 Brak pułapki na klawiaturę,
- 2.3.1 Trzy błyski lub wartości poniżej progu, oraz
- 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie.

[25. Brak zakłóceń](ICT-25-brak-zaklocen)