---
title: Łącza pomijające
tags: [nawigacja,struktury]
sidebar: testy_sidebar
permalink: H1-03-linki-pomijajace
folder: testy/jbt
---

## Nawigacja - Linki pomijające

### Metoda badania:
Kontrola wzrokowa i test ręczny

## Zastosowanie
_do opracowania_
## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [2.4.1 Możliwość pominięcia bloków](https://wcag.lepszyweb.pl/#bypass-blocks)
-	Jeśli pomiędzy górną krawędzią strony a jej zawartością główną znajduje się więcej niż pięć elementów interaktywnych, to na początku strony znajduje się nawigacja pomijająca – co najmniej jedno łącze do głównej treści strony.
-	Łącza w nawigacji pomijającej są łączami tekstowymi.
-	Łącza są zawsze widoczne albo stają się widoczne po otrzymaniu fokusa klawiatury
-	Uruchomienie łącza powoduje, że punkt uwagi (fokus) przenosi się na początek głównej treści strony lub do pierwszego interaktywnego elementu w wybranym obszarze strony, jeśli nawigacja pomijająca zawiera więcej  łączy.

### Procedura testowania:
1.	Odśwież stronę, aby mieć pewność, że znajduje się w stanie domyślnym.
2.	Obejrzyj stronę i zlokalizuj miejsce, w którym rozpoczyna się główna zawartość strony
3.	Sprawdź za pomocą nawigacji klawiaturą  albo za pomocą narzędzia ujawniającego interaktywne elementy strony, czy przed główną zawartością strony znajduje się więcej niż pięć elementów interaktywnych.
4.	Jeśli tak, sprawdź, czy istnieje mechanizm umożliwiający pomijanie bloków treści, które poprzedzają główną treść strony (nawigacja pomijająca).
5.	Przetestuj każde łącze w nawigacji pomijającej i sprawdź, czy po uaktywnieniu punkt uwagi (fokus) przenosi się na początek głównej treści strony lub do pierwszego interaktywnego elementu w wybranym obszarze strony.   

### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [Skip Links](https://jimthatcher.com/favelets/) z kolekcji Jima Tatchera.  Oznacza łącza pomijające oraz miejsca, do których zostanie przeniesiony użytkownik po wybraniu łącza.
-	skryptozakładka [Track focus](https://github.com/ThePacielloGroup/bookmarklets) z kolekcji Pacciello Group

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_
