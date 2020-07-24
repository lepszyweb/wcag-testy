---
title: 17. Multimedia zsynchronizowane


sidebar: testy_sidebar
permalink: tz-17-multimedia-zsynchronizowane
folder: testy/tz
---

## Cel procedury testowej

Celem tego zestawu testów jest sprawdzenie, czy wszyscy użytkownicy mają równy dostęp do wizualnych i dźwiękowych komponentów zsynchronizowanych mediów. Osiąga się to poprzez: (1) zsynchronizowane podpisy ścieżki dźwiękowej dla osób niesłyszących lub słabosłyszących, oraz (2) opisy dźwiękowe treści dostępnych tylko wizualnie, w tym ważnych szczegółów wizualne dla osób niewidomych lub słabowidzących. Ponadto odtwarzacz multimedialny używany do prezentacji zsynchronizowanych multimediów musi zapewniać wszystkim użytkownikom kontrolę nad napisami i opisami audio.

Procedura testowa „Multimedia zsynchronizowane” obejmuje sześć testów:

1.	Test 17.A 1.2.2-rownowazne-napisy
2.	Test 17.B 1.2.5-rownowazna-audiodeskrypcja
3.	Test 17.C 1.2.4-rownowazne-napisy-na-zywo
4.	Test 17.D 503.4-sterowanie-napisami-i-audiodeskrypcją
5.	Test 17.E 503.4.1-sterowanie-napisami
6.	Test 17.F 503.4.2-sterowanie-audiodeskrypcją


## Napisy dla niesłyszących // Równoważne napisy


### Test 17.A 1.2.2-rownowazne-napisy

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.2.2-rownowazne-napisy | 17.A    | Media mają napisy dokładnie odwzorowujące treści audio. |

### Cele testu 17.A 1.2.2-rownowazne-napisy

