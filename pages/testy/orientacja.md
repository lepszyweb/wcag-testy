---
title: Orientacja
last_updated: 22 października 2024
toc: false
sidebar: testy_sidebar
permalink: orientacja
folder: testy
---

## Wymagania dostępności
- {% include ks/1-3-4.md %} 

## Dostępność wersji alternatywnej
Identyfikator testu podstawowego: _orientacja-wyswietlacza_ / _testID-050_ 

### Test 1.A Wersja-alt-zgodna

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|---------------------------------------|
| orientacja-wyswietlacza | 1.A | Treść wyświetla się w orientacji wybranej przez użytkownika (pionowej lub poziomej) bez utraty informacji lub funkcji|

### Cel testu
Niektóre urządzenia (głównie mobilne) mogą dynamicznie zmieniać orientację ekranu, gdy zmienia się orientacja samego urządzenia. O ile takie zachowanie doskonale przydaje się w przypadku treści tekstowych, to może mieć negatywny wpływ w przypadku treści, które wymagają konkretnej orientacji urządzenia, np. gry oparte na orientacji urządzenia. 

Celem tego testu jest sprawdzenie, czy treści oferowane przez stronę internetową mogą być odtwarzane niezależnie od orientacji ekranu (pionowej lub poziomej) oraz upewnienie się, że zmiana orientacji wyświetlania nie powoduje utraty informacji lub funkcji.

Jeśli użytkownik zdecyduje się zablokować całe urządzenie w konkretnej orientacji, wszystkie strony muszą uwzględnić to ustawienie i odpowiednio wyświetlić treść.

## Zastosowanie

### Oczekiwania, ograniczenia lub wyjątki

### Identyfikacja treści

## Jak testować

### Metody i narzędzia testowe 

### Procedura testowa

### Ocena wyników
Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymagania zgodności, jeśli twierdzenie poniżej jest **fałszywe**, ten warunek testowy **nie ma zastosowania**.


## Założenia, ograniczenia lub wyjątki

- Treść jest czytelna i użyteczna niezależnie od orientacji ekranu.
- Termin „orientacja ekranu” odnosi się do tego, czy obszar widoku przeglądarki znajduje się w trybie poziomym (czyli szerokość obszaru widoku jest większa od jego wysokości), czy w trybie pionowym (wysokość obszaru widoku jest większa od jego szerokości).
- Kryterium sukcesu dotyczy tylko treści internetowych, nie dotyczy ustawień specyficznych dla urządzenia, których ktoś może użyć, aby ograniczyć swoje urządzenie do określonej orientacji. Innymi słowy, autorzy powinni tworzyć treści, które automatycznie dostosowują się do orientacji urządzenia, na którym są wyświetlane.
- Zmiany zakresu widocznych informacji lub funkcji wynikające z wielkości wyświetlacza nie są objęte tym kryterium, które koncentruje się na ograniczeniach orientacji.

### Identyfikacja treści

### Zastosowanie:
Test 1.A Wersja-alt-zgodna **nie ma zastosowania**, jeśli istnieje tylko jedna wersja treści.

### Jak testować:


### Ocena wyników
Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymagania zgodności, jeśli twierdzenie poniżej jest **fałszywe**, ten warunek testowy **nie ma zastosowania**.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G214.md %}
- {% include techniki/F97.md %}
- {% include techniki/F100.md %}



## Wymagania dostępności
- {% include ks/1-3-4.md %} 

## Uzasadnienie metody testowej




Intencją tego kryterium sukcesu jest zapewnienie, że treść wyświetla się w orientacji wybranej przez użytkownika (pionowej lub poziomej). 
Celem tego kryterium sukcesu jest to, żeby autorzy nigdy nie ograniczali orientacji treści, zapewniając w ten sposób, że zawsze będzie dopasowana do orientacji wyświetlacza urządzenia.
Niektórzy użytkownicy mają swoje urządzenia zamontowane w stałej orientacji (np. na ramieniu wózka inwalidzkiego). Dlatego strony internetowe i aplikacje muszą wspierać obie orientacje, nie ograniczając możliwości zmiany orientacji. 




•	Aplikacje nie ograniczają zmian orientacji wyświetlacza.
•	Aplikacje nie polegają na ruchu urządzenia.

Treść nie wymaga określonego ułożenia wyświetlacza (pionowego lub poziomego), poza uzasadnionymi wyjątkami 

	


Zmiany orientacji i testowanie ruchu są zwykle przeprowadzane na urządzeniach mobilnych. Gdy urządzenie mobilne jest przechylone o 90 stopni, jego czujniki wyzwalają zmianę orientacji treści. Jest to oczekiwane zachowanie na poziomie platformy, więc test zapewnia, że aplikacja nie blokuje wyświetlania treści zarówno w orientacji poziomej, jak i pionowej.

