---
title: Nawigacja - Menu nawigacyjne

sidebar: testy_sidebar
permalink: H1-05-menu-nawigacyjne
folder: testy/jbt
---

## Nawigacja - Menu nawigacyjne

### Metoda badania:
Kontrola wizualna. Test obsługi za pomocą klawiatury. Test obsługi za pomocą czytnika ekranu. Inspekcja kodu.

## Zastosowanie
_do opracowania_
## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [2.4.5 Wiele dróg](https://wcag.lepszyweb.pl/#multiple-ways).
-	Menu można rozpoznać jako takie dzięki odpowiedniej stylizacji i oznaczeniu np. etykietą.  
-	Główne menu nawigacyjne znajduje się w miejscu, w którym spodziewają się je znaleźć użytkownicy (góra strony, boczny pasek).
-	Paski nawigacyjne na różnych stronach znajdują się zawsze w tych samych miejscach.
-	Pozycje w menu pojawiają się w tej samej kolejności.
-	Każde menu jest objęte znacznikiem `nav` i opisane etykietą lub nagłówkiem odróżniającym je od innych menu na stronie.   
-	Struktura menu jest utworzona za pomocą listy nieuporządkowanej, a w uzasadnionych przypadkach listy uporządkowanej.
-	Teksty pozycji menu są zwięzłe, czytelne, dopasowane  do rozmiaru tekstu na stronie.
-	Rozmiary obszarów wyboru pozycji menu są odpowiednie, aby je wybrać dotykiem
-	Specjalne stany pozycji menu – bieżąca (aktywna), wskazywana, fokusowana są wyróżnione.  
-	Podczas nawigacji klawiszem Tab podmenu nie rozwija się i można je pominąć.
-	Istnienie i stan podmenu są ogłaszane użytkownikom czytników ekranu dzięki zastosowaniu atrybutów `aria-haspopup` i `aria-expanded`.

### Procedura testowania:
1.	Sprawdź, czy na wszystkich stronach menu znajdują się w spodziewanych tych samych miejscach.
2.	Nawiguj między wszystkimi pozycjami menu za pomocą klawisza Tab i klawiszy strzałek, sprawdź, czy w każdym momencie możesz przejść do następnej i poprzedniej pozycji oraz opuścić menu.
3.	Użyj narzędzia kontrolnego, aby określić rolę i stan pozycji menu z podmenu
4.	Testuj ręcznie za pomocą klawiatury i czytnika ekranu, aby ustalić, czy podmenu otwiera się tylko po akcji użytkownika
5.	Testuj ręcznie za pomocą czytnika ekranu, aby ustalić, czy stan jest przekazywany poprawnie

### Zasoby

#### Pomocne narzędzia:

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_