Celem tego testu jest ustalenie, czy dla treści audiowizualnej prezentacji medialnej zapewniono napisy, które dokładnie odwzorowują treści dźwiękowe. Testowany warunek wymaga, aby napisy poprawnie odwzorowywały treści wypowiadane przez narratora i uczestników prezentacji medialnej oraz zawierały     
ważne informacje, takie jak kto mówi, a także wszelkie znaczące dźwięki. Napisy muszą być zsynchronizowane z dźwiękiem, aby wizualne i słyszalne szczegóły były odpowiednio skorelowane.

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1.2.2
Napisy rozszerzone (nagranie)](https://wcag.lepszyweb.pl/#captions-prerecorded).

### Metody i narzędzia testowe 
1. Kontrola ręczna 
2. Inspekcja wzrokowa

<!-- Kontrola ręczna zsynchronizowanych mediów (plik audiowizualny i związane z nim podpisy).-->

### Identyfikacja treści

Wszelkie nagrane wcześniej zsynchronizowane treści multimedialne.

**Z wyłączeniem** mediów, które stanowią alternatywę dla tekstu i tak zostały wyraźnie określone.

Na przykład strona zawierająca instrukcje krok po kroku dotyczące wiązania sznurowadła może również zawierać zsynchronizowane media zawierające te same instrukcje. Zsynchronizowane media są wyraźnie oznaczone jako alternatywa tekstu przeznaczona dla użytkowników, którzy mogą uczyć się lepiej, obserwując, jak ktoś wykonuje zadanie. W takim przypadku równoważne napisy dla prezentacji medialnej   nie są wymagane, ponieważ te same instrukcje są już przedstawione w tekście na stronie.

**Uwaga**: Warunkiem jest jednak, aby prezentacja medialna została oznaczona jako alternatywa.

### Zastosowanie
Test 17.A 1.2.2-rownowazne-napisy **nie ma zastosowania** <!--, jeśli na stronie nie ma wcześniej nagranych multimediów zsynchronizowanych. --> w następujących przypadkach:

1.	gdy na stronie nie ma wcześniej nagranych multimediów zsynchronizowanych. (Nie dotyczy to treści tylko audio lub tylko wideo.)
2.	gdy zsynchronizowane media są alternatywną prezentacją informacji, które są również prezentowane na stronie internetowej w postaci tekstu i jako alternatywa są oznaczone.
3.	gdy media są transmitowane na żywo (ten przypadek objęty jest testem 17.C 1.2.4-rownowazne-napisy-na-zywo).

W takich przypadkach oznacz wynik testu jako **ND**.


**Uwaga**: Jeśli transmisja jest nagrywana, ten wymóg testowy **ma zastosowanie** do późniejszej publikacji zsynchronizowanego nagrania multimedialnego.

### Jak testować

1.  Włącz napisy za pomocą funkcji odtwarzacza multimedialnego i odtwarzaj multimedia.

    1.  Aby spełnić ten wymóg, można dostarczyć osobny plik multimedialny z napisami (tzn. wersja z napisami to inny plik). Jeśli jest dostarczony, przetestuj go. Oddzielny plik multimedialny może być osiągalny poprzez łącze lub opcję menu na stronie.

2.  Odsłuchaj dźwięk z całego medium zsynchronizowanego. Porównaj dźwięk z napisami pod względem dokładności, synchronizacji czasowej i równoważności.

    1.  Napisy powinny zawierać wszystkie wypowiedzi i ich odpowiedniki dla niedialogowych informacji audio potrzebnych do zrozumienia treści programu (np. kto mówi), w tym efektów dźwiękowych, muzyki, śmiechu, identyfikacji lokalizacji osób mówiących.

    2.  Definicja napisów obejmuje synchronizację. Jeśli nie są zsynchronizowane, nie są uważane za napisy.

    3.  Napisy nie mogą zasłaniać istotnych treści na filmie.	

### Ocena wyników

Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.2.2:

1.  Napisy są dostarczane do wszystkich treści multimedialnych **oraz**

2.  Napisy są dokładne i obejmują wszystkie dialogi i ich odpowiedniki dla nie-dialogowych informacji audio potrzebnych do zrozumienia treści programu, w tym efektów dźwiękowych, np. muzyki, śmiechu, identyfikacji i lokalizacji osób mówiących, **oraz**

3.  Wszystkie inne istotne informacje na filmie są wyraźnie widoczne (nie są zasłonięte napisami), gdy napisy są włączone.


### Uwaga

-  Dokładność napisów może często zależeć od tego, jak dobrze są zsynchronizowane z prezentacją audiowizualną; nie powinno być żadnych różnic czasowych między informacjami prezentowanymi dźwiękiem a treścią odpowiadających im napisów.

-  Same transkrypcje i niezsynchronizowane alternatywy nie spełniają wymogów tego testu.

## Audiodeskrypcja (Opisy dźwiękowe)

### Test 17.B 1.2.5-rownowazna-audiodeskrypcja

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.2.5-rownowazna-audiodeskrypcja | 17.B    | Multimedia zapewniają równoważną ścieżkę dźwiękową (połączenie narracji i opisów audio) dla treści wideo. |

## Cel testu 17.B 1.2.5-rownowazna-audiodeskrypcja

Celem testu jest ustalenie, czy informacje wizualne w zsynchronizowanej prezentacji medialnej są dostępne również dla osób niewidomych lub słabowidzących. Aby osoby niewidome i słabowidzące skorzystały z prezentacji medialnej może być konieczna narracja dźwiękowa przedstawiająca istotne treści wizualne, które nie są odpowiednio opisane w głównej ścieżce dźwiękowej. 
Celem tego testu jest sprawdzenie, czy ważne dla zrozumienia informacje wizualne, takie, jak co dokładnie się dzieje na ekranie, jak wygląda miejsce akcji, jak zachowują się bohaterowie i inne zdarzenia wizualne, których osoby niewidome i słabowidzące nie są w stanie samodzielnie zobaczyć, są przekazywane w dodatkowej ścieżce dźwiękowej.

<!-- Informacjami ważnymi dla zrozumienia treści wizualnych są informacje o tym, co dokładnie dzieje się na ekranie, co widać na ekranie, jak wygląda miejsce akcji, jak wyglądają bohaterzy, ich mimika, gestykulacja i inne zdarzenia wizualne, których osoby niewidome i słabowidzące nie są w stanie samodzielnie zobaczyć. -->

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1.2.5 Audiodeskrypcja (nagranie)](https://wcag.lepszyweb.pl/#captions-prerecorded).
 
### Metody i narzędzia testowe 
1. Inspekcja ręczna zsynchronizowanych mediów (plik audio-wideo i powiązane z nim opisy audio). Może to również obejmować osobny plik multimedialny, który zawiera opis audio.

### Identyfikacja treści
Wszelkie nagrane wcześniej zsynchronizowane treści multimedialne.

**Uwaga**: Transkrypcja zsynchronizowanego pliku multimedialnego nie spełnia tego wymagania i nie jest częścią testowanej treści.


### Zastosowanie
Test 17.B 1.2.5-rownowazna-audiodeskrypcja **nie ma zastosowania** <!--, jeśli na stronie nie ma wcześniej nagranych multimediów zsynchronizowanych. --> w następujących przypadkach:


1.	gdy na stronie nie ma wcześniej nagranych multimediów zsynchronizowanych. (Nie dotyczy to treści tylko audio lub tylko wideo.)
2.	gdy zsynchronizowane media są alternatywną prezentacją informacji, które są również prezentowane na stronie internetowej w postaci tekstu i jako alternatywa są oznaczone.
3.	gdy media są transmitowane na żywo (ten przypadek objęty jest testem 17.C 1.2.4-rownowazne-napisy-na-zywo).

W takich przypadkach oznacz wynik testu jako **ND**.

### Jak testować

1. Włącz audiodeskrypcję za pomocą odtwarzacza multimedialnego i odtwarzaj multimedia.

    1.  Audiodeskrypcja to narracja dodana do ścieżki dźwiękowej lub połączona z nią w celu opisania ważnych szczegółów wizualnych, których nie można zrozumieć na podstawie samej ścieżki dźwiękowej.

    2.  Aby spełnić ten wymóg, można dostarczyć osobny plik multimedialny z audiodeskrypcją (tzn. plik multimedialny z audiodeskrypcją jest innym plikiem). Jeśli taki plik jest dostarczony, należy go przetestować.

2.  Określ treści wizualne wymagające opisów dźwiękowych.

3. Ustal, czy główna ścieżka dźwiękowa w połączeniu z audiodeskrypcją odpowiednio opisują ważne szczegóły wizualne (działania, postacie, zmiany scen, tekst na ekranie itp.) dla widza, który nie jest w stanie zobaczyć treści.

    1.  Jeśli główna ścieżka dźwiękowa odpowiednio opisuje ważne treści widoczne na nagraniu, w tym działania, postacie, zmiany scen, teksty na ekranie, lokalizację osób mówiących oraz inne treści wizualne, dodatkowy opis audio nie jest konieczny.

4.  Porównaj obraz wideo z dołączoną ścieżką dźwiękową i sprawdź, czy jest ona dokładna, zsynchronizowana czasowo i równoważna.

    1.  Opisy audio są wstawiane w przerwach w oknie dialogowym. Synchronizacja może nie być możliwa, ale opis należy podać tak szybko, jak to możliwe, aby znaczenie zostało zachowane.

### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.2.5:

1.  Ścieżka dźwiękowa (połączenie opisów audio i narracji) odpowiednio opisuje ważne treści wizualne w medium, w tym informuje o działaniach, postaciach, zmianach scen, tekście na ekranie i innych treściach wizualnych.

### Uwaga

-  Same transkrypcje i niezsynchronizowane alternatywy nie spełniają tego wymogu.

## Media synchronizowane na żywo

### Test 17.C 1.2.4-rownowazne-napisy-na-zywo

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.2.4-rownowazne-napisy-na-zywo | 17.C    | Multimedia na żywo zawierają napisy dokładnie odwzorowujące treści audio. |

### Cel testu
Celem tego testu jest ustalenie, czy dla zsynchronizowanych mediów transmitowanych na żywo w czasie rzeczywistym, zapewnione są równoważne napisy, które dokładnie odwzorowują treści dźwiękowe, w tym wypowiedzi, tożsamość mówców, efekty dźwiękowe i inne znaczące treści audio.

Ma to zapewnić, że treść mediów transmitowanych w czasie rzeczywistym jest dostępna dla osób niesłyszących lub słabosłyszących.

Podczas transmisji na żywo może być niemożliwa poważna redakcja napisów, aby zapewnić poprawność i dokładność (pisowni, interpunkcji, identyfikacji osób mówiących itp.). Błędy napisów, które nie powodują utraty zrozumienia zsynchronizowanych treści multimedialnych na żywo, są dopuszczalne. Bardziej krytyczna weryfikacja jakości napisów powinna zostać wykonana w przypadku ponownego nadawania nagrania, ponieważ nie będzie ono wtedy uważane za prezentowane „na żywo”.

Dla testera wykonującego testy w realnym świecie dokładne udokumentowanie błędów w napisach podczas transmisji „na żywo” jest szczególnym wyzwaniem.

Zidentyfikuj synchronizowane treści multimedialne na żywo. Te wymagania są przeznaczone wyłącznie do emisji (nadawania) zsynchronizowanych treści multimedialnych.

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1.2.4
Napisy rozszerzone](https://wcag.lepszyweb.pl/#captions-live).


### Metody i narzędzia testowe 
1. Inspekcja wzrokowa i słuchowa napisów związanych z transmisją internetową lub transmisją na żywo.

### Identyfikacja treści
Wszelkie transmisje na żywo lub webcasty.

### Zastosowanie
Test 17.C 1.2.4-rownowazne-napisy-na-zywo **nie ma zastosowania** w przypadkach:

- jeśli na stronie nie ma mediów prezentowanych na żywo,
- wcześniejsza prezentacja na żywo jest ponownie odtwarzana (jest wcześniej nagrana),
- połączeń multimedialnych między dwiema lub więcej osobami za pośrednictwem aplikacji internetowych.

### Jak testować

1.  Włącz napisy za pomocą funkcji odtwarzacza multimedialnego.

2. Odsłuchaj dźwięk zsynchronizowanego medium. Porównaj dźwięk z napisami, aby sprawdzić jego dokładność, synchronizację czasową i równoważność.

    1.  Mniejsza dokładność napisów w transmisjach na żywo może być akceptowalna ze względu na ograniczenia możliwości redagowania napisów w czasie rzeczywistym.

    2.  Definicja napisów obejmuje synchronizację. Jeśli nie są one zsynchronizowane, nie są one uznawane za napisy.

### Ocena wyników

Jeśli wszystkie twierdzenia poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.2.4:

1.  Napisy są dostarczane do wszystkich multimediów na żywo **oraz**

2.  Wszystkie napisy są dokładne, **oraz**

3.  Wszelkie rozbieżności pomiędzy napisami a wyjściem audio są niewielkie i nie wpływają znacząco na zrozumienie (dotyczy tylko napisów na żywo).

## Sterowanie multimediami

### Test 17.D 503.4-sterowanie-napisami-i-audiodeskrypcją

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 503.4-sterowanie-napisami-i-audiodeskrypcją | 17.D    | Odtwarzacz multimedialny zapewnia kontrolę użytkownika nad zamkniętymi napisami i audiodeskrypcją. |

### Cel testu 

Celem testu jest sprawdzenie, czy w przypadku, gdy do prezentacji zsynchronizowanych multimediów używany jest odtwarzacz multimediów, użytkownicy mają do dyspozycji elementy, takie jak łącza lub przyciski, za pomocą których mogą kontrolować wyświetlanie napisów i odtwarzanie audiodeskrypcji.  

Wyniki tego testu służą do ustalenia, czy spełniony jest punkt 503.4. Wymaganie techniczne dotyczące kontroli użytkownika nad napisami i opisami dźwiękowymi (oprogramowanie rozdział 5, aplikacje 503) Sekcji 508.


### Metody i narzędzia testowe 
1. Inspekcja wzrokowa strony.

### Identyfikacja treści
Każdy odtwarzacz multimedialny używany do wyświetlania zsynchronizowanych treści wideo i audio.

### Zastosowanie

Test 17.D 503.4-sterowanie-napisami-i-audiodeskrypcją **nie ma zastosowania**, eśli nie ma odtwarzacza multimedialnego lub odtwarzacz multimedialny NIE wyświetla wideo zsynchronizowanego z dźwiękiem (tzn. wyświetla tylko dźwięk lub tylko wideo). W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Znajdź elementy sterujące wyborem (włączaniem i wyłączaniem) napisów zamkniętych i audiodeskrypcji.

   **Uwaga**: Użytkownik musi mieć możliwość aktywowania kontrolki (wybrania, włączenia). Nieaktywna kontrolka (której nie można wybrać, włączyć), nie spełnia tego wymagania.
   
   Ten test dotyczy tylko i wyłącznie opcji odtwarzacza multimedialnego, a nie treści multimedialnych. Nie ma więc dla oceny wyników testu znaczenia, że zsynchronizowane audio i wideo mają napisy otwarte lub otwartą audiodeskrypcję i nie jest konieczne ich uaktywnianie. Standardy Sekcji 508 nadal wymagają kontroli użytkownika nad napisami i opisami audio w odtwarzaczu multimedialnym. 


### Ocena wyników
Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;wymaganiem 503.4 Sekcji 508:

1.  Odtwarzacz multimedialny zapewnia kontrolę użytkownika nad zamkniętymi napisami i opisami dźwiękowymi.

## Odtwarzacz multimedialny - sterowanie napisami

### Test 17.E 503.4.1-lokalizacja-kontrolki-napisow

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 503.4.1-lokalizacja-kontrolki-napisow | 17.E    | Kontrolki użytkownika dla napisów są dostępne na tym samym poziomie menu, co kontrolki użytkownika dotyczące wyboru głośności lub programu. |

### Cel testu 17.E 503.4.1-lokalizacja-kontrolki-napisow

Celem tego testu jest sprawdzenie, czy w przypadku, gdy zapewniony jest odtwarzacz multimediów z regulacją głośności, kontrolki sterujące napisami w odtwarzaczu multimediów znajdują się na tym samym poziomie menu, co elementy regulacji głośności lub wyboru programu. 

Dzięki temu użytkownicy korzystający z napisów mogą łatwo znaleźć kontrolkę. 

Wyniki tego testu służą do ustalenia, czy spełniony jest punkt 503.4.1 Wymaganie techniczne dotyczące kontroli użytkownika nad napisami (oprogramowanie rozdział 5, aplikacje 503) Sekcji 508.


### Metody i narzędzia testowe 
1. Inspekcja wzrokowa strony.

### Identyfikacja treści
Każdy odtwarzacz multimedialny używany do wyświetlania zsynchronizowanych treści wideo i audio.

### Zastosowanie

Test 17.E 503.4.1-lokalizacja-kontrolki-napisow **nie ma zastosowania**, jeśli nie ma odtwarzacza multimedialnego lub odtwarzacz nie ma funkcji regulacji głośności. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Kontynuuj test 17.D. Znajdź element sterujący wyborem  napisów zamkniętych.

    Jeśli nie ma kontrolki umożliwiającej użytkownikowi wybór napisów lub nie można jej aktywować, ten test kończy się niepowodzeniem. Pamiętaj, że kontrolka użytkownika z definicji musi zapewniać możliwość aktywacji / wyboru.

2.  Znajdź elementy sterujące użytkownika do wyboru głośności i wyboru programu.

3.  Porównaj poziom menu kontrolki wyboru napisów zamkniętych z poziomem menu regulacji głośności lub menu wyboru programu.

    **Uwaga**: Wybór programu to funkcja odtwarzacza multimedialnego, która umożliwia użytkownikowi wybór prezentacji lub części dłuższej prezentacji do odtworzenia. Wybór programu jest zwykle taki sam, jak w przypadku otwierania pliku lub korzystania z interaktywnego spisu treści. Elementy sterujące multimediami służące do wyświetlania otwartego pliku (odtwarzanie, pauza, szybkie przewijanie do przodu, przewijanie do tyłu itp.) **nie** są uważane za elementy sterujące wyborem programu. W większości implementacji internetowych odtwarzacze multimediów są zazwyczaj dostarczane do przeglądania określonych zsynchronizowanych multimediów, więc elementy sterujące wyborem programu do otwierania dowolnego pliku nie są powszechne. Można zapewnić kontrolę wyboru programu, aby przejść do określonych tematów w mediach (czasami określanych jako „rozdziały”). Kontrolka głośności jest traktowana jako unikalna kontrolka, różna od kontrolki wyboru programu.



### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;wymaganiem 503.4.1 Sekcji 508:

1.  Kontrolki sterowania napisami są dostępne na tym samym poziomie menu, co elementy sterowania głośnością lub wyboru programu.



## Odtwarzacz multimedialny - sterowanie audiodeskrypcją

### Test 17.F 503.4.2-lokalizacja-kontrolki-audiodeskrypcji

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 503.4.2-lokalizacja-kontrolki-audiodeskrypcji | 17.F    | Kontrolki użytkownika dla audiodeskrypcji są dostępne na tym samym poziomie menu, co kontrolki użytkownika do wyboru programu lub głośności. |

### Cel testu 

Celem tego testu jest sprawdzenie, czy w przypadku, gdy zapewniony jest odtwarzacz multimediów z elementami sterującymi wyborem programu lub regulacji głośności, kontrolki sterujące audiodeskrypcją w odtwarzaczu multimediów znajdują się na tym samym poziomie menu, co elementy regulacji głośności lub wyboru programu.

Dzięki temu użytkownicy korzystający z audiodeskrypcji mogą łatwo znaleźć kontrolkę.  

Wyniki tego testu służą do ustalenia, czy spełniony jest punkt 503.4.2 Wymaganie techniczne dotyczące kontroli użytkownika nad napisami (oprogramowanie rozdział 5, aplikacje 503) Sekcji 508.

### Metody i narzędzia testowe 
1. Inspekcja wzrokowa strony.

### Identyfikacja treści
Każdy odtwarzacz multimedialny używany do wyświetlania zsynchronizowanych treści wideo i audio.

### Zastosowanie

Test 503.4.2-lokalizacja-kontrolki-audiodeskrypcji **nie ma zastosowania**, jeśli nie ma odtwarzacza multimedialnego lub odtwarzacz nie ma funkcji wyboru programu lub regulacji głośności. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Kontynuuj test 17.D. Znajdź element sterujący wyborem audiodeskrypcji.

    Jeśli nie ma kontrolki umożliwiającej użytkownikowi wybór audiodeskrypcji lub nie można jej aktywować, ten test kończy się niepowodzeniem. Pamiętaj, że kontrolka użytkownika z definicji musi zapewniać możliwość aktywacji / wyboru.

2.  Znajdź elementy sterujące użytkownika do wyboru głośności i wyboru programu.

3.  Porównaj poziom menu kontrolki wyboru audiodeskrypcji z poziomem menu regulacji głośności lub menu wyboru programu.


    **Uwaga**: Wybór programu to funkcja odtwarzacza multimedialnego, która umożliwia użytkownikowi wybór prezentacji lub części dłuższej prezentacji do odtworzenia. Wybór programu jest zwykle taki sam, jak w przypadku otwierania pliku lub korzystania z interaktywnego spisu treści. Elementy sterujące multimediami służące do wyświetlania otwartego pliku (odtwarzanie, pauza, szybkie przewijanie do przodu, przewijanie do tyłu itp.) **nie** są uważane za elementy sterujące wyborem programu. W większości implementacji internetowych odtwarzacze multimediów są zazwyczaj dostarczane do przeglądania określonych zsynchronizowanych multimediów, więc elementy sterujące wyborem programu do otwierania dowolnego pliku nie są powszechne. Można zapewnić kontrolę wyboru programu, aby przejść do określonych tematów w mediach (czasami określanych jako „rozdziały”). Kontrolka głośności jest traktowana jako unikalna kontrolka, różna od kontrolki wyboru programu.

### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;wymaganiem 503.4.2 Sekcji 508:

1.  Elementy sterujące audiodeskrypcją znajdują się na tym samym poziomie menu, co elementy sterowania głośnością lub wyboru programu.



### Obowiązujące normy

{% include ks/1-2-2.md %}
{% include ks/1-2-4.md %}
{% include ks/1-2-5.md %}

[*Section 508 503.4.1 Sterowanie napisami*](https://www.access-board.gov/guidelines-and-standards/communications-and-it/about-the-ict-refresh/final-rule/text-of-the-standards-and-guidelines#503-applications): Jeżeli do regulacji głośności przez użytkownika służą elementy sterujące, technologia zapewnia elementy sterujące wyborem napisów na tym samym poziomie menu, co elementy sterujące wyborem przez użytkownika głośności lub programu.


[*Section 508 503.4.2 Sterowanie audiodeskrypcją*](https://www.access-board.gov/guidelines-and-standards/communications-and-it/about-the-ict-refresh/final-rule/text-of-the-standards-and-guidelines#503-applications): Jeżeli do wyboru programu przez użytkownika przewidziano elementy sterujące, technologia zapewnia elementy sterujące wyborem opisów dźwiękowych na tym samym poziomie menu, co elementy sterujące wyborem przez użytkownika głośności lub programu.

[17. Media zsynchronizowane](ICT-17-media-zsynchronizowane)

                                                                                                                