W ten sam sposób, w jaki platforma oferuje blokadę, aby zapobiec przypadkowemu wywołaniu zmiany orientacji przez użytkownika, wszelkie działania w aplikacji, które są wyzwalane przez ruch, muszą zawierać mechanizm wyłączający aktywację ruchem. 


Sprawdź, czy aplikacja zapewnia inny niż detekcja ruchu sposób aktywacji.




Niektóre strony internetowe i aplikacje automatycznie ustawiają orientację ekranu, blokują go w tej orientacji i oczekują, że użytkownicy zareagują obracając swoje urządzenie, aby dopasować się do niego, co może sprawiać problemy. 





Do sprawdzenia
Sprawdź, czy wszystkie treści i funkcje są dostępne w obu orientacjach (bez utraty informacji, bez obciętych elementów).

Oczekiwany wynik


Jest to istotne dla użytkowników, którzy mają ekran zamontowany poziomo na wózku inwalidzkim i nie mogą go obrócić.

1 na 3 osoby używa powiększonej czcionki. Orientacja pozioma ułatwia czytanie tekstu przy użyciu (bardzo) dużej czcionki.

## Założenia, ograniczenia lub wyjątki



 może mieć istotne znaczenie, np. czek bankowy, aplikacja na pianino, slajdy do projektora czy telewizora lub przedstawienie rzeczywistości wirtualnej, której treść niekoniecznie jest ograniczona do orientacji poziomej lub pionowej.
 
   - Technologie takie jak wirtualna rzeczywistość wykorzystują ekrany w goglach, które nie mogą zmienić orientacji względem oczu użytkownika.

      Wyjątek dotyczący rzeczy uznanych za istotne ma na celu sytuacje, w których treść byłaby zrozumiała tylko w określonej orientacji lub gdy technologia ogranicza możliwe orientacje. 






























## #.X Procedura testowa dla dowolna orientacja wyświetlacza
Identyfikator testu podstawowego: _7.A-dowolna-orientacja-wyswietlacza_

### Identyfikacja treści
Cała treść strony internetowej lub ekranu w aplikacji mobilnej
Użyj do testu urządzenia, które umożliwia zmianę orientacji wyświetla nia, np. smartfona, tabletu.

### Instrukcja testowania

1. Sprawdź, czy do przeglądania i obsługi treści konieczny jest widok pionowy, czy poziomy.

1. Otwórz treść w widoku poziomym. 
   - Sprawdź, czy treść jest zorientowana dla tego widoku.
2. Otwórz treść w widoku pionowym. 
   - Sprawdź, czy treść jest zorientowana dla tego widoku.

Jeśli w treści, programie użytkownika, systemie operacyjnym lub urządzeniu występują jakiekolwiek kontrolki, które ograniczają lub zezwalają na zmiany orientacji, sprawdź, czy kontrolki te można skonfigurować tak, aby sprawdzenia nr 1 i 2 były prawdziwe.


Oczekiwane rezultaty
Jeśli sprawdzenie nr 1 lub sprawdzenie nr 2 jest fałszywe, a sprawdzenia nr 3 i 4 są fałszywe, wówczas obowiązuje ten warunek niepowodzenia i treść nie spełnia kryterium sukcesu.



Procedura
W przypadku treści, które nie zmieniają orientacji podczas obracania urządzenia:

Sprawdź, czy w interfejsie użytkownika znajduje się kontrolka umożliwiająca zmianę orientacji treści.
Sprawdź, czy po użyciu elementu sterującego następuje zmiana orientacji zawartości.
Oczekiwane rezultaty
Sprawdzenia nr 1 i nr 2 są prawdziwe.

Procedura
Otwórz zawartość w widoku poziomym. Sprawdź, czy pojawi się komunikat z prośbą o zmianę orientacji urządzenia.
Otwórz zawartość w widoku pionowym. Sprawdź, czy pojawi się komunikat z prośbą o zmianę orientacji urządzenia.
Sprawdź, czy do przeglądania i obsługi treści konieczny jest widok pionowy czy poziomy.
Oczekiwane rezultaty
Jeśli sprawdzenie nr 1 lub nr 2 jest prawdą, a sprawdzenie nr 3 jest fałszem, wówczas ten warunek testowy ma zastosowanie i treść nie spełnia kryterium sukcesu.


### Wynik testów
Jeśli WSZYSTKIE powyższe testy zakończą się niepowodzeniem, test podstawowy _7.A-Color_ kończy się niepowodzeniem.


##  Wskazówki dotyczące usprawniania procesu testowego

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G214.md %}
- {% include techniki/F97.md %}
- {% include techniki/F100.md %}