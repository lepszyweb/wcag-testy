---
title: 17. Miltimedia zsynchronizowane


sidebar: testy_sidebar
permalink: tz-17-multimedia-zsynchronizowane
folder: testy/tz
---

## Nagrane multimedia zsynchronizowane

### Identyfikacja treści

Zidentyfikuj wszelkie nagrane wcześniej zsynchronizowane treści multimedialne.

**WYKLUCZ** media, które stanowią (są) wyraźnie alternatywę dla tekstu.

Jeżeli nie ma takiej treści, to wynikiem dla testów 17.A oraz 17.B jest **NIE MA ZASTOSOWANIA** 

#### Test 1.2.2-rownowazne-napisy

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.2.2-rownowazne-napisy | 17.A    | Media mają napisy dokładnie odwzorowujące treści audio. |

#### Zastosowanie

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli na stronie nie ma wcześniej nagranych multimediów zsynchronizowanych

#### Jak testować

1.  Włącz napisy za pomocą funkcji odtwarzacza multimedialnego i odtwarzaj multimedia.

    1.  Aby spełnić ten wymóg, można dostarczyć osobny plik multimedialny z napisami (tzn. wersja z napisami to inny plik). Jeśli jest dostarczony, przetestuj go.

2.  Odsłuchaj dźwięk z całego medium zsynchronizowanego. Porównaj dźwięk z napisami pod względem dokładności, synchronizacji czasowej i równoważności.

    1.  Napisy powinny zawierać wszystkie dialogi i ich odpowiedniki dla niedialogowych informacji audio potrzebnych do zrozumienia treści programu, w tym efektów dźwiękowych, muzyki, śmiechu, identyfikacji lokalizacji osób mówiących.

    2.  Definicja napisów obejmuje synchronizację. Jeśli nie są zsynchronizowane, nie są uważane za napisy.

    3.  Napisy nie mogą zasłaniać istotnych treści na filmie.	
	
### Ocena wyników

Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, then the Warunek testowy is **TRUE** and the content **PASSES**:

1.  Napisy są dostarczane do wszystkich treści multimedialnych, ORAZ

2.  Napisy są dokładne i obejmują wszystkie dialogi i ich odpowiedniki dla nie-dialogowych informacji audio potrzebnych do zrozumienia treści programu, w tym efektów dźwiękowych, np. muzyki, śmiechu, identyfikacji i lokalizacji osób mówiących, ORAZ

3.  Wszystkie inne istotne informacje na filmie są wyraźnie widoczne (nie są zasłonięte napisami), gdy napisy są włączone.


### Uwaga

-  Same transkrypcje i niezsynchronizowane alternatywy nie spełniają tego wymogu.

### Test 1.2.5-rownowazna-audiodeskrypcja

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.2.5-rownowazna-audiodeskrypcja | 17.B    | Multimedia zapewniają równoważną ścieżkę dźwiękową (połączenie narracji i opisów audio) dla treści wideo. |


### Zastosowanie

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli na stronie nie ma wcześniej nagranych multimediów zsynchronizowanych

### Jak testować

1. Włącz audiodeskrypcję za pomocą odtwarzacza multimedialnego i odtwarzaj multimedia.

    1.  Audiodeskrypcja to narracja dodana do ścieżki dźwiękowej lub połączona z nią w celu opisania ważnych szczegółów wizualnych, których nie można zrozumieć na podstawie samej ścieżki dźwiękowej.

    2.  Aby spełnić ten wymóg, można dostarczyć osobny plik multimedialny z audiodeskrypcją (tzn. plik multimedialny z audiodeskrypcją jest innym plikiem). Jeśli taki plik jest dostarczony, należy go przetestować.

2.  Zidentyfikuj treści wizualne wymagające opisów narracyjnych.

3. Ustal, czy główna ścieżka dźwiękowa w połączeniu z opisami audio odpowiednio opisują ważne szczegóły wizualne (działania, postacie, zmiany scen, tekst na ekranie itp.) dla widza, który nie jest w stanie zobaczyć treści.

    1.  Jeśli główna ścieżka dźwiękowa odpowiednio opisuje ważne treści wizualne w mediach, w tym informacje o działaniach, postaciach, zmianach scen, tekstach ekranowych, identyfikacji i lokalizacji osób mówiących oraz inne treści wizualne, dodatkowy opis audio nie jest konieczny.

