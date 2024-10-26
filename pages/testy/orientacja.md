---
title: Orientacja
last_updated: 22 października 2024
toc: false
sidebar: testy_sidebar
permalink: Orientacja
folder: testy
---

## Wymagania dostępności
- {% include ks/1-3-4.md %} 

## Test Orientacja wyświetlania
Identyfikator testu podstawowego: _orientacja-wyswietlania_ / _testID-050_ 

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|---------------------------------------|
| orientacja-wyswietlania | ??? | Treść wyświetla się w orientacji wybranej przez użytkownika (pionowej lub poziomej) bez utraty informacji lub funkcji|

## Cel testu
Celem tego testu jest sprawdzenie, czy treści oferowane przez stronę internetową mogą być odtwarzane niezależnie od orientacji ekranu (pionowej lub poziomej). Jeśli użytkownik zdecyduje się zablokować całe urządzenie w konkretnej orientacji, wszystkie strony muszą uwzględnić to ustawienie i odpowiednio wyświetlić treść.

<!-- Niektóre urządzenia (głównie mobilne) mogą dynamicznie zmieniać orientację ekranu, gdy zmienia się orientacja samego urządzenia. O ile takie zachowanie doskonale przydaje się w przypadku treści tekstowych, to może mieć negatywny wpływ w przypadku treści, które wymagają konkretnej orientacji urządzenia, np. gry oparte na orientacji urządzenia. -->

## Oczekiwania, ograniczenia lub wyjątki

- Treść jest czytelna i użyteczna niezależnie od orientacji ekranu, z wyjątkiem sytuacji, gdy konkretna orientacja wyświetlania ma <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.istotny | strip_html | replace: '*', ''}}">istotne</a> znaczenie. 
   - **Uwaga do KS 1.3.4**: Przykłady, w których konkretna orientacja wyświetlania może mieć istotne znaczenie, to np. czek bankowy, aplikacja na pianino, slajdy do projektora czy telewizora lub treść rzeczywistości wirtualnej, gdy treść nie musi być ograniczona do orientacji poziomej lub pionowej.
   -  **Wyjątek**. Wyjątek odnosi się do poniższych dwóch sytuacji, w których treść może być w pełni czytelna i użyteczna tylko w określonej orientacji lub gdy technologia ogranicza możliwe orientacje: 
      - gdy treść wymaga konkretnej (zwykle poziomej) orientacji wyświetlania, aby można jej efektywnie użyć, np. aplikacja do gry na pianinie wymaga prezentacji w widoku poziomym, aby zapewnić wystarczającą ilość miejsca na klawisze (w przecinym przypadku klawiszy byłoby zbyt mało albo byłyby zbyt wąskie);
      - gdy treść jest przeznaczona dla określonego środowiska, które jest dostępne tylko w jednej orientacji (np. telewizor, okulary wirtualne), wówczas możliwe orientacje ogranicza technologia.
- Termin „orientacja ekranu” odnosi się do tego, czy obszar widoku przeglądarki znajduje się w trybie poziomym (czyli szerokość obszaru widoku jest większa od jego wysokości), czy w trybie pionowym (wysokość obszaru widoku jest większa od jego szerokości).
- Kryterium sukcesu dotyczy tylko treści internetowych, nie dotyczy ustawień specyficznych dla urządzenia, których ktoś może użyć, aby ograniczyć swoje urządzenie do określonej orientacji. Innymi słowy, autorzy powinni tworzyć treści, które automatycznie dostosowują się do orientacji urządzenia, na którym są wyświetlane.
- Zmiany zakresu widocznych informacji lub funkcji wynikające z wielkości wyświetlacza nie są objęte tym kryterium, które koncentruje się na ograniczeniach orientacji. Zmiana orientacji może wymagać przewijania ekranu w dół, aby zobaczyć całą treść.

## Identyfikacja treści
Wszystkie treści, **z wyjątkiem sytuacji**, gdy do przeglądania i obsługi treści konieczny jest widok pionowy albo poziomy.
Ogranicz badanie tylko do zachowania się treści w urządzeniach, które umożliwiają zmianę orientacji ekranu.

## Zastosowanie:
Test _orientacja-wyswietlania_ **nie ma zastosowania** do treści, które muszą być wyświetlone w konkretnej orientacji widoku (ekranu).

## Jak testować:
1. Sprawdź, czy treść można przeglądać i obsługiwać w widoku poziomym.
2. Sprawdź, czy treść można przeglądać i obsługiwać w widoku pionowym.  
3. Jeśli w treści, programie użytkownika, systemie operacyjnym lub urządzeniu występują jakiekolwiek kontrolki, które ograniczają lub zezwalają na zmiany orientacji,
   - Sprawdź, czy po użyciu kontrolki następuje zmiana orientacji treści.
   - Sprawdź, czy treść można przeglądać i obsługiwać w widoku poziomym.
   - Sprawdź, czy treść można przeglądać i obsługiwać w widoku pionowym.
   - Sprawdź, czy zmiana orientacji widoku nie powoduje utraty informacji lub funkcji.
4. Jeśli pojawi się komunikat z prośbą o zmianę orientacji urządzenia, sprawdź czy do przeglądania i obsługi treści konieczna jest żądana orientacja urządzenia (orientacja widoku). 
 
## Ocena wyników
Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** warunki testowe i test podstawowy _orientacja-wyswietlania_ kończy się wynikiem **zaliczony**.
Jeśli którekolwiek twierdzenie poniżej jest **fałszywe**, wówczas strona (treść) **nie spełnia** warunków testowych i test podstawowy _orientacja-wyswietlania_ kończy się niepowodzeniem (wynikiem **niezaliczony**).

1. Użycie kontrolek zmiany oientacji, jeśli istnieją, powoduje zmianę orientacji treści.
2. Treść można przeglądać zarówno w widoku poziomym, jak i w widoku pionowym.
3. Zmiana orientacji widoku nie powoduje utraty informacji lub funkcji.
4. Żądana orientacja widoku (ekranu), jeśli ma miejsce, jest konieczna do przeglądania i obsługi treści. 

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G214.md %}
- {% include techniki/F97.md %}
- {% include techniki/F100.md %}
