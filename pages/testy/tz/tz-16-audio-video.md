---
title: 16. Tylko audio, tylko wideo i animacje


sidebar: testy_sidebar
permalink: tz-16-audio-video
folder: testy/tz
---
## Cel scenariusza testowego 

Celem tego zestawu testów jest sprawdzenie, czy informacje prezentowane w nagranym pliku audio są również prezentowane w równoważnej wersji tekstowej oraz czy cała nagrana treść wideo jest udostępniana w ekwiwalentnej  postaci (alternatywa tekstowa lub audiodeskrypcja). 

Gdy dostępna jest alternatywa dla wcześniej nagranych mediów audio lub wideo, to sprawia, że informacje są dostępne, ponieważ alternatywę można odwzorować za pomocą różnych trybów sensorycznych, takich jak wzrokowy, słuchowy czy dotykowy, aby dopasować je do potrzeb użytkownika. Jest to korzystne dla osób niewidomych, słabowidzących, z ograniczeniami słuchu, a także z ograniczonymi zdolnościami językowymi, poznawczymi i trudnościami w uczeniu się. 


Ten zestaw obejmuje dwa testy:
1.	Transkrypcje nagrań dźwiękowych - Test 16.A 1.2.1-transkrypcja-audio
2.	Alternatywy nagrań wideo - Test 16.B 1.2.1-odpowiedniki-wideo

## Nagrania dźwiękowe


### Test 16.A: 1.2.1-transkrypcja-audio

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.2.1-transkrypcja-audio | 16.A    | Dostępna jest alternatywa tekstowa dla nagrań dźwiękowych (tylko audio), która zapewnia dokładne i pełne przedstawienie treści nagrania. |

### Cel testu 16.A: 1.2.1-transkrypcja-audio

Celem tego testu jest sprawdzenie, czy dla nagrań dźwiękowych (tylko audio), która zapewnia dokładne i pełne przedstawienie treści nagrania. Dzięki temu osoby, które nie są w stanie usłyszeć treści dźwiękowych mogą uzyskać dostęp do informacji przedstawionych w alternatywnej postaci. 