4.  Porównaj obraz wideo z połączoną ścieżką dźwiękową i sprawdź, czy jest ona dokładna, zsynchronizowana czasowo i równoważna.

    1.  Opisy audio są wstawiane w przerwach w oknie dialogowym. Synchronizacja może nie być możliwa, ale opis należy podać tak szybko, jak to możliwe, aby znaczenie zostało zachowane.
	
### Ocena wyników

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, then the content **PASSES**:

1.  Ścieżka dźwiękowa (połączenie opisów audio i narracji) adekwatnie opisuje ważne treści wizualne w mediach, w tym informuje o działaniach, postaciach, zmianach scen, tekście na ekranie i innych treściach wizualnych.


### Uwaga

-  Same transkrypcje i niezsynchronizowane alternatywy nie spełniają tego wymogu.

## Media synchronizowane na żywo

### Identyfikacja treści

Zidentyfikuj synchronizowane treści multimedialne na żywo. Te wymagania są przeznaczone wyłącznie do emisji (nadawania) zsynchronizowanych treści multimedialnych.

**WYKLUCZ** dwukierunkowe połączenia multimedialne między dwiema lub więcej osobami za pośrednictwem aplikacji internetowych.

Jeśli nie ma takiej treści, wynik dla następujących identyfikatorów testów **NIE MA ZASTOSOWANIA**: 17.C.

### Test 1.2.4-rownowazne-napisy-na-zywo

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.2.4-rownowazne-napisy-na-zywo | 17.C    | Multimedia na żywo zawierają napisy dokładnie odwzorowujące treści audio. |
 

### Zastosowanie

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli nie istnieją media synchronizowane na żywo.

### Jak testować

1.  Włącz napisy za pomocą funkcji odtwarzacza multimedialnego.

2. Odsłuchaj dźwięk zsynchronizowanego medium. PPorównaj dźwięk z napisami, aby sprawdzić jego dokładność, synchronizację czasową i równoważność.

    1.  Mniejsza dokładność napisów w transmisjach na żywoo może być akceptowalna ze względu na ograniczenia możliwości napisów w czasie rzeczywistym.

    2.  Definicja napisów obejmuje synchronizację. Jeśli nie są one zsynchronizowane, nie są one uznawane za napisy.
	
### Ocena wyników

Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, then the content **PASSES**:

1.  Napisy są dostarczane do wszystkich multimediów na żywo ORAZ

2.  Wszystkie napisy są dokładne, ORAZ

3.  Wszelkie rozbieżności pomiędzy podpisami a wyjściem audio są niewielkie i nie wpływają znacząco na zrozumienie (dotyczy tylko napisów na żywo).


## Kontrolki odtwarzacza multimedialnego

### Identyfikacja treści

Zidentyfikuj dowolny odtwarzacz multimedialny używany do wyświetlania zsynchronizowanych treści wideo i audio.

Jeśli nie ma takiej treści, wynik dla następujących identyfikatorów testów **NIE MA ZASTOSOWANIA**: 17.D to 17.F.

### Test 503.4-kontrolki-napisow-i-audiodeskrypcji

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 503.4-kontrolki-napisow-i-audiodeskrypcji | 17.D    | Odtwarzacz multimedialny zapewnia kontrolę użytkownika nad zamkniętymi napisami i audiodeskrypcją. |

### Zastosowanie

Ten warunek testowy **NIE MA ZASTOSOWANIA** jeśli nie ma odtwarzacza multimedialnego lub odtwarzacz multimedialny NIE wyświetla wideo zsynchronizowanego z dźwiękiem (tzn. wyświetla tylko dźwięk lub tylko wideo).

### Jak testować

1.  Znajdź elementy sterujące do wyboru zamkniętych napisów i audiodeskrypcji.

### Ocena wyników

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, then the content **PASSES**:

1.  Odtwarzacz multimedialny zapewnia kontrolę użytkownika nad zamkniętymi napisami i opisami dźwiękowymi.

## Odtwarzacz multimedialny - elementy sterujące napisami na poziomie menu głośności

### Identyfikacja treści

Zidentyfikuj dowolny odtwarzacz multimedialny z elementami sterującymi regulacją głośności.

