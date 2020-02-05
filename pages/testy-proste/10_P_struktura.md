---
title: Podstawowy test struktury strony
tags: struktury

sidebar: testy-proste_sidebar

permalink: 10_P_struktura
folder: testy-proste
---

## Podstawowy test struktury strony
Podczas gdy inne testy z Bazy testów wstępnych koncentrują się na konkretnych kryteriach sukcesu w WCAG, ten test jest szerszy, bardziej ogólny. Pomaga zrozumieć, w jak różny sposób przeglądają i „widzą” stronę internetową niektórzy ludzie. W ramach tego podstawowego testu struktury strony sprawdzasz możliwość korzystania ze strony bez obrazów, stylów i układu.

Strony internetowe są często zaprojektowane z wieloma kolumnami, sekcjami, kolorami i innymi aspektami wizualnymi, które pomagają uporządkować informacje osobom, które widzą stronę w swoim domyślnym wyświetlaczu. Jednak niektórzy ludzie nie zobaczą strony w ten sposób. Osoby niewidome słuchają strony za pomocą czytnika ekranu lub czytają ją na monitorze brajlowskim. Niektóre osoby słabowidzące lub z innymi wadami wzroku zmieniają sposób wyświetlania strony, aby ją przeczytać; na przykład zmieniają układ z wielokolumnowego na jednokolumnowy, zmieniają rozmiar tekstu i inne własności.

Podstawowy test struktury polega na sprawdzeniu, jak strona działa, gdy jest  „linearyzowana” w jedną kolumnę, a prezentacja jest zmieniona, jak pokazano na obrazach poniżej.

### Obrazy przedstawiające zlinearyzowany i zmieniony sposób wyświetlania 
Poniższe zdjęcia ilustrują domyślny sposób wyświetlania strony internetowej w 3 kolumnach i zmieniony sposób wyświetlania.
Rysunek A pokazuje domyślne wyświetlanie trzech kolumn z nawigacją po lewej stronie.

![Rysunek A. Domyślne wyświetlanie strony z trzema kolumnami i stopką](images/andi/10_P_linear_01.png) 
RysunekA
 
Rysunek B pokazuje stronę zlinearyzowaną w jedną kolumnę, z nawigacją u góry. Rysunek C pokazuje stronę zlinearyzowaną, z nawigacją na dole. Kolejność sekcji (np. nawigacja u góry, u dołu lub w innym miejscu) zależy od projektu strony internetowej - użytkownik zwykle nie może kontrolować kolejności.
 
![Rysunek B. Strona zlinearyzowana w jedna kolumnę z nawigacją na górze](images/andi/10_P_linear_02.png)
Rysunek B 

![Rysunek C. Strona zlinearyzowana w jedna kolumnę z nawigacją na dole](images/andi/10_P_linear_03.png)
Rysunek C 

Rysunek D pokazuje stronę zlinearyzowaną z wyłączonymi stylami. Gdy wykonasz poniższe kroki sprawdzania struktury podstawowej, twoja strona będzie wyglądać mniej więcej tak:
 
![Rysunek D Strona z wyłączonymi stylami](images/andi/10_P_linear_04.png)
Rysunek D  
 
Rysunek E pokazuje stronę zmienioną przez osobę słabowidzącą, aby była bardziej czytelna, na przykład główny tekst jest duży, tekst stopki jest bardzo mały, a nagłówki mają inny kolor.
 
 
![Rysunek E](images/andi/10_P_linear_05.png)
Rysunek E  
 
Chociaż dobrze jest mieć doświadczonego użytkownika czytnika ekranu testującego strony internetowe, każdy może uzyskać wstępne wyobrażenie o potencjalnych barierach dostępu dla użytkowników czytników ekranu i innych osób, które zmieniają sposób prezentacji strony. Poniższe kroki pokazują, jak wyłączyć obrazy, wyłączyć style wyświetlania strony i linearyzować stronę w&nbsp;celu sprawdzenia struktury strony.

### Uwagi:
-	Tabele danych nie będą miały sensu, gdy zostaną zlinearyzowane – zignoruj to, ponieważ czytniki ekranu mają funkcję umożliwiającą korzystanie z tabel danych (pod warunkiem, że są odpowiednio oznakowane).
-	Demo Przed i Po daje wyraźny pogląd na to, jak podstawowy test struktury strony ujawnia bariery dostępności. (Jest to również trochę zabawne, więc sugerujemy, aby to sprawdzić, wykonując [poniższe ZŁE instrukcje]() ).

