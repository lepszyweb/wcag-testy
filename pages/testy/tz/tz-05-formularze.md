---
title: 5. Formularze


sidebar: testy_sidebar
permalink: tz-05-formularze
folder: testy/tz
---


## Cel procedury testowej

Celem tej procedury testowej jest sprawdzenie, czy formularze i powiadomienia o formularzach zawierają odpowiednie instrukcje ekranowe i prawidłowe programowe powiązania, aby wszyscy użytkownicy mogli wchodzić w&nbsp;interakcje z formularzami w przewidywalny sposób. 

Ta procedura testowa obejmuje zmiany treści strony internetowej, które pojawiają się w wyniku interakcji z&nbsp;formularzami. Gdy interakcja formularza powoduje zmiany w treści strony internetowej, nie powinny to  być nieoczekiwane zmiany kontekstu. Gdy treść strony internetowej zmienia się w wyniku interakcji użytkownika z&nbsp;elementami formularza, użytkownik powinien otrzymywać automatyczne powiadomienie o zmianie.

Ta procedura testowa obejmuje kilka testów związanych z identyfikacją błędów, sugestiami i zapobieganiem błędom.

**Uwaga**: Ważne jest, aby zrozumieć różnicę między zmianami treści a zmianami kontekstu. Zmiany w treści obejmują zmiany związane z rozszerzaniem konspektu strony, ujawnianiem i ukrywaniem treści lub dostępem do menu dynamicznego. Natomiast zmiany w kontekście to poważne zmiany w treści lub funkcjonalnościach strony, takie jak uruchomienie nowego okna, wykonanie określonej akcji lub celowe przeniesienie fokusa klawiatury na inny komponent interfejsu. 

Zmiany kontekstu mogą być oczekiwane lub nieoczekiwane. Nieoczekiwane zmiany są mylące i uznawane za barierę dostępności.

Rozróżnienie zmian treści i zmian kontekstu bywa czasem problematyczne, ponieważ zmiana treści może również powodować zmianę kontekstu.

Procedura testowa „Formularze” obejmuje osiem testów:

1.	Test 5.A: 3.3.2-etykiety-lub-instrukcje 
2.	Test 5.B: 2.4.6-opisowe-etykiety.
3.	Test 5.C: 1.3.1-etykiety-instrukcje-powiązane programowo
4.	Test 5.D: 3.2.2-podczas-wprowadzania-danyc
5.	Test 5.E: 4.1.2-powiadomienia-o-zmianie
6.	Test 5.F: 3.3.1-identyfikacja-błędów
7.	Test 5.G: 3.3.3-sugestie-poprawy-bledow
8.	Test 5.H: 3.3.4-zapobieganie-błedom


### Test 5A. 3.3.2-etykiety-lub-instrukcje

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 3.3.2-etykiety-lub-instrukcje | 5.A     | Każde pole formularza ma etykietę lub instrukcję ekranową. |


### Cel testu 5A. 3.3.2-etykiety-lub-instrukcje

Celem tego testu jest sprawdzenie, czy wszystkie pola formularza mają etykiety lub instrukcje ekranowe. Zawsze, gdy na stronie umieszczone jest interaktywne pole formularza, musi ono zawierać etykietę lub instrukcje (np. pole tekstowe może mieć etykietę „Data urodzenia”). Etykiety lub instrukcje mogą być tekstem lub innymi elementami treści z alternatywą tekstową (np. grafiką) i muszą być widoczne, gdy pole formularza jest aktywne.

Sprawdzeniu w tym teście podlega jedynie to, czy pola formularzy posiadają etykiety lub instrukcje. To, czy etykiety lub instrukcje są wystarczająco jasne i opisowe, podlega ocenie w kolejnym teście - 5.B: 2.4.6-opisowe-etykiety. 

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu WCAG 3.3.2 Etykiety lub instrukcje.

### Metody i narzędzia testowe 

1.	ANDI: interaktywne (tylko w celu identyfikacji pola formularza).

2.	Inspekcja wzrokowa strony.


### Identyfikacja treści