Jeśli nie ma takiej treści, wynik dla następujących identyfikatorów testów **NIE MA ZASTOSOWANIA**: 17.E.

### Test 503.4.1-kontrolki-napisow

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 503.4.1-kontrolki-napisow | 17.E    | Kontrolki użytkownika dla napisów są dostępne na tym samym poziomie menu, co kontrolki użytkownika dotyczące wyboru głośności lub programu. |

### Zastosowanie

Ten warunek testowy **NIE MA ZASTOSOWANIA** jeśli nie ma odtwarzacza multimediów lub odtwarzacz nie ma regulacji głośności.

### Jak testować

1.  Kontynuuj test 17.D.

2.  Znajdź elementy sterujące użytkownika do wyboru głośności i wyboru programu.

### Ocena wyników

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, then the content **PASSES**:

1.  Elementy sterowania użytkownika napisami są dostępne na tym samym poziomie menu, co elementy sterowania głośnością lub wyboru programu.

## Odtwarzacz multimedialny - sterowanie audiodeskrypcją na poziomie menu programu

### Identyfikacja treści

Zidentyfikuj dowolny odtwarzacz multimedialny za pomocą kontroli wyboru programu.

> ** Uwaga: ** Wybór programu to funkcja odtwarzacza multimedialnego, która umożliwia użytkownikowi wybór prezentacji lub części dłuższej prezentacji do odtworzenia. Wybór programu jest zazwyczaj taki sam, jak w przypadku otwierania pliku lub korzystania ze spisu treści. Elementy sterujące multimediami służące do wyświetlania otwartego pliku (odtwarzanie, pauza, szybkie przewijanie do przodu, przewijanie do tyłu itp.) NIE są uważane za elementy sterujące wyborem programu.

> W większości implementacji internetowych odtwarzacze multimediów są zazwyczaj dostarczane do przeglądania określonych zsynchronizowanych multimediów, więc elementy sterujące wyborem programu do otwierania dowolnego pliku nie są powszechne. Można zapewnić kontrolę wyboru programu, aby przejść do określonych tematów w mediach (czasami określanych jako „rozdziały”). Kontrola głośności jest traktowana jako unikalna kontrola, różna od kontroli wyboru programu.


Jeśli nie ma takiej treści, wynik dla następujących identyfikatorów testów **NIE MA ZASTOSOWANIA**: 17.F.

### Test 503.4.2-kontrolki-audiodeskrypcji

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 503.4.2-kontrolki-audiodeskrypcji | 17.F    | Kontrolki użytkownika dla audiodeskrypcji są dostępne na tym samym poziomie menu, co kontrolki użytkownika do wyboru programu lub głośności. |

### Zastosowanie

Ten warunek testowy **NIE MA ZASTOSOWANIA** jeśli nie ma odtwarzacza multimedialnego lub odtwarzacz multimedialny nie ma kontrolek wyboru programu.

### Jak testować

1.  Kontynuuj test 17.D.

2.  Znajdź elementy sterujące użytkownika do wyboru programu i głośności.

### Ocena wyników

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, then the content **PASSES**:

1.  Elementy sterujące dla opisów audio znajdują się na tym samym poziomie menu, co elementy sterujące wyborem programu lub głośność.

### Zastosowane standardy

{% include ks/1-2-2.md %}

[*Section 508 503.4.1 Sterowanie napisami*](https://www.access-board.gov/guidelines-and-standards/communications-and-it/about-the-ict-refresh/final-rule/text-of-the-standards-and-guidelines#503-applications): Jeżeli do regulacji głośności służą elementy sterujące użytkownika, technologia zapewnia elementy sterujące wyborem napisów na tym samym poziomie menu, co elementy sterujące wyborem przez użytkownika głośności lub programu.


[*Section 508 503.4.2 Sterowanie audiodeskrypcją*](https://www.access-board.gov/guidelines-and-standards/communications-and-it/about-the-ict-refresh/final-rule/text-of-the-standards-and-guidelines#503-applications): Jeżeli do wyboru programu przewidziano elementy sterujące użytkownika, technologia zapewnia sterujące wyborem opisów dźwiękowych na tym samym poziomie menu, co elementy sterujące wyborem przez użytkownika głośności lub programu.

[17. Media zsynchronizowane](ICT-17-media-zsynchronizowane)

                                                                                                                