### Co robić:
Uzyskaj widok podstawowej struktury strony, postępując zgodnie z instrukcjami w sekcji Podstawowe testy struktury poniżej, aby:
-	Wyłączyć obrazy i wyświetlić teksty alternatywne.
-	Wyłączyć arkusze stylów (CSS), które określają sposób wyświetlania strony z układem, kolorami itp.
-	Zlinearyzuj stronę lub tabele (w zależności od paska narzędzi).

### Co sprawdzić:
-	Sprawdź, czy informacje mają sens, gdy są czytane w kolejności, w jakiej są wyświetlane; na przykład, czy nagłówki znajdują się tuż nad informacjami, których dotyczą. (Tabele danych nie muszą mieć sensu zlinearyzowanego, zgodnie z uwagą powyżej).
-	Sprawdź, czy tekst alternatywny zawiera odpowiednie informacje o brakujących obrazach (zgodnie z sekcją [Teksty alternatywne obrazów](02_P_odpowiedniki-tekstowe-obrazow.md)).
-	Sprawdź, czy bloki informacji mają wyraźne nagłówki (zobacz także sekcja [Nagłówki](03_P_naglowki.md)). Gdy nawigacja, główna treść i inne sekcje mają dobre nagłówki, łatwiej jest ludziom znaleźć informacje.

### Podstawowe testy struktury strony

### Sprawdzanie za pomocą paska narzędzi WebDeveloper
Aby sprawdzić podstawową strukturę za pomocą paska narzędzi WebDeveloper:

1. Otwórz stronę internetową, którą sprawdzasz, w przeglądarce z zainstalowanym paskiem narzędzi WebDeveloper.
2. Na pasku narzędzi wybierz opcję *Images* (Obrazy), a następnie *Disable Images* (Wyłącz obrazy).
3. Na pasku narzędzi wybierz *CSS*, a następnie *Disable All Styles* (Wyłącz wszystkie style).
4. Na pasku narzędzi wybierz *Miscellaneous* (Różne), a następnie *Linearize Page* (Linearyzuj stronę).

### Sprawdzenie struktury na stronie demo PrzediPo  

1. Najpierw sprawdź strukturę dostępnej wersji strony głównej: https://przedipo.lepszyweb.pl/after/home.html
   1. Wykonaj kolejno przedstawione powyżej testy, aby wyłączyć obrazy i wyłączyć CSS.
   2. Przewiń stronę w dół i zauważ, że w sekcji „Witamy w Światłach Miasta” znajdują się 3 nagłówki artykułów z tekstami zwiastunów (zapowiedzi, streszczenia, lidu) pod każdym z nagłówków.
   
   ![Fragment dostępnej wersji strony z wyłączonymi stylami](images/andi/10_P_linear-home-dostepna.png)    
   
2. Następnie sprawdź strukturę niedostępnej wersji strony głównej: https://przedipo.lepszyweb.pl/before/reports/home.html 
   1. Wykonaj kolejno przedstawione powyżej testy, aby wyłączyć obrazy i wyłączyć CSS.   
   2. Przewiń stronę w dół i zauważ, że w sekcji „Witamy w Światłach Miasta” trzy nagłówki następują jeden po drugim, a nie  przed testami, które tytułują. Teksty wszystkich trzech zwiastunów artykułów następują po sobie, tak, jakby to był jeden tekst.
   
   ![Fragment niedostępnej wersji strony z wyłączonymi stylami](images/andi/10_P_linear-home-niedostepna.png)  
	
3. Sprawdź także formularz na niedostępnej wersji strony Ankieta: https://przedipo.lepszyweb.pl/before/survey.html.
   1. Wykonaj kolejno przedstawione powyżej testy, aby wyłączyć obrazy, wyłączyć CSS i włączyć linearyzację strony (najlepiej widać w przeglądarce Firefox). Zwróć uwagę, jak rozmieszczone są pola przeznaczone na adres e-mail. Zauważ, że etykiety nie są powiązane z polami (jest tak, ponieważ strona nieprawidłowo używa tabeli układu):
   
   ![Linearyzacja strony z formularzem. Fragment](images/andi/10_P_linear-formularz.png)