1.  Znajdź wszystkie kontrolki formularzy (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.

2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub instrukcji formatowania itp.

    **WYJATEK**: Wyklucz kontrolki wyłączone. Nie są elementami aktywnymi, nie mogą otrzymać fokusa klawiatury, nie mogą być wybrane ani modyfikowane. 


### Zastosowanie

Test 5.A: 3.3.2-etykiety-lub-instrukcje **nie ma zastosowania**, jeśli na stronie nie ma elementów formularza lub wszystkie elementy formularza są wyłączone. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Użyj modułu ANDI: interaktywne. Sprawdź, czy każde pole formularza zawiera etykietę lub instrukcję.

    Przeprowadzasz inspekcję wzrokową. Celem jest ustalenie, czy wszystkie niewyłączone kontrolki formularzy posiadają widoczną etykietę lub instrukcję. Nie sprawdzasz w tym teście, czy etykieta lub instrukcja jest poprawna. Skorzystaj z przycisków poprzedni/następny element w module ANDI, by nawigować między interaktywnymi kontrolkami formularza.
	
	Każde pole formularza powinno mieć widoczną etykietę lub instrukcje. Może to oznaczać trzy sytuacje:
	
	- każde pole ma etykietę lub instrukcję **albo**
	
	- zestaw pól ma etykietę, która objaśnia każde pole formularza, **albo**
	
	- zestaw pól ma instrukcje, które wyjaśniają każde pole formularza.

### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 3.3.2:

1.  Każde pole formularza ma etykietę lub instrukcję ekranową.

### Uwaga

-   Etykieta lub instrukcja musi być widoczna, gdy pole formularza otrzymuje fokus (jest aktywne).

-   To, czy etykieta lub instrukcja wystarczająco opisuje pole jest objęte testem 5.B (2.4.6-opisowe-etykiety).

-   Programowe powiazanie etykiety tekstowej lub instrukcji jest objęte testem 5.C   1.3.1-programmatic-label.

## Opisowe etykiety

### Test 5.B 2.4.6–opisowe-etykiety

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.4.6–opisowe-etykiety | 5.B     | Każda etykieta lub instrukcja w formularzu wystarczająco informuje użytkowników, jakie dane są oczekiwane. |

### Cel testu 5.B 2.4.6–opisowe-etykiety

Celem testu 5.B 2.4.6–opisowe-etykiety jest sprawdzenie, czy jeśli element formularza ma etykietę ekranową lub instrukcję, to etykieta lub instrukcja jest wystarczająco jasna i opisowa. Etykiety i instrukcje ekranowe muszą również zawierać wszystkie obowiązujące wymagania dotyczące danych (np. formaty daty,  typ danych, informacja, że pole jest obowiązkowe, itp.). 

Zapewnienie jasnych i jednoznacznych etykiet i instrukcji (w tym przykładów oczekiwanych formatów danych) pomaga wszystkim użytkownikom - ale szczególnie osobom z zaburzeniami poznawczymi, językowymi i trudnościami w nauce - poprawnie wprowadzać informacje. Celem tego wymagania nie jest zaśmiecanie strony niepotrzebnymi informacjami, ale zapewnienie ważnych wskazówek i instrukcji, które przyniosą korzyści osobom z&nbsp;niepełnosprawnościami. Zbyt dużo informacji lub instrukcji może być tak samo szkodliwych jak zbyt mało. Celem jest zapewnienie się, że użytkownik dostarczy wystarczającą ilość informacji, aby wykonać zadanie bez zbędnego zamieszania lub nawigacji.

Sprawdzeniu w tym teście podlega jedynie to, czy etykiety lub instrukcje są wystarczająco jasne i opisowe, a nie sprawdzanie, czy etykiety i instrukcje są prawidłowo powiązane programowo. Poprawność programowego powiązania etykiet lub instrukcji z polami formularza oceniana jest w następnym teście 5.C: 1.3.1-etykiety-instrukcje-powiązane programowo    

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu WCAG 2.4.6 Nagłówki i etykiety.

### Metody i narzędzia testowe 

1.	ANDI: interaktywne.

2.	Inspekcja wzrokowa strony.


### Identyfikacja treści

1.  Znajdź wszystkie kontrolki formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.

2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z  kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.

    **WYJATEK**: Wyklucz kontrolki wyłączone. Nie są elementami aktywnymi, nie mogą otrzymać fokusa klawiatury, nie mogą być wybrane ani modyfikowane. 


### Zastosowanie

Test 5.B 2.4.6–opisowe-etykiety **nie ma zastosowania**, jeśli na stronie nie ma elementów formularza lub wszystkie elementy formularza są wyłączone albo jeśli elementy formularza nie mają etykiet (instrukcji). W takim przypadku oznacz wynik testu jako **ND**.

Pamiętaj, że jeśli etykieta lub instrukcja nie jest widoczna, gdy pole formularza jest aktywne (ma fokus klawiatury), to strona nie spełnia wymagań testu 5.A. i nawet, jeśli istnieją ukryte etykiety lub instrukcje, to nie są one testowane i&nbsp;oceniane. 


### Jak testować

1.  Przejrzyj etykiety i instrukcje dla każdego pola formularza.

2.  Ustal, czy etykiety lub instrukcje dla pól oczekujących na dane użytkownika wystarczająco opisują cel i&nbsp;obowiązujące wymagania dotyczące danych (formaty daty, wymagane pola, typ danych itp.).

    **Uwaga**: Chociaż możesz skorzystać z narzędzia testowego, aby znaleźć wszystkie elementy formularzy na stronie, to narzędzie nie oceni za ciebie, czy etykiety lub instrukcje są odpowiednie, aby użytkownicy wiedzieli, jakie informacje są potrzebne i w jakim formacie.

    **Uwaga 2**: Jeśli pole formularza nie zawiera instrukcji, może być konieczne wypełnienie pola formularza, aby sprawdzić, czy instrukcja nie pojawi się dopiero po wprowadzeniu danych.     

### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 2.4.6:

1.  Każda etykieta lub instrukcja dla pola formularza jest wystarczająco jasna i opisowa, aby użytkownicy wiedzieli, jakie dane są oczekiwane.

### Uwaga

-   Komunikat o błędzie nie jest wystarczający do przekazania oczekiwanego formatu, aby zaliczyć ten test. Istotą wymogu wystarczająco opisowych etykiet i instrukcji jest przede wszystkim pomoc użytkownikowi w uniknięciu błędów.

-   W tym teście należy uwzględnić wszelkie zmiany formularzy, które pojawiają się automatycznie lub są wynikiem interakcji ze stroną.

## Etkiety i instrukcje powiązane programowo

### Test 5.C: 1.3.1-etykiety-powiązane programowo

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.1-etykiety-powiązane programowo | 5.C     | Kombinacja dostępnej nazwy, dostępnego opisu i innych asocjacji programowych (np. powiązania nagłówków kolumn lub wierszy z kolumnami lub wierszami) opisuje każde pole wejściowe i zawierają wszystkie niezbędne instrukcje i wskazówki (tekstowe i graficzne). |


#### Cel testu  5.C: 1.3.1-etykiety-powiązane programowo


Celem testu 5.C: 1.3.1-etykiety-instrukcje-powiązane programowo jest sprawdzenie, czy etykiety i instrukcje dla pól formularzy są programowo powiązane z tymi polami. Ten test stanowi kontynuację dwóch poprzednich testów (5.A i&nbsp;5.B), które służyły ocenie, czy pola formularza posiadają widoczne etykiety lub instrukcje i czy są ono wystarczająco opisowe i jasne. 

Programowe powiązanie etykiet i instrukcji z polami formularza, których dotyczą, to niezbędny warunek, aby technologie wspomagające prawidłowo przekazywały użytkownikom informacje, jakie dane, jakiego typu i w jakim formacie są oczekiwane. Powiązanie programowe pozwalają technologiom wspomagającym, takim jak czytniki ekranu, przekazywać użytkownikowi ważne informacje, aby rozumiał przeznaczenie i funkcję każdego elementu formularza.
Technologie wspomagające przekazują użytkownikom informacje &bdquo;wyliczone&rdquo; z odpowiednio zakodowanych i powiązanych z polami formularzy treści umieszczonych w tekstach etykiet i instrukcji widocznych na ekranie oraz treściach etykiet i instrukcji niewidocznych na ekranie, przekazywanych w atrybutach pól bądź elementów z nimi powiązanych.

Oznacza to, że jest możliwe, iż pole formularza, które nie spełnia wymogów testów 5.A i 5.B, bo nie ma widocznej na ekranie etykiety lub instrukcji, przejdzie pomyślnie ten test, ponieważ instrukcje mogą być niewidoczne na ekranie, ale możliwe do odczytania przez technologię wspomagającą.    

Podobnie jak poprzedni test obejmował również zmiany w formularzach, które pojawiają się automatycznie lub w&nbsp;wyniku interakcji ze stroną, także i&nbsp;ten test wymaga uwzględnienia wszystkich zmian, pojawiającychsię automatycznie lub będących wynikiem akcji użytkownika.

Wyniki tego testu służą do ustalenia, czy spełnione są kryteria sukcesu WCAG 1.3.1 Informacje i relacje oraz 4.1.2 Nazwa, rola, wartość.


### Metody i narzędzia testowe 

1.	ANDI: (elementy) interaktywne.


### Identyfikacja treści

1.  Znajdź wszystkie kontrolki formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.

2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z  kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.


    **WYJATEK**: Wyklucz kontrolki wyłączone. Nie są elementami aktywnymi, nie mogą otrzymać fokusa klawiatury, nie mogą być wybrane ani modyfikowane. 
	
### Zastosowanie

Test 5.C: 1.3.1-etykiety-instrukcje-powiązane programowo **nie ma zastosowania**, jeśli na stronie nie ma aktywnych (włączonych) elementów formularza. W takim przypadku oznacz wynik testu jako **ND**.	


### Jak testować

1.	Uruchom ANDI: elementy interaktywne (ustawienie domyślne).

2.	Użyj myszy lub przycisków następny/poprzedni element, aby podświetlić każdy aktywny element formularza i&nbsp;przejrzeć dane wyjściowe ANDI.

3.	Przejrzyj wyniki ANDI dla każdego pola formularza, na którym można ustawić fokus.


    **Uwaga**:
	
    -	W tym teście należy uwzględnić wszelkie zmiany elementów formularza, które następują automatycznie lub są wynikiem interakcji ze stroną.

    -	Przyciski opcji i pola wyboru powinny być co najmniej programowo powiązane z&nbsp;ich pytaniami i&nbsp;odpowiedziami.

    -	Pola formularza nie muszą mieć powiązań programowych z nagłówkami sekcji formularza, chyba że istnieje znaczące ryzyko pomyłki.

    -	ANDI nie wyświetla opcji na liście rozwijanej, nawet jeśli są one wybrane. Nie jest to uważane za błąd, ponieważ technologie wspomagające odczytają te elementy. Zawartość listy rozwijanej nie jest uważana za część powiązania programowego wymaganego dla etykiety listy rozwijanej.


4.	Przejrzyj inne asocjacje programowe, takie jak nagłówki tabeli lub położenie w hierarchicznej strukturze listy, aby ustalić, czy dostarczają one, czy przyczyniają się do opisu pola formularza, wskazówek lub instrukcji.

    **Uwaga**:

    -	Aby ocenić etykiety i wskazówki dostarczone przez inne powiązania programowe, może być konieczne wykonanie innych testów, w tym między innymi [14. Tabele](tz-14-tabele) i [10. Struktury treści](tz-10-struktury-tresci).
	
	-	Opcje listy rozwijanej (elementy `<option>` elementu `<select>`) nie są częścią opisu pola formularza, wskazówek ani instrukcji potrzebnych do spełnienia tego wymagania.



### Ocena wyników

Jeśli którekolwiek z poniższych stwierdzeń jest **prawdą**, wówczas strona (treść) **spełnia** testowane wymaganie i jest (w testowanym zakresie) **zgodna** z KS 1.3.1:

1.	Dane wyjściowe ANDI obejmują wszystkie istotne instrukcje i wskazówki dla elementu formularza, w tym informację, że wypełnienie pola jest wymagane, **lub**

2.	Etykiety opisowe i wskazówki są zapewnione przez inne powiązania programowe (np. asocjacje kolumn lub wierszy tabeli), **lub**

3.  Kombinacja Wyjścia ANDI i innych powiązań programowych obejmuje wszystkie istotne instrukcje i wskazówki.

### Uwaga

-   Test ten obejmuje również wymóg dotyczący [ kryterium sukcesu 4.1.2 Nazwa, rola wartość](https://www.w3.org/WAI/WCAG21/Understanding/name-role-value).

- W tym teście należy uwzględnić wszelkie zmiany elementów formularza, które następują automatycznie lub są wynikiem interakcji ze stroną.

- Aby ocenić etykiety i wskazówki dostarczone przez inne powiązania programowe, może być konieczne wykonanie innych testów, w tym między innymi [14. Tabele](tz-14-tabele) i [10. Struktury treści](tz-10-struktury-tresci).

- Przyciski opcji i pola wyboru powinny być co najmniej programowo powiązane z ich pytaniami i odpowiedziami.

- Pola formularzy nie muszą mieć powiązań programowych z nagłówkami sekcji formularza, chyba że istnieje znaczące ryzyko pomyłki.

## Podczas wprowadzania danych 

### Test 5.D 3.2.2-podczas-wprowadzania-danych

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 3.2.2-podczas-wprowadzania-danych | 5.D     | Żadna zmiana wyboru albo wartości w polu formularza (np. wprowadzanie danych w polu tekstowym, zmiana wyboru przycisku opcji), ani opuszczenie pola formularza nie inicjuje nieoczekiwanej zmiany kontekstu |

### Cel testu 5.D 3.2.2-podczas-wprowadzania-danych

Celem tego testu jest sprawdzenie, czy podczas wypełniania przez użytkownika pól formularza bądź zaznaczania wybranych opcji nie następuje nieoczekiwana zmiana kontekstu. 

Przykłady nieoczekiwanych zmian kontekstu obejmują:

-	automatyczne przesłanie formularza po opuszczeniu pola,
-	automatyczne przesłanie formularza po opuszczeniu ostatniego pola w formularzu,
-	uruchomienie nowego okna, gdy zostanie zmienione zaznaczenie w grupie przycisków opcji,
-   przeniesienie fokusa na inny komponent interfejsu po zaznaczeniu elementu na liście wyboru,
-   zmiana rozmiaru okna po wprowadzeniu tekstu w polu szczegółów.

Nieoczekiwana zmiana kontekstu może powodować znaczące zamieszanie dla użytkowników.

Test polega na obserwacji zachowania się strony internetowej podczas wprowadzania przez testera danych do formularza. Do przeprowadzenia testu nie są używane żadne narzędzia testujące.

Wyniki tego testu służą do ustalenia, czy spełnione są kryteria sukcesu WCAG 3.2.2 Podczas wprowadzania danych.

### Metody i narzędzia testowe 
Kontrola ręczna, obserwacja

### Identyfikacja treści

1.  Znajdź wszystkie kontrolki formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.

2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z  kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.


    **WYJATEK**: Wyklucz kontrolki wyłączone. Nie są elementami aktywnymi, nie mogą otrzymać fokusa klawiatury, nie mogą być wybrane ani modyfikowane. 
	
### Zastosowanie

Test 5.D: 3.2.2-podczas-wprowadzania-danych **nie ma zastosowania**, jeśli na stronie nie ma aktywnych (włączonych) elementów formularza. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Użyj klawiatury, aby przechodzić elementów formularza, np. pól tekstowych, przycisków opcji, pól wyboru, przycisków.

    **Uwaga**: Jeśli nie możesz nawigować do aktywnego pola formularza za pomocą klawiatury, sprawdź, czy nie możesz użyć do nawigacji i uzupełnienia elementów formularza urządzenia wskazującego, takiego jak np. mysz. (W takim przypadku nie powiedzie się test dostępności z klawiatury (4.A&nbsp;2.1.1-dostep-z-klawiatury).

    Zwracaj szczególną uwagę takie elementy, jak rozwijane listy wyboru czy przyciski opcji. W&nbsp;niektórych przypadkach następuje automatyczne uruchamianie opcji z listy wyboru, na którą został przeniesiony kursor podczas przemieszczania się między opcjami. Gdy użytkownik klawiatury przechodzi do pierwszej opcji, treść jest uruchamiana i nie ma możliwości przejścia za pomocą klawiatury  do innych opcji, co oznacza, że niespełnione jest także kryterium 4.A 2.1.1-dostep-z-klawiatury, ponieważ inne opcje nie są dostępne z&nbsp;klawiatury (choć mogą być dostępne za pomocą myszy. Dla tego testu istotna jest jednak nieoczekiwana zmiana kontekstu (automatyczne uruchomienie pierwszej z opcji, na jaką trafi użytkownik klawiatury, choć nie potwierdzi swojego wyboru). 	

2.  Wprowadzaj dane w każdej kontrolce formularza, np. zaznacz wybrany przycisk opcji lub pole wyboru, wpisz informacje w polu tekstowym, wybierz element z rozwijanej listy opcji.

3.  Opuść wypełniony element formularza i zaobserwuj, czy powoduje to są jakieś nieoczekiwane zmiany kontekstu.

    **Uwaga**: W przypadku niektórych typów pól formularzy, takich jak pola wprowadzania tekstu, może być konieczne odsunięcie fokusa od pola, aby zaobserwować, czy nie następuje zmiana kontekstu.

4.  Zmiany w kontekście obejmują zmiany: programu użytkownika, rzutni, fokusa, treści zmieniającej znaczenie strony.

    **Uwagi dotyczące definicji**:

    - **Programy użytkownika** to przeglądarki internetowe, odtwarzacze multimedialne, wtyczki i inne programy - w tym technologie wspomagające - które pomagają w wyszukiwaniu, renderowaniu i interakcji z treścią stron internetowych.
    - **rzutnia** to rozmiar ekranu (może to być okno lub ramka), w którym program użytkownika prezentuje treść (na przykład rzutnia urządzenia przenośnego jest znacznie mniejsza niż rzutnia ekranu monitora zewnętrznego).
    - **Zmiana kontekstu** to istotna zmiana w treści, która - jeśli zostanie dokonana bez świadomości użytkownika - może dezorientować użytkowników.	
	

**Uwaga**: Zmiany nie uważa się za nieoczekiwaną, jeśli:

-  Użytkownik jest powiadamiany o zbliżającej się zmianie kontekstu.
-  Kontrolka ma wyraźnie na celu zainicjowanie zmiany kontekstu po aktywacji.
		
### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** testowane wymaganie i jest **zgodna** z KS 3.2.2:


1.  Zmiana wartości elementu formularza nie powoduje nieoczekiwanej zmiany kontekstu.

### Uwaga

-   W przypadku niektórych typów pól formularzy, takich jak pola wprowadzania tekstu, może być konieczne odsunięcie fokusa od pola, aby zaobserwować, czy nie następuje zmiana kontekstu.


## Powiaddomeinia o zmianie

### Test 5.E 4.1.2-powiadomienia-o-zmianie

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 4.1.2-powiadomienia-o-zmianie | 5.E     | Strona powiadamia użytkownika o każdej zmianie treści związanej z formularzem. |


### Cel testu 5.E 4.1.2-powiadomienia-o-zmianie


Celem tego testu jest sprawdzenie, czy strona internetowa zapewnia wystarczające powiadomienie i opis wszelkich zmian treści na stronie internetowej, które nastąpiły w wyniku interakcji z elementem formularza. Gdy element formularza inicjuje zmianę treści, strona internetowa może powiadomić użytkowników, że mogą się tego spodziewać za pomocą różnych technik, w tym tekstu w sąsiedztwie elementu formularza, wyskakującego komunikatu lub modalnego okna dialogowego zawierającego tekst powiadamiający użytkowników o zmianie. 


**Uwaga**: Ten test jest badaniem mającym na celu stwierdzenie, czy użytkownik otrzymuje odpowiednie powiadomienie o każdej zmianie treści na stronie z formularzem, która występuje na stronie w wyniku interakcji z formularzem, a nie o zmianie treści na inne stronie.


Wyniki tego testu służą do ustalenia, czy spełnione są kryteria sukcesu WCAG 4.1.2 Nazwa, rola, wartość.

### Metody i narzędzia testowe 


1.	ANDI: interaktywne.
2.	ANDI: struktury > żywe regiony.

### Identyfikacja treści

1.  Znajdź wszystkie kontrolki formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.

2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z  kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.


3.	Znajdź wszystkie zmiany treści strony, które nastąpią w wyniku interakcji z elementami formularza. Zmiany treści mogą obejmować zmiany innych treści lub elementów sterujących, komunikaty o błędach, informacje tekstowe, nowe treści, usunięte treści itp.

    **Uwaga**: Ten test dotyczy tylko i wyłącznie treści, które w wyniku interakcji z formularzem zmieniają się na badanej stronie, a nie na innych stronach. 
	
    **NIE WYKLUCZAJ** z badania wyłączonych elementów formularzy. Wprawdzie nie są one elementami aktywnymi, nie mogą otrzymać fokusa klawiatury, nie mogą być wybrane ani modyfikowane, ale w wyniku interakcji z formularzem może nastąpić zmiana treści, która spowoduje włączenie wyłączonej wcześniej kontrolki. W takim przypadku należy wykonać ten, a także poprzednie testy, aby sprawdzić, czy te kontrolki spełniają wymagania dostępności.    
	
### Zastosowanie

Test 5.E 4.1.2-powiadomienia-o-zmianie **nie ma zastosowania**, jeśli na stronie nie ma aktywnych (włączonych) elementów formularza lub jeśli treść strony nie zmienia się w wyniku interakcji z formularzem. W takich przypadkach oznacz wynik testu jako **ND**.



### Jak testować

1.  Kontynuuj test 5.D.

2.	W razie potrzeby powtórz interakcje, które powodują zmiany w treści strony (zmiany instrukcji, powiadomienie o&nbsp;błędach, usunięcie treści, dodanie treści itp.).

    **Uwaga**: Konieczne może być użycie myszy do ustalenia, czy zmiany stanu występują po najechaniu myszą, czy po kliknięciu, **oraz**
	
	**Zwróć uwagę**, że w zależności od komponentu formularza zmiana stanu może zostać wywołana przez różne akcje, takie jak zmiana wartości lub stanów innych komponentów, przełączanie funkcji, wprowadzanie danych do komponentu, najechanie myszą itp.

3.  Określ, w jaki sposób użytkownik jest powiadamiany o zmianie treści.
 
	
	Istnieje kilka sposobów powiadamiania użytkownika, w tym komunikaty o elemencie formularza wywołującym zmianę, otwarcie okna dialogowego, przeniesienie fokusa na zmienioną treść lub do żywego regionu ARIA.
	
	**Uwaga**: Ta lista technik spełniających KS 4.1.2 nie jest wyczerpująca; mogą pojawić się nowe  dopuszczalne techniki.
	

    a. Ustal, czy element formularza, który wyzwala zmianę, ma dostępną nazwę, dostępny opis lub kontekst, który zapewnia wystarczający opis celu komponentu interfejsu.

    Jeżeli zmiany treści są bezpośrednim wynikiem działania użytkownika w trakcie interakcji z treścią, a element interfejsu, który wywołuje zmianę, zawiera wystarczający opis zmiany, wówczas nie jest konieczne dodatkowe programowe powiadamianie o zmianie.  

    2.  Zidentyfikuj wszystkie okna dialogowe ostrzegające użytkownika o zmianach treści.

        1.  Ustal, czy okna dialogowe zapewniają wystarczające programowe powiadamianie o zmianach treści.

    3.  Zidentyfikuj zmiany treści, które powodują przeniesienie fokusu na treść, która uległa zmianie.

        1.  Ustal, czy przeniesienie fokusa na zmienioną treść jest wystarczające, aby powiadomić użytkownika o zdarzeniu zmiany (np. istnieje wystarczający opis zmiany w treści, na którą fokus został przeniesiony.

    4.  Zidentyfikuj zmiany treści występujące w żywym regionie ARIA:


        Uwaga : żywe regiony ARIA to sposób na oznaczenie i poinformowanie technologii wspomagających o&nbsp;dynamicznych obszarach strony internetowej. Żywy region może ostrzec technologię użytkownika o&nbsp;pojawieniu się komunikatu o błędzie lub innych zmian (np. notowania giełdowego lub stopera). Dzięki temu technologia wspomagająca może powiadamiać użytkowników o zmianie treści bez przerywania ich bieżącego skupienia.

        1.  Uruchom ANDI: struktury

        2.  Wybierz łącze „żywe regiony”, a następnie użyj myszy, aby najechać wskaźnikiem myszy na dowolny zidentyfikowany żywy region (alternatywnie, użyj przycisków poprzedni/następny, aby przejść do zidentyfikowanych żywych regionów)..

        3.  Sprawdź, czy w żywym regionie pojawia się zmieniona treść.

**Uwagi**:

-	Wszystkie elementy formularza, które zmieniły się podczas tego testu, muszą zostać przetestowane pod kątem testu 5.C: 1.3.1-etykiety-instrukcje-powiązane programowo.

-	Cała ujawniona treść musi zostać przetestowana zgodnie z testem 4.G, 2.4.3-fokus-do-tresci-odkrytej

-	Konieczne może być użycie myszy do ustalenia, czy zmiany stanu występują po najechaniu myszą, czy po kliknięciu.

-   W zależności od komponentu formularza zmiana stanu może zostać wywołana przez różne akcje, takie jak zmiana wartości lub stanów innych komponentów, przełączanie funkcji, wprowadzanie danych do komponentu, najechanie myszą itp.

-	Ta lista technik spełniających KS 4.1.2 nie jest wyczerpująca; mogą pojawić się nowe techniki, które nie zostały wyraźnie określone i są dopuszczalne.



### Ocena wyników

Jeśli którekolwiek z poniższych stwierdzeń jest **prawdą**, wówczas strona (treść) **spełnia** testowane wymaganie i jest (w testowanym zakresie) **zgodna** z KS 4.1.2:

1.	Działanie użytkownika bezpośrednio powoduje zmianę treści, **a** komponent interfejsu, który wywołał zmianę, dostarczył wystarczający opis zdarzenia zmiany **lub**

2.  Strona powiadamia użytkownika o zmianie za pomocą okna dialogowego dostępnego z klawiatury, LUB

3.  Strona przenosi fokus na treść, która uległa zmianie, a zmieniona treść zapewnia wystarczający opis zmiany, **lub**

4.  Treść, która uległa zmianie, znajduje się w żywym regonie ARIA.


### Uwaga

-   Wszystkie elementy formularza, które zmieniły się podczas tego testu, muszą zostać przetestowane pod kątem testu 5.C: 1.3.1-etykiety-instrukcje-powiązane programowo.

-   Cała ujawniona treść musi zostać przetestowana zgodnie z testem 4.G, **2.4.3-fokus-do-tresci-odkrytej**.

-   Konieczne może być użycie myszy do ustalenia, czy zmiany stanu występują po najechaniu myszą, czy po kliknięciu.

-   W zależności od komponentu formularza zmiana stanu może zostać wywołana przez różne akcje, takie jak zmiana wartości lub stanów innych komponentów, przełączanie funkcji, wprowadzanie danych do komponentu, najechanie myszą itp.

-	Ta lista technik spełniających KS 4.1.2 nie jest wyczerpująca; mogą pojawić się nowe techniki, które nie zostały wyraźnie określone i są dopuszczalne.


## Identyfikacja błędów

### Test 5.F 3.3.1-identyfikacja-bledow

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 3.3.1-identyfikacja-bledow  | 5.F     | Błędnie wypełniony element formularza jest wskazany i&nbsp;wystarczająco opisany użytkownikowi w tekście. |

### Cel testu 5.F 3.3.1-identyfikacja-bledow

Celem tego testu jest sprawdzenie, czy użytkownicy otrzymują wskazówki i instrukcje potrzebne do zrozumienia, w&nbsp;którym polu wejściowym formularza występuje błąd, wszędzie tam, gdzie w elementach formularza przewidziano automatyczne wykrywanie błędów. Użytkownicy muszą wiedzieć, że wystąpił błąd, co jest nie tak i które elementy należy poprawić. 

**Uwaga**: Nie jest wymagane, aby formularz miał automatyczne wykrywanie błędów.

Wyniki tego testu służą do ustalenia, czy spełnione są kryteria sukcesu WCAG 3.3.1 Identyfikacja błędów.

#### Metody i narzędzia testowe 

1.	Inspekcja wzrokowa.

2.	Klawiatura.


### Identyfikacja treści

Znajdź  wszystkie automatycznie wykrywane błędy wprowadzania danych, powiadomienia o błędach, sugestie naprawy błędów i związane z nimi instrukcje:

1.  Znajdź wszystkie kontrolki formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.

2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z  kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.

3.  Celowo wprowadzaj wartości i dokonuj wyborów, które naruszają format lub inne instrukcje formularzy, aby spowodować wystąpienie błędów i zobaczyć powiadomienia o błędach. Celowo pomijaj w każdym przypadku wprowadzenie wymaganych danych.

### Zastosowanie

Test 3.3.1-identyfikacja-bledow **nie ma zastosowania**, jeśli błędy we wprowadzaniu danych w formularzu na stronie nie są wykrywane automatycznie. W takich przypadku oznacz wynik testu jako **ND**.


### Jak testować

1.  Celowo naruszaj wymagane formatowanie i inne wskazówki dotyczące wypełniania formularza, np. pozostaw puste pole formularza, użyj innego formatu daty niż wymagany i / lub utwórz hasło, które nie spełnia wymagań dotyczących siły hasła.

2.  Spróbuj przesłać formularz lub przejść do następnej strony.

3.  Ustal, czy błąd został określony (wskazany) i opisany w tekście.

    1.  Ustal, czy błąd został określony (wskazany)w tekście, np. „Błąd: W polu hasła.”

    2.  Ustal, czy błąd jest wystarczająco opisany, np. w oknie dialogowym z informacją „Wprowadzone hasło jest nieprawidłowe”.


### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** testowane wymaganie i jest **zgodna** z KS 3.3.1:


1.  Element, który zawiera błąd, jest zakomunikowany tekstem i wystarczająco opisany użytkownikowi w tekście.

**Wskazówka**: Sprawdzasz, czy istnieje tekstowe wskazanie błędnego pola **oraz** opis każdego błędu (jeśli strona ma automatyczne wykrywanie błędów).

**Uwaga**: Ten test nie sprawdza, czy komunikat o błędzie sugeruje także, jak naprawić ten błąd. To, czy istnieją sugestie naprawy błędów i czy są one wystarczające, zostanie ocenione w teście 5.G, 3.3.3-sugestie-poprawy-bledow. 

## Sugestie korekty błędów

#### Test 5.G: 3.3.3-sugestie-poprawy-bledow

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 3.3.3-sugestie-poprawy-bledow | 5.G     | Podano wskazówki dotyczące sposobu poprawienia błędów w polach formularza. |


Celem tego testu jest sprawdzenie, czy w przypadku automatycznego wykrycia błędu użytkownicy otrzymują wskazówki dotyczące naprawy błędu (jeśli to możliwe). Zdarzają się sytuacje, w których sugestie dotyczące błędów nie są możliwe, na przykład gdy nie są one znane lub gdy wprowadzenie poprawek może zagrozić bezpieczeństwu lub przeznaczeniu pola. Zapewnienie sugestii poprawiania błędów pomaga użytkownikom pomyślnie wypełnić formularz, zrozumieć każdy błąd i ustalić sposób jego poprawienia, a także zmniejsza liczbę potrzebnych zmian we wprowadzonych danych. Sugestia poprawy błędu musi oferować prawidłowe alternatywne opcje wprowadzania danych lub porady, jak poprawić nieprawidłowe wpisy. 


Wyniki tego testu służą do ustalenia, czy spełnione są kryteria sukcesu WCAG 3.3.3 Identyfikacja błędów.

#### Metody i narzędzia testowe 

1. Inspekcja wzrokowa  - analiza poznawcza

### Identyfikacja treści

Znajdź  wszystkie automatycznie wykrywane błędy wprowadzania danych, powiadomienia o błędach, sugestie naprawy błędów i związane z nimi instrukcje:

1.  Znajdź wszystkie kontrolki formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.

2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z  kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.

3.  Celowo wprowadzaj wartości i dokonuj wyborów, które naruszają format lub inne instrukcje formularzy, aby spowodować wystąpienie błędów i zobaczyć powiadomienia o błędach. Celowo pomijaj w każdym przypadku wprowadzenie wymaganych danych.

### Zastosowanie

Test 5.G 3.3.3-sugestie-poprawy-bledow **nie ma zastosowania**, jeśli którekolwiek z poniższych stwierdzeń jest prawdziwe:

- Nie ma automatycznego wykrywania błędów wejściowych.

- Nie można podać sensownych sugestii poprawy błędów, ponieważ nie są znane.

- Podanie informacji o tym, jak poprawić błąd, zagroziłoby bezpieczeństwu lub celowi treści, np. szczegółom dotyczącym błędnego hasła.

W takich przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Kontynuuj test 5.F.

2.  Ustal, czy wskazówki zawierają wystarczające szczegóły, jak skorygować błąd lub sugerują poprawną formę danych.


Sugestia błędu musi zawierać poprawione dane wejściowe lub szczegółowe wskazówki dla użytkownika, jak poprawić wprowadzone dane wejściowe. 

### Ocena wyników

Jeśli którekolwiek z poniższych stwierdzeń jest **prawdą**, wówczas strona (treść) **spełnia** testowane wymaganie i jest (w testowanym zakresie) **zgodna** z KS 3.3.3:


1.  Podano sugestie poprawienia wprowadzonych danych, **lub**

2.  Opis błędu zawiera odpowiednie wskazówki dla użytkownika, aby wiedział, co jest wymagane do naprawienia błędu.

## Zapobieganie błędom

### Test 5H: 3.3.4-zapobieganie-bledom

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| Test 5H: 3.3.4-zapobieganie-bledom | 5.H     | Strona internetowa umożliwia użytkownikowi sprawdzenie, anulowanie lub potwierdzenie danych przed ich wysłaniem. |

Celem tego testu jest ustalenie, czy strona internetowa pozwala użytkownikowi sprawdzić, cofnąć lub potwierdzić poprawność danych przed ich wysłaniem w każdym przypadku, gdy przesłanie formularza pociąga za sobą zobowiązania prawne lub transakcje finansowe (takie jak zakup biletu lotniczego), modyfikacje lub usunięcie danych kontrolowanych przez użytkownika w systemach pamięci masowej (takich jak aktualizacja danych kontaktowych dla konta bankowego) lub przesyła odpowiedzi testowe użytkownika. 

Pomaga to użytkownikom, w tym osobom z niepełnosprawnościami, uniknąć poważnych konsekwencji w wyniku pomyłki podczas wypełniania formularza, którego później nie można cofnąć ani zmienić. Niektóre osoby mogą częściej popełniać błędy z powodu trudności w nawigacji po niektórych interfejsach użytkownika, problemów z pamięcią krótkotrwałą albo koncentracją uwagi.

Wyniki tego testu służą do ustalenia, czy spełnione są kryteria sukcesu WCAG 3.3.4  Zapobieganie błędom (prawne, finansowe, dane).

#### Metody i narzędzia testowe 

1. Inspekcja wzrokowa
2. Klawiatura.

#### Identyfikacja treści

Znajdź kontrolki formularza, które po wprowadzeniu danych lub wybraniu opcji i przesłaniu formularza:

- powodują powstanie zobowiązań prawnych użytkownika **lub**

- inicjują przeprowadzenie transakcji finansowych, **lub**

- modyfikują albo usuwają kontrolowane przez użytkownika dane w systemach przechowywania danych,

- przekazują odpowiedzi testowe, egzaminacyjne 

### Zastosowanie
Test 5H: 3.3.4-zapobieganie-bledom **nie ma zastosowania**, jeśli którekolwiek z poniższych stwierdzeń jest prawdziwe:

- przesłanie formularza nie powoduje zobowiązań prawnych ani finansowych

- przesłanie formularza nie modyfikuje i nie usuwa danych kontrolowane przez użytkownika w systemach przechowywania danych  

- formularz nie zawiera odpowiedzi testowych, egzaminacyjnych. 
 
### Jak testować

1.  Uzupełnij wymagane pola formularza celowymi błędami i prześlij treść.


„Prześlij treść” oznacza każdy mechanizm, który przesyła treść. Warunki testu nie są ograniczone do użycia przycisku „Wyślij”. Formularze mogą mieć automatyczną kontrolę błędów wprowadzania, która wyświetla komunikat o błędzie, gdy tylko niepoprawne dane zostaną wstawione do pola formularza bez wymogu użycia przez użytkownika przycisku „Wyślij”. Możliwe jest również, że przycisk „Wyślij” może nie być aktywny, dopóki wszystkie wymagane pola formularza nie zostaną wypełnione; w takich przypadkach spróbuj najpierw wprowadzić nieprawidłowe dane do wszystkich pól. Inne przypadki, które mogą nie być zgodne z prostym mechanizmem „Wyślij”, mogą obejmować transakcje finansowe wymagające od użytkowników wypełnienia kilku stron formularzy (takich jak strona kasy, która zawiera informacje o wysyłce i fakturowaniu) przed zaoferowaniem możliwości sprawdzenia, potwierdzenia i poprawienia informacji. 

Wszystkie te mechanizmy powinny zostać przetestowane i ocenione przy użyciu w tym teście.

Prosty, jednostronicowy formularz zawierający mechanizm przesyłania treści może zostać sprawdzony przez użytkownika przed przesłaniem. Ten formularz nie musi zawierać dodatkowego kroku przeznaczonego na przeglądu poprawności przez użytkownika. Jednak w formularzu obejmującym wiele stron internetowych, na których dane są zbierane od użytkownika w wielu krokach przed zatwierdzeniem transakcji, metoda sprawdzania jest bardzo przydatna, ale nie wymagana. Aby spełnić ten wymóg, można zastosować inne techniki.


### Ocena wyników

Jeśli którekolwiek z poniższych stwierdzeń jest **prawdą**, wówczas strona (treść) **spełnia** testowane wymaganie i jest (w testowanym zakresie) **zgodna** z KS 3.3.4:

1.  Użytkownik może cofnąć przesyłanie **lub**

2.  Użytkownik ma możliwość przejrzenia, potwierdzenia i poprawienia informacji przed przesyłaniem formularza, **lub**

3.  Strona sprawdza dane pod kątem błędów i daje użytkownikowi możliwość ich poprawienia.


### Obowiązujące normy
- {% include ks/1-3-1.md %}
- {% include ks/2-4-6.md %}
- {% include ks/3-2-2.md %}
- {% include ks/3-3-1.md %}
- {% include ks/3-3-2.md %}
- {% include ks/3-3-3.md %}
- {% include ks/3-3-4.md %}
- {% include ks/4-1-2.md %}

- [10. Formularze](ICT-10-formularze.md)
- [5. Treść zmienna](ICT-05-tresc-zmienna.md) |
