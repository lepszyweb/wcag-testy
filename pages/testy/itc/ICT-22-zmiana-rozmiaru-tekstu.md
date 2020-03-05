---
title: 22. Zmiana rozmiaru tekstu


sidebar: testy_sidebar
permalink: ICT-22-zmiana-rozmiaru-tekstu
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/1-4-4.md %}

## Uzasadnienie metody badania
Ten test podstawowy wymaga oceny wizualnej treści i funkcjonalności po zmianie rozmiaru tekstu.

## Ograniczenia, założenia lub wyjątki

-   Wyjątek: Napisy obrazy tekstu nie są uwzględniane w teście.

## Procedura testu dla 1.4.4 Zmiana rozmiaru tekstu

### Identyfikacja treści
Cały tekst na stronie.

### Instrukcja testowania
1.  Sprawdź, czy istnieje mechanizm zmiany rozmiaru, skalowania lub powiększania zawartości co najmniej do 200% oryginalnego rozmiaru. Znane rozwiązania obejmują:
    -   funkcja powiększania w przeglądarce,
	-   funkcje dostępności zapewniane przez platformę lub system operacyjny,
    -   Kontrolki do zmiany rozmiaru tekstu. (Jeśli funkcja powiększenia przeglądarki, systemu operacyjnego lub platformy nie jest obsługiwana przez stronę, strona musi zawierać mechanizm zmiany rozmiaru).
2.  Zmodyfikuj rozmiar czcionki, aby zwiększyć dwukrotnie szerokość i wysokość lub zwiększyć ją o 200%.
3.  Sprawdź wszystkie następujące elementy:
    -   tekst nie jest skracany, obcinany ani zasłaniany
    -   tekst wprowadzany w polach formularza również zmienia rozmiar
    -   cała funkcjonalność jest dostępna
    -   cała zawartość jest dostępna

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.4.4  oraz Wymaganie podstawowe nr 10 kończy się niepowodzeniem.

## Wskazówki dotyczące usprawniania procesu testów
brak

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G178.md %}
- {% include techniki/G179.md %}
- {% include techniki/F69.md %}
- {% include techniki/F80.md %}
- {% include techniki/F94.md %}