Transkrypcja musi zawierać dokładne i pełne przedstawienie istotnych treści dźwiękowych, w tym -  oprócz dialogów - dźwięków tła. Istotne treści dźwiękowe to np. trzaskanie drzwiami, zawodzenie syren, a także identyfikacja każdego mówcy w dialogu. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-2-1 I1.2.1
Tylko audio lub tylko wideo (nagranie)
](https://wcag.lepszyweb.pl/#audio-only-and-video-only-prerecorded).

### Metody i narzędzia testowe 
Inspekcja ręczna strony

### Identyfikacja treści

Wszystkie nagrane wcześniej treści zawierajace tylko dźwięk.

   **Uwaga**: Treść zawierająca tylko dźwięk jest definiowana jako prezentacja oparta na czasie, która zawiera wyłącznie dźwięk (bez wideo i bez interakcji).

**z wyjątkiem** treści dźwiękowych, które:

-   są wyraźnie oznaczone jako medialna alternatywa dla tekstu, **lub*

-   składają się z krótkich dźwięków używanych do sygnalizowania użytkownikowi zdarzeń  systemowych, takich jak sygnały potwierdzające i powiadomienia o błędach.

**Uwagi**: 

- Medialne alternatywy dla tekstu to media, które nie zawierają więcej informacji niż te, które są już przedstawione w tekście (bezpośrednio lub za pomocą tekstow alternatywnych). Treść zawierająca tylko dźwięk może być alternatywą medialną dla samej zawartości wideo, na przykład wideo w języku migowym.

-   Jeśli audio jest *zsynchronizowane* z dowolnymi elementami wizualnymi, takimi jak obraz, wideo, slajdy, animacje lub inne media wizualne oparte na czasie, skorzystaj z testów mediów zsynchronizowanych  w sekcji [17. Miltimedia zsynchronizowane](tz-17-multimedia-zsynchronizowane).

### Zastosowanie:

Test 16.A: 1.2.1-transkrypcja-audio **nie ma zastosowania**, jeśli na stronie internetowej nie ma wcześniej nagranych prezentacji tylko-audio.

### Jak testować:

1.  Ustal, czy do każdej treści zawierającej tylko dźwięk dołączona jest transkrypcja.

    1.  Ustal, czy każda transkrypcja jest tekstem (tzn. obraz z tekstem transkrypcji nie wystarczy do zaliczenia tego testu).


   **Uwaga**: Transkrypcja musi być tekstem i nie może być obrazem tekstu. Jednym ze sposobów ustalenia, czy transkrypcja jest tekstem, jest użycie urządzenia wskazującego (takiego jak mysz), albo klawiatura czy polecenia dyktowania, aby zaznaczyć fragment tekstu w transkrypcji. Jeśli można zaznaczyć fragmenty tekstu, transkrypcja jest tekstem.
   
2.  Odtwarzaj treść audio podczas przeglądania transkrypcji.

3.  Ustal, czy informacje w transkrypcji są dokładne, w poprawniej kolejności i czy zawierają pełną reprezentację treści tylko audio.

    1.  Aby zapewnić pełną reprezentację treści, transkrypcja musi także opisywać odpowiednie dźwięki oprócz dialogu, takie jak trzaskanie drzwiami, zawodzenie syren, identyfikacja mówców w dialogu itp.
	
	2. Jeśli audio zawiera wypowiedzi wielu osób, sprawdź, czy transkrypcja określa w każdym przypadku, kto mówi.



Aby ustalić, czy dźwięk jest „znaczący”, tester powinien zapytać:

-	Czy ten dźwięk dodaje do treści istotne informacje lub wskazówki? Niektóre dźwięki przyczyniają się do ustawienia sceny lub dodania dodatkowych wyjaśnień do narracji czy dialogu. W tych przypadkach dźwięk jest istotny i powinien zostać uwzględniony w transkrypcji.

-	Czy użytkownik straciłby jakieś informacje, gdyby dźwięk nie został uwzględniony w transkrypcji? Jeśli odpowiedź brzmi „tak”, dźwięk jest istotny i powinien zostać uwzględniony w transkrypcji.

-	Czy dźwięk jest nieistotnym klipem audio? Chociaż nie jest wymagane dołączanie do transkrypcji dźwięków, które nie mają znaczenia (np. muzyka odtwarzana w tle), należy uwzględnić odpowiednie dźwięki. Przykładem, w którym muzyka jest istotna i musi być uwzględniona w transkrypcji, może być np. piosenka „Jailhouse Rock” słyszana podczas wywiadu z wykonawcą, Elvisem Presleyem. **Wskazówka**: jeśli nie masz pewności, czy dźwięk jest istotny, rozsądne jest przyjąć, że powinien być uwzględniony.


### Wyniki oceny

Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.2.1:

1.  Transkrypcja tekstowa jest dostępna dla wszystkich treści tylko audio **oraz**

2.  Transkrypcja jest dokładną i kompletną prezentacją treści tylko audio.

## Alternatywy nagrań wideo

### Test 16.B 1.2.1-odpowiedniki-wideo

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.2.1-odpowiedniki-wideo | 16.B    | Dokładne i pełne przedstawienie treści nagrania tylko-wideo dostępne jest również w postaci równoważnej alternatywy tekstowej lub dźwiękowej. |

### Cel testu 1.2.1-odpowiedniki-wideo 

Celem tego testu jest sprawdzenie, czy treści nagrań tylko wideo (np. niemego filmu, animacji) są opatrzone równoważną alternatywę tekstową lub dźwiękową:

-	**Transkrypcją**, która zapewnia tekst równoważny z tym, co jest prezentowane wizualnie, **albo**
•	**Ścieżką dźwiękową** (**audiodeskrypcją**), w której narrator relacjonuje treści prezentowane wizualnie.  

Transkrypcja może być wykorzystana przez technologie wspomagające do zaprezentowania użytkownikom niewidomym i słabowidzącym treści nagrania wideo w odpowiedniej dla nich formie, np. zamiany tekstu na mowę syntetyczną lub pismo punktowe (brajl). Audiodeskrypcja może także ułatwić osobom z ograniczonymi umiejętnościami językowymi, poznawczymi i edukacyjnymi zrozumienie treści.

Alternatywa musi być równoważna filmowi. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-2-1 I1.2.1
Tylko audio lub tylko wideo (nagranie)
](https://wcag.lepszyweb.pl/#audio-only-and-video-only-prerecorded).

### Metody i narzędzia testowe 
Inspekcja ręczna strony

### Identyfikacja treści

Wszystkie nagrane wcześniej treści zawierające tylko wideo **z wyjątkiem** wszelkich treści wideo, które są wyraźnie oznaczone jako medialna alternatywa dla tekstu.

   **Uwaga**: Treść zawierająca tylko wideo jest definiowana wizualna jako prezentacja oparta na czasie, która zawiera wyłącznie wideo (bez dźwięku i bez interakcji).

-	W prezentacji tylko wideo informacje są prezentowane na różne sposoby, w tym animację, tekst lub grafikę, ustawienia i tło, działania i emocje ludzi, zwierząt itp.


- Medialne alternatywy dla tekstu to media, które nie zawierają więcej informacji niż te, które są już przedstawione w tekście (bezpośrednio lub za pomocą tekstow alternatywnych). 
Może to być tylko dźwięk, tylko wideo (w tym wideo w języku migowym) lub audio-wideo.

**Uwaga**: Jeśli do wideo dołączony jest dźwięk (dźwięk), nie jest to już tylko „tylko wideo”; skorzystaj z testów mediów zsynchronizowanych  w sekcji [17. Miltimedia zsynchronizowane]

### Zastosowanie:

16.B 1.2.1-odpowiedniki-wideo **nie ma zastosowania**, jeśli na stronie internetowej nie ma wcześniej nagranych prezentacji tylko-audio, która spełnia kryteria opisane powyżej w sekcji Identyfikacja treści.


### Jak testować:

1.  Ustal, czy do każdej treści zawierającej tylko wideo dołączona alternatywa tekstowa lub dźwiękowa (np. transkrypcja lub ścieżka audio, która zawiera opis treści i akcji wideo.


    1.  Ustal, czy każda transkrypcja jest tekstem (tzn. obraz z tekstem transkrypcji nie wystarczy do zaliczenia tego testu).

   **Uwaga 1**: Transkrypcja musi być tekstem i nie może być obrazem tekstu. Jednym ze sposobów ustalenia, czy transkrypcja jest tekstem, jest użycie urządzenia wskazującego (takiego jak mysz), albo klawiatura czy polecenia dyktowania, aby zaznaczyć fragment tekstu w transkrypcji. Jeśli można zaznaczyć fragmenty tekstu, transkrypcja jest tekstem.

2.  Odtwarzaj treść tylkoe wideo podczas przeglądania tekstu lub odsluchiwania dźwięku.

    **Uwaga**: alternatywa dźwiękowa nie musi być zsynchronizowana z treścią tylko wideo. W&nbsp;niektórych przypadkach użytkownicy mogą zdecydować się na słuchanie alternatywy dźwiękowej zamiast wideo (na przykład osoby niewidome i slabowidzące, które mogą pominąć tylko wideo).

3.	Ustal, czy informacje w tekście lub dźwięku zawierają te same treści, które wyświetla prezentacja tylko wideo (np. jeśli wideo zawiera wiele symboli, alternatywa musi określać, który symbol jest powiązany z każdym przedstawionym działaniem). Wszystkie istotne widoczne na filmie lub animacji działania muszą być przekazywane alternatywnie. Obejmuje to takie np. czynnosci, jak okazanie dowodu tożsamości policjantowi, czy wyświetlenie zegara z godziną 6:30 rano.

**Wskazówka**: Podczas przeglądania alternatywy pomocne może być wyobrazenie sobie tego, co jest prezentowane przez alternatywę, tak że gdyby film został wyłączony lub usunięty, alternatywą byłaby równie skuteczną prezentacją treści (zarówno dokładną, jak i kompletną).


### Wyniki oceny

Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.2.1:

1. W przypadku wszystkich treści tylko wideo dostępna jest alternatywa tekstowa lub dźwiękowa **oraz**

2.  Tekst lub dźwięk stanowi dokładne i pełne przedstawienie treści tylko wideo.

## Zastosowane standardy

- {% include ks/1-2-1.md %}
- [16. Tylko audio i tylko wideo](ICT-16-tylko-audio-tylko-wideo)                                                                                                   